# Guest Program Execution Under KVM (Full Flow) : start from lv.c
                         ┌────────────────────────┐
                         │     GUEST PROGRAM      │
                         │   (runs on VCPU HW)    │
                         └───────────┬────────────┘
                                     │
                                     ▼
                           (1) Normal execution
                                     │
                                     ▼
                 ┌────────────────────────────────────┐
                 │ Does instruction/event require exit│
                 │ (IO, MMIO, CPUID, HLT, NPF, INT)?  │
                 └──────────┬─────────────────────────┘
                            │ No
                            ▼
                    Continue guest execution
                            │
                            └───► loops back forever
                            │ Yes
                            ▼
         ┌────────────────────────────────────────────────┐
         │        HARDWARE VMEXIT (AMD SVM EXIT)         │
         │   VMCB.control.exit_code = SVM_EXIT_xxx       │
         └──────────────────────────┬─────────────────────┘
                                    │
                                    ▼
             ┌────────────────────────────────────┐
             │        KVM (svm.c in kernel)       │
             │  Interpret SVM_EXIT_xxx from VMCB  │
             └──────────────────────┬─────────────┘
                                    │
                ┌─────────────────────────────────────┐
                │   Does KVM handle this internally?  │
                │   (CRx, DRx, RDTSC, LGDT, LIDT…)   │
                └───────────────┬─────────────────────┘
                                │
                                │_________________________________
                                │                                 │
                                │ Yes                             │
                                ▼                                 │
            ┌────────────────────────────────────────────┐        │
            │  KVM emulates instruction internally       │        │
            │  updates registers, RIP, RFLAGS etc.       │        │
            └─────────────────┬──────────────────────────┘        │
                              │                                   │
                              ▼                                   │
                     Resume GUEST execution                       │
                       (hardware VMRUN)                           │
                              │                                   │
                              └─────► loops back                  │
                                                                  │
                                ──────────────────────────────────
                                │ No
                                ▼
       ┌─────────────────────────────────────────────────────────┐
       │   KVM translates VMEXIT to generic KVM_EXIT_xxx         │
       │   Examples:                                             │
       │      SVM_EXIT_IOIO    → KVM_EXIT_IO                     │
       │      SVM_EXIT_CPUID   → KVM_EXIT_CPUID                  │
       │      SVM_EXIT_MSR     → KVM_EXIT_MSR                    │
       │      SVM_EXIT_NPF     → KVM_EXIT_MMIO                   │
       │      SVM_EXIT_HLT     → KVM_EXIT_HLT                    │
       └───────────────────────┬─────────────────────────────────┘
                               │
                               ▼
                Userspace exit: ioctl(KVM_RUN) returns
                            to QEMU
                               │
                               ▼
                   ┌───────────────────────┐
                   │     QEMU (userspace)  │
                   │      kvm_cpu_exec     │
                   └───────────┬───────────┘
                               │
                ┌──────────────────────────────────┐
                │   switch(run->exit_reason)       │
                │                                   │
                │   case KVM_EXIT_IO:               │
                │         → QEMU device model       │
                │   case KVM_EXIT_MMIO:             │
                │         → QEMU memory access      │
                │   case KVM_EXIT_CPUID:            │
                │         → userspace CPUID emulate │
                │   case KVM_EXIT_MSR:              │
                │         → MSR emulation           │
                │   case KVM_EXIT_HLT:              │
                │         → idle/continue           │
                └─────────────────┬─────────────────┘
                                  │
                                  ▼
                     QEMU updates VCPU state
                                  │
                                  ▼
                         Re-enter guest:
                         ioctl(KVM_RUN)
                                  │
                                  ▼
                            GUEST continues






# No VM only run Guest program full emulation: start from linux-user/main.c
         +-----------------------+
         | qemu-i386 (linux-user)|
         +-----------+-----------+
                     |
                     v
            Parse ELF binary
              load segments
                     |
                     v
           Setup CPUState (fake)
             - registers
             - stack
             - PC = entry point
                     |
                     v
            Start main loop:
            cpu_loop(env)
                     |
                     v
         +-----------------------------+
         | TCG translates guest code   |
         | into host instructions      |
         +-----------------------------+
                     |
                     v
             Execute guest code
                     |
                     v
          Does guest execute a syscall?
                     |
       +-------------+--------------+
       | Yes                        | No
       v                             v
Emulate syscall in QEMU        Continue TCG block
   - open/read/write
   - fork/clone (NOTE: in KVM, its guest os responsibility and qemu will not handle these system call)
   - mmap/brk
   - futex
   - signal handling
   - any Linux syscall
       |
       v
  Produce syscall result
     like kernel does
       |
       v
Return to guest instruction
       |
       v
Guest continues execution
       |
       └─── loop forever until exit()
