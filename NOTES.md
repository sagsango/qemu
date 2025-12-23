# keyboard press
┌──────────────────────────────────────────────────────────────┐
│                    HOST HARDWARE                             │
├──────────────────────────────────────────────────────────────┤
│                                                              │
│   Physical Keyboard                                          │
│        │                                                     │
│        ▼                                                     │
│   AT / USB Keyboard Controller                               │
│        │                                                     │
│        ▼                                                     │
│   Linux Kernel Input Stack                                   │
│   ├─ atkbd / usbhid                                         │
│   ├─ serio / usbcore                                        │
│   └─ evdev                                                  │
│        │                                                     │
│        ▼                                                     │
│   /dev/input/eventX                                         │
│        │                                                     │
│        ▼                                                     │
│   X Server (Xorg)                                           │
│   ├─ Reads evdev                                            │
│   ├─ Applies keymaps (XKB)                                  │
│   └─ Generates X11 KeyPress / KeyRelease                    │
│        │                                                     │
│        │   (Window Manager only controls focus)              │
│        ▼                                                     │
│   SDL (X11 backend)                                         │
│   ├─ SDL_PollEvent()                                        │
│   ├─ SDL_KEYDOWN / SDL_KEYUP                                │
│   └─ X11 internally via libX11                              │
│        │                                                     │
│        ▼                                                     │
│   QEMU (userspace process)                                  │
│                                                              │
│   ┌──────────────────────────────────────────────────────┐  │
│   │ sdl.c                                                │  │
│   │                                                      │  │
│   │ while (SDL_PollEvent(&ev)) {                         │  │
│   │   case SDL_KEYDOWN:                                  │  │
│   │   case SDL_KEYUP:                                    │  │
│   │       sdl_process_key(ev);                           │  │
│   │ }                                                    │  │
│   └──────────────────────────────────────────────────────┘  │
│        │                                                     │
│        ▼                                                     │
│   ┌──────────────────────────────────────────────────────┐  │
│   │ x_keymap.c                                           │  │
│   │                                                      │  │
│   │ SDL / X11 keysym                                     │  │
│   │        ↓                                             │  │
│   │ QEMU internal keycode                                │  │
│   │        ↓                                             │  │
│   │ PC AT scancode (set 1 / set 2)                       │  │
│   └──────────────────────────────────────────────────────┘  │
│        │                                                     │
│        ▼                                                     │
│   ┌──────────────────────────────────────────────────────┐  │
│   │ kbd.c                                                │  │
│   │                                                      │  │
│   │ kbd_put_keycode()                                   │  │
│   │ kbd_put_keysym()                                    │  │
│   └──────────────────────────────────────────────────────┘  │
│        │                                                     │
│        ▼                                                     │
│   ┌──────────────────────────────────────────────────────┐  │
│   │ hw/i8042.c                                           │  │
│   │                                                      │  │
│   │ ps2_put_keycode()                                   │  │
│   │ Emulated PS/2 controller                             │  │
│   │ Raises IRQ1                                          │  │
│   └──────────────────────────────────────────────────────┘  │
│        │                                                     │
│        ▼                                                     │
│   ┌──────────────────────────────────────────────────────┐  │
│   │ Virtual PIC / APIC                                   │  │
│   │ Injects interrupt into guest CPU                    │  │
│   └──────────────────────────────────────────────────────┘  │
│        │                                                     │
│        ▼                                                     │
│   Guest IDT[33]  (IRQ1)                                     │
│        │                                                     │
│        ▼                                                     │
│   Guest OS Keyboard Driver                                  │
│   (e.g. Linux atkbd.c)                                      │
│                                                              │
└──────────────────────────────────────────────────────────────┘

# Keyboard press virtio
═══════════════════════════════════════════════════════════════════════
           KEYPRESS FLOW — QEMU + KVM + VIRTIO-INPUT
═══════════════════════════════════════════════════════════════════════

[ Physical Keyboard ]
        |
        v
[ USB / HID Controller ]
        |
        v
=========================== HOST KERNEL ===============================
        |
        v
IRQ → usb_hcd_irq()
        |
        v
HID keyboard driver
        |
        v
input_report_key(KEY_A)
        |
        v
/dev/input/eventX
========================== HOST USERSPACE =============================
        |
        v
QEMU input core
        |
        v
virtio-input backend
        |
        v
Fill virtqueue:
  struct virtio_input_event
        |
        v
============================ PCI BUS =================================
        |
        v
MSI-X interrupt
============================== KVM ===================================
        |
        v
KVM_SIGNAL_MSI
=========================== GUEST CPU ================================
        |
        v
IDT[MSI vector]
        |
        v
common_interrupt
        |
        v
handle_irq_event()
========================== GUEST KERNEL ===============================
        |
        v
virtio_input_irq()
        |
        v
virtqueue_get_buf()
        |
        v
input_report_key(KEY_A)
        |
        v
/dev/input/eventX
        |
        v
TTY line discipline (n_tty)
========================= GUEST USERSPACE =============================
        |
        v
Shell / Application
        |
        v
read(STDIN) → 'A'
═══════════════════════════════════════════════════════════════════════


# keyboard press no virtio
══════════════════════════════════════════════════════════════════════
                 KEY PRESS FLOW — QEMU + KVM + LINUX
══════════════════════════════════════════════════════════════════════

[ Physical Keyboard ]
        |
        v
[ USB / PS2 Controller ]
        |
        v
======================== HOST KERNEL ========================
        |
        v
IRQ → usb_hcd_irq() / i8042_interrupt()
        |
        v
HID / AT keyboard driver
        |
        v
input_report_key(KEY_A)
        |
        v
input_event()
        |
        v
/dev/input/eventX
======================== HOST USERSPACE =====================
        |
        v
QEMU frontend (SDL/GTK/evdev)
        |
        v
qemu_input_event_send_key()
        |
        v
Emulated Keyboard Device
  (i8042 / USB / virtio-input)
        |
        v
=========================== KVM =============================
        |
        v
ioctl(KVM_INTERRUPT)
        |
        v
Inject virtual IRQ
========================= GUEST CPU =========================
        |
        v
IDT[IRQ1]
        |
        v
common_interrupt
        |
        v
do_IRQ()
        |
        v
handle_irq_event()
        |
        v
i8042_interrupt()
======================== GUEST KERNEL =======================
        |
        v
atkbd.c
        |
        v
input_report_key()
        |
        v
/dev/input/eventX
        |
        v
TTY line discipline (n_tty)
        |
        v
====================== GUEST USERSPACE ======================
        |
        v
Shell / Application
        |
        v
read(STDIN) → 'A'
══════════════════════════════════════════════════════════════════════

