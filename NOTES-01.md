# Works well with linux kernel v2.6.20

# LEVEL 1 — High-Level Overview
+---------+    KVM_RUN     +-----------+    VMEXIT     +----------+
|  QEMU   | --------------> |   KVM     | ------------> |   QEMU   |
| (userspace)  <----------  | (kernel)  | <------------ |          |
+---------+   return(exit)  +-----------+  resume(run) +----------+


# LEVEL 2 — Execution Pipeline Overview (with CPU)
      QEMU user-space
           |
           | ioctl(KVM_RUN)
           v
      +--------------------+
      |       KVM          |
      |   (kernel driver)  |
      +--------------------+
           |
           | vcpu->enter
           v
+----------------------------------+
|               CPU                |
|    (VMX/SVM Guest Execution)     |
+----------------------------------+
           |
           | VM-EXIT (reason)
           v
      +------------------------+
      |       KVM kernel       |
      |   (fill kvm_run data)  |
      +------------------------+
           |
           | return from ioctl
           v
      +------------------------+
      |        QEMU            |
      |  Handle exit reason    |
      +------------------------+


# LEVEL 3 — Detailed Flow: From QEMU → run guest → exit → QEMU
   ┌───────────────────────────────────────────────────────────────┐
   │                           QEMU                                │
   │                      (target-i386/kvm.c)                      │
   └───────────────────────────────────────────────────────────────┘
                 |
                 | 1. ioctl(KVM_RUN)
                 v
   ┌───────────────────────────────────────────────────────────────┐
   │                              KVM                             │
   │                  (kernel virtualization module)              │
   └───────────────────────────────────────────────────────────────┘
                 |
                 | 2. Prepare vCPU state
                 |    - load registers
                 |    - load CR0, CR3, CR4
                 |    - load segment desc.
                 |    - load MSRs (EFER, APIC base)
                 |
                 | 3. Enter CPU virtualization
                 v
┌────────────────────────────────────────────────────────────────────────┐
│                           CPU PROCESSOR                                │
│          Intel VMX: VMRESUME / VMLAUNCH                                │
│          AMD  SVM: VMRUN                                               │
└────────────────────────────────────────────────────────────────────────┘
                 |
                 | Guest executes instructions
                 | Hardware runs guest mode
                 |
                 | (any exit condition)
                 v
┌────────────────────────────────────────────────────────────────────────┐
│                        VM EXIT (hardware)                             │
└────────────────────────────────────────────────────────────────────────┘
                 |
                 | 4. CPU → KVM exit handler in kernel
                 |
                 | KVM populates: struct kvm_run.exit_reason =
                 |    - MMIO?
                 |    - IO?
                 |    - HLT?
                 |    - SHUTDOWN?
                 |    - EXCEPTION?
                 |    - EPT/NPT fault?
                 |    - APIC?
                 |
                 v
   ┌───────────────────────────────────────────────────────────────┐
   │                             KVM                               │
   │         (kernel writes info into shared kvm_run struct)       │
   └───────────────────────────────────────────────────────────────┘
                 |
                 | 5. ioctl(KVM_RUN) returns to userspace
                 v
   ┌───────────────────────────────────────────────────────────────┐
   │                             QEMU                              │
   │              Handles exit reason → acts accordingly           │
   └───────────────────────────────────────────────────────────────┘


# LEVEL 4 — Branching Flow: What Happens on Different VM-EXITs
                           ┌───────────────┐
                           │ VM-EXIT event │
                           └───────┬───────┘
                                   |
     ┌─────────────────────────────┼────────────────────────────┐
     v                             v                            v
┌──────────────┐           ┌──────────────┐             ┌──────────────┐
│   MMIO       │           │     PIO      │             │     HLT      │
│ (exit=mmio)  │           │ (exit=io)    │             │ (exit=hlt)   │
└─────┬────────┘           └─────┬────────┘             └─────┬────────┘
      |                          |                            |
      v                          v                            v
┌──────────────┐           ┌──────────────┐             ┌──────────────────┐
│   QEMU       │           │    QEMU      │             │  QEMU checks     │
│ device model │           │  I/O port    │             │  for pending IRQ │
└─────┬────────┘           └─────┬────────┘             └───────┬───────-──┘
      |                          |                              |
      v                          v                              v
┌──────────────┐           ┌──────────────┐             ┌──────────────────┐
│ emulate read │           │ emulate port │             │ sleep until IRQ  │
│ or write     │           │ in/out ops   │             └──────────────────┘
└─────┬────────┘           └─────┬────────┘
      |                          |
      v                          v
  ioctl(KVM_RUN)                ioctl(KVM_RUN)
             (continue guest execution)



# LEVEL 5 — Full Super-Detailed Flow (Complete Cycle)
┌────────────────────────────────────────────────────────────────────────────────────────┐
│                                        QEMU                                            │
│                               target-i386/kvm.c                                        │
└────────────────────────────────────────────────────────────────────────────────────────┘
                                      |
                                      | prepare vcpu state
                                      v
                      ┌────────────────────────────────────┐
                      │    ioctl(vcpu_fd, KVM_RUN)         │
                      └────────────────────────────────────┘
                                      |
                                      v
┌────────────────────────────────────────────────────────────────────────────────────────┐
│                                    KVM (kernel)                                        │
│                             arch/x86/kvm/x86.c                                         │
└────────────────────────────────────────────────────────────────────────────────────────┘
                                      |
                                      | load guest registers into hardware VMCS/VMCB
                                      |
                                      | evaluate pending IRQs/NMIs
                                      |
                                      v
                    ┌─────────────────────────────────────────────┐
                    │        CPU enters guest mode                │
                    │   Intel: VMRESUME / AMD: VMRUN              │
                    └─────────────────────────────────────────────┘
                                      |
                                      | Guest executes instructions
                                      | Hardware performs VMX/SVM transitions
                                      |
                                      v
                    ┌─────────────────────────────────────────────┐
                    │        VM EXIT on some condition           │
                    └─────────────────────────────────────────────┘
                                      |
                                      | hardware dumps exit code to VMCS/VMCB
                                      |
                                      v
             ┌────────────────────────────────────────────────────────────────────────┐
             │                         Back in KVM kernel                             │
             └────────────────────────────────────────────────────────────────────────┘
                                      |
                                      | decode exit reason
                                      |
                                      | fill struct kvm_run { exit_reason = ... }
                                      |
                                      v
                        ┌────────────────────────────────────────┐
                        │ return to QEMU from ioctl()            │
                        └────────────────────────────────────────┘
                                      |
                                      | QEMU reads kvm_run->exit_reason
                                      v
┌────────────────────────────────────────────────────────────────────────────────────────┐
│                                  QEMU handles exit                                     │
├────────────────────────────────────────────────────────────────────────────────────────┤
│ if MMIO     → handle with device model (read/write, update state)                      │
│ if PIO      → handle in port I/O handlers                                              │
│ if HLT      → wait for IRQ, then resume                                                │
│ if INTR     → process host events, inject guest IRQs                                   │
│ if SHUTDOWN → stop VM                                                                   │
│ if FAIL     → software fallback or abort                                                │
└────────────────────────────────────────────────────────────────────────────────────────┘
                                      |
                                      | prepare next vcpu state update
                                      v
                        ┌────────────────────────────────────────┐
                        │ ioctl(KVM_RUN) again                   │
                        └────────────────────────────────────────┘
                                      |
                                      v
                              Guest re-enters CPU

