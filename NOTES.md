Very basic POC of qemu
 - elf reading
 - instruction decoding
 - instruction trnslation
 - virtualization of resources
    - cpu
    - memory
    - signal
    - fd
    - thread/fork - system calls
 - basic testing of all the above
 - it did not targeted the whole kernel image
 - this was the baby star who made billion doller impact in next 2 decade.

.
├── Changelog
├── config.log
├── configure
├── COPYING
├── COPYING.LIB
├── cpu-i386.h
├── dis-asm.h
├── dis-buf.c
├── dyngen.c        : Its independent code to test - convernts object file into c like equivalent instruction
├── elf.h
├── exec-i386.c     : execution loop which fetches the instruction then decode if needed then call the equivalent trslated function.
├── exec-i386.h
├── gen-i386.h
├── i386-dis.c      : diss assembler 
├── i386.ld
├── linux-user
│   ├── elfload.c   : loading the elf, and init reg appropriatly!
│   ├── ioctls.h
│   ├── main.c      : Guest(qemu) starts here!
│   ├── qemu.h
│   ├── signal.c
│   ├── syscall_defs.h  : More syscall defs
│   ├── syscall_types.h : More syscall structs
│   └── syscall.c       : syscall emulation; this is very importent because we see many resource virtualization happen here 
├── Makefile
├── NOTES.md
├── op-i386.c       : unit asm op functions
├── opc-i386.h
├── opreg_template.h
├── ops_template.h
├── ppc.ld
├── README
├── syscall-i386.h  : syscall number, syscall arg struct
├── tests
│   ├── hello.c
│   ├── Makefile
│   ├── test-i386-code16.S
│   ├── test-i386-muldiv.h
│   ├── test-i386-shift.h
│   ├── test-i386.c
│   ├── test-i386.h
│   ├── testclone.c
│   ├── testsig.c
│   └── testthread.c
├── thunk.c
├── thunk.h
├── TODO
├── translate-i386.c
└── VERSION

3 directories, 48 files
