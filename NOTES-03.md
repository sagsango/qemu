# keyboard - interrupt & data delivery
┌──────────────────────────────────────────────────────────────┐
│                        HOST USERSPACE                        │
│                                                              │
│  ┌──────────────┐                                            │
│  │ X11 / SDL    │                                            │
│  │ (host GUI)   │                                            │
│  └──────┬───────┘                                            │
│         │  Key press (host keycode)                          │
│         ▼                                                    │
│  ┌──────────────────────────┐                                │
│  │ QEMU 0.10 (userspace)    │                                │
│  │                          │                                │
│  │ ① Translate keycode      │                                │
│  │   host → PC scancode     │                                │
│  │   (e.g., 'A' → 0x1E)     │                                │
│  │                          │                                │
│  │ ② Emulated i8042 write   │                                │
│  │   --------------------   │                                │
│  │   kbd.output_buf = 0x1E  │◄────── DATA STORED HERE        │
│  │   kbd.status |= OBF      │                                │
│  │                          │                                │
│  │ ③ Raise IRQ1             │                                │
│  │   qemu_set_irq(IRQ1, 1)  │                                │
│  └──────────┬───────────────┘                                │
│             │                                                │
│             │ KVM_INTERRUPT / pending IRQ                    │
│             ▼                                                │
│  ┌──────────────────────────┐                                │
│  │        KVM (kernel)      │                                │
│  │                          │                                │
│  │ ④ Mark IRQ1 pending      │                                │
│  │   for vCPU               │                                │
│  │                          │                                │
│  └──────────┬───────────────┘                                │
│             │                                                │
│             │ ioctl(KVM_RUN)                                 │
│             ▼                                                │
│  ┌──────────────────────────────────────────────────────────┐│
│  │                    GUEST CPU EXECUTION                   ││
│  │                                                          ││
│  │ ⑤ vCPU enters guest mode                                 ││
│  │                                                          ││
│  │ ⑥ CPU sees IRQ1 pending                                  ││
│  │   → vectors via IDT                                      ││
│  │                                                          ││
│  │ ⑦ Guest keyboard ISR starts                              ││
│  │                                                          ││
│  │ ⑧ Guest executes:                                        ││
│  │      inb $0x60, %al                                      ││
│  │                                                          ││
│  │      ⚠️ I/O instruction                                   ││
│  │      → VM-EXIT (KVM_EXIT_IO)                             ││
│  └──────────┬───────────────────────────────────────────────┘│
│             │                                                │
│             │ VM-EXIT reason: I/O PORT READ                  │
│             ▼                                                │
│  ┌──────────────────────────┐                                │
│  │ QEMU (userspace again)   │                                │
│  │                          │                                │
│  │ ⑨ Handle KVM_EXIT_IO     │                                │
│  │   port == 0x60           │                                │
│  │                          │                                │
│  │   return kbd.output_buf  │◄────── DATA FINALLY COPIED     │
│  │   clear OBF flag         │        INTO GUEST CPU          │
│  │                          │                                │
│  └──────────┬───────────────┘                                │
│             │                                                │
│             │ resume guest                                   │
│             ▼                                                │
│  ┌──────────────────────────────────────────────────────────┐│
│  │                 GUEST CONTINUES                          ││
│  │                                                          ││
│  │ ⑩ %al now contains scancode 0x1E                         ││
│  │                                                          ││
│  │ ⑪ Linux input stack processes key                        ││
│  │                                                          ││
│  └──────────────────────────────────────────────────────────┘│
└──────────────────────────────────────────────────────────────┘
