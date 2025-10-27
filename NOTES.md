.
├── a.out.h          Header for a.out executable format support.
├── acl.c            Implementation of access control lists for QEMU.
├── acl.h            Declarations for access control lists.
├── aes.c            AES encryption algorithm implementation.
├── aes.h            Header for AES encryption functions.
├── aio.c            Asynchronous I/O operations core.
├── alpha-dis.c      Alpha architecture disassembler.
├── alpha.ld         Linker script for Alpha target.
├── arch_init.c      Architecture-specific initialization routines.
├── arch_init.h      Headers for architecture initialization.
├── arm-dis.c        ARM architecture disassembler.
├── arm-semi.c       ARM semihosting support.
├── arm.ld           Linker script for ARM target.
├── async.c          Asynchronous operation helpers.
├── audio            Directory for audio device emulation.
├── balloon.c        Memory ballooning device for VM guests.
├── balloon.h        Headers for memory ballooning.
├── bitmap.c         Bitmap manipulation utilities.
├── bitmap.h         Headers for bitmap operations.
├── bitops.c         Bit operations library.
├── bitops.h         Headers for bit operations.
├── block            Directory for block device layer.
├── block_int.h      Internal headers for block layer.
├── block-migration.c Live block device migration.
├── block-migration.h Headers for block migration.
├── block.c          Block driver core implementation.
├── block.h          Public headers for block layer.
├── blockdev.c       Block device management commands.
├── blockdev.h       Headers for block device commands.
├── bsd-user         Directory for BSD user-mode emulation.
├── bswap.h          Byte swap utilities header.
├── bt-host.c        Bluetooth host controller emulation.
├── bt-host.h        Headers for Bluetooth host.
├── bt-vhci.c        Bluetooth virtual HCI device.
├── buffered_file.c  Buffered file I/O implementation.
├── buffered_file.h  Headers for buffered file I/O.
├── cache-utils.c    Cache line utilities.
├── cache-utils.h    Headers for cache utilities.
├── Changelog        Change log for QEMU releases.
├── check-qdict.c    Test for QDict (QEMU dictionary).
├── check-qfloat.c   Test for QFloat type.
├── check-qint.c     Test for QInt type.
├── check-qjson.c    Test for QJSON parsing.
├── check-qlist.c    Test for QList type.
├── check-qstring.c  Test for QString type.
├── cmd.c            Command line parsing utilities.
├── cmd.h            Headers for command utilities.
├── CODING_STYLE     QEMU coding style guidelines.
├── compatfd.c       Compatibility file descriptor handling.
├── compatfd.h       Headers for compatfd.
├── compiler.h       Compiler-specific macros.
├── config.h         Auto-generated configuration headers.
├── config.log       Configure script log.
├── configure        Build configuration script.
├── console.c        Console device emulation.
├── console.h        Headers for console.
├── COPYING          GPL license file.
├── COPYING.LIB      LGPL license file.
├── coroutine-gthread.c GLib-based coroutine backend.
├── coroutine-ucontext.c ucontext-based coroutine backend.
├── coroutine-win32.c Win32 fiber-based coroutine backend.
├── cpu-all.h        Common CPU definitions across architectures.
├── cpu-common.h     Shared CPU functions headers.
├── cpu-defs.h       CPU definition macros.
├── cpu-exec.c       CPU execution engine.
├── cpus.c           CPU subsystem management.
├── cpus.h           Headers for CPU management.
├── cris-dis.c       CRIS architecture disassembler.
├── cscope.out       Cscope database for source navigation.
├── cursor_hidden.xpm XPM image for hidden cursor.
├── cursor_left_ptr.xpm XPM image for left pointer cursor.
├── cursor.c         Cursor management for VNC/SPICE.
├── cutils.c         Core utilities implementation.
├── darwin-user      Directory for Darwin user-mode emulation.
├── def-helper.h     TCG helper function definitions.
├── default-configs  Directory for default configuration files.
├── device_tree.c    Device tree parsing and generation.
├── device_tree.h    Headers for device tree.
├── dis-asm.h        Generic disassembler headers.
├── disas.c          Disassembler library.
├── disas.h          Headers for disassembler.
├── dma-helpers.c    DMA operation helpers.
├── dma.h            Headers for DMA emulation.
├── docs             Directory for documentation.
├── dyngen-exec.h    Dynamic code generation headers.
├── elf.h            ELF file format headers.
├── envlist.c        Environment variable list handling.
├── envlist.h        Headers for envlist.
├── error_int.h      Internal error handling headers.
├── error.c          Error reporting framework.
├── error.h          Public error headers.
├── event_notifier.c Event notifier implementation.
├── event_notifier.h Headers for event notifiers.
├── exec-all.h       Execution engine headers.
├── exec-memory.h    Memory execution helpers.
├── exec.c           Main execution loop.
├── fpu              Directory for FPU emulation.
├── fsdev            Directory for filesystem devices.
├── gdb-xml          Directory for GDB XML descriptions.
├── gdbstub.c        GDB remote debugging stub.
├── gdbstub.h        Headers for GDB stub.
├── gen-icount.h     Instruction counting headers.
├── HACKING          Hacking guide for contributors.
├── hmp-commands.hx  Human Monitor Protocol commands definition.
├── hmp.c            Human monitor implementation.
├── hmp.h            Headers for HMP.
├── host-utils.c     Host-specific utility functions.
├── host-utils.h     Headers for host utils.
├── hppa-dis.c       HPPA architecture disassembler.
├── hppa.ld          Linker script for HPPA target.
├── hw               Directory for hardware emulation.
├── i386-dis.c       x86 disassembler.
├── i386.ld          Linker script for i386 target.
├── ia64-dis.c       IA64 architecture disassembler.
├── ia64.ld          Linker script for IA64 target.
├── input.c          Input device emulation.
├── int128.h         128-bit integer support headers.
├── iohandler.c      I/O handler management.
├── ioport-user.c    User-mode I/O port handling.
├── ioport.c         I/O port emulation.
├── ioport.h         Headers for I/O ports.
├── iorange.h        I/O range management headers.
├── iov.c            I/O vector utilities.
├── iov.h            Headers for I/O vectors.
├── json-lexer.c     JSON lexer implementation.
├── json-lexer.h     Headers for JSON lexer.
├── json-parser.c    JSON parser implementation.
├── json-parser.h    Headers for JSON parser.
├── json-streamer.c  JSON streaming utilities.
├── json-streamer.h  Headers for JSON streamer.
├── kvm-all.c        KVM acceleration support.
├── kvm-stub.c       KVM stub for non-KVM builds.
├── kvm.h            Headers for KVM.
├── libcacard        Directory for libcacard smartcard support.
├── libfdt_env.h     libfdt environment headers.
├── LICENSE          License file.
├── linux-aio.c      Linux AIO backend.
├── linux-headers    Directory for Linux headers.
├── linux-user       Directory for Linux user-mode emulation.
├── m68k-dis.c       m68k disassembler.
├── m68k-semi.c      m68k semihosting support.
├── m68k.ld          Linker script for m68k target.
├── main-loop.c      Main event loop.
├── main-loop.h      Headers for main loop.
├── MAINTAINERS      Maintainers list.
├── Makefile         Top-level build Makefile.
├── Makefile.dis     Makefile for disassemblers.
├── Makefile.hw      Makefile for hardware emulation.
├── Makefile.objs    Object file dependencies.
├── Makefile.target  Target-specific Makefile.
├── Makefile.user    User-mode Makefile.
├── memory.c         Guest memory management.
├── memory.h         Headers for memory management.
├── microblaze-dis.c Microblaze disassembler.
├── migration-exec.c Exec-based migration.
├── migration-fd.c   FD-based migration.
├── migration-tcp.c  TCP-based migration.
├── migration-unix.c Unix socket migration.
├── migration.c      Live migration framework.
├── migration.h      Headers for migration.
├── mips-dis.c       MIPS disassembler.
├── mips.ld          Linker script for MIPS target.
├── module.c         Dynamic module loading.
├── module.h         Headers for modules.
├── monitor.c        Monitor interface implementation.
├── monitor.h        Headers for monitor.
├── nbd.c            NBD (Network Block Device) server.
├── nbd.h            Headers for NBD.
├── net              Directory for networking.
├── net.c            Networking core.
├── net.h            Headers for networking.
├── NOTES.md         Release notes.
├── notify.c         Notification utilities.
├── notify.h         Headers for notifications.
├── os-posix.c       POSIX OS support.
├── os-win32.c       Win32 OS support.
├── osdep.c          OS-dependent functions.
├── osdep.h          Headers for osdep.
├── oslib-posix.c    POSIX OS library.
├── oslib-win32.c    Win32 OS library.
├── path.c           Path manipulation utilities.
├── pc-bios          Directory for PC BIOS images.
├── pci-ids.txt      PCI device ID list.
├── pflib.c          PF (Packet Filter) library for networking.
├── pflib.h          Headers for PF library.
├── poison.h         Poisoned pointers for debugging.
├── posix-aio-compat.c POSIX AIO compatibility layer.
├── ppc-dis.c        PowerPC disassembler.
├── ppc.ld           Linker script for PowerPC target.
├── ppc64.ld         Linker script for PowerPC64 target.
├── qapi             Directory for QAPI (QEMU API).
├── qapi-schema-guest.json Guest agent QAPI schema.
├── qapi-schema-test.json Test QAPI schema.
├── qapi-schema.json Main QAPI schema.
├── qbool.c          QBool type implementation.
├── qbool.h          Headers for QBool.
├── qdict-test-data.txt Test data for QDict.
├── qdict.c          QDict (dictionary) implementation.
├── qdict.h          Headers for QDict.
├── qemu_socket.h    Socket abstraction headers.
├── qemu-aio.h       AIO abstraction headers.
├── qemu-barrier.h   Barrier synchronization headers.
├── qemu-char.c      Character device backend.
├── qemu-char.h      Headers for character devices.
├── qemu-common.h    Common QEMU definitions.
├── qemu-config.c    Configuration parsing.
├── qemu-config.h    Headers for configuration.
├── qemu-coroutine-int.h Internal coroutine headers.
├── qemu-coroutine-lock.c Coroutine locking.
├── qemu-coroutine.c Coroutine implementation.
├── qemu-coroutine.h Public coroutine headers.
├── qemu-doc.texi    QEMU user documentation.
├── qemu-error.c     Error utilities.
├── qemu-error.h     Headers for errors.
├── qemu-ga.c        Guest agent main program.
├── qemu-img-cmds.hx QEMU-img command definitions.
├── qemu-img.c       Disk image utility.
├── qemu-img.texi    QEMU-img documentation.
├── qemu-io.c        Interactive disk I/O utility.
├── qemu-lock.h      Locking primitives headers.
├── qemu-log.h       Logging framework headers.
├── qemu-nbd.c       NBD server utility.
├── qemu-nbd.texi    QEMU-NBD documentation.
├── qemu-objects.h   QOM (QEMU Object Model) headers.
├── qemu-option.c    Option parsing.
├── qemu-option.h    Headers for options.
├── qemu-options.h   Option definitions.
├── qemu-options.hx  Option help text.
├── qemu-os-posix.h  POSIX OS headers.
├── qemu-os-win32.h  Win32 OS headers.
├── qemu-progress.c  Progress reporting.
├── qemu-queue.h     Queue utilities headers.
├── qemu-sockets.c   Socket utilities.
├── qemu-tech.texi   Technical documentation.
├── qemu-thread-posix.c POSIX threading.
├── qemu-thread-posix.h POSIX thread headers.
├── qemu-thread-win32.c Win32 threading.
├── qemu-thread-win32.h Win32 thread headers.
├── qemu-thread.h    Threading abstraction headers.
├── qemu-timer-common.c Common timer functions.
├── qemu-timer.c     Timer subsystem.
├── qemu-timer.h     Headers for timers.
├── qemu-tls.h       Thread-local storage headers.
├── qemu-tool.c      Tool utilities.
├── qemu-x509.h      X.509 certificate headers.
├── qemu-xattr.h     Extended attributes headers.
├── qemu.sasl        SASL authentication support.
├── qerror.c         QError string table.
├── qerror.h         Headers for QError.
├── qfloat.c         QFloat type implementation.
├── qfloat.h         Headers for QFloat.
├── qga              Directory for guest agent.
├── qint.c           QInt type implementation.
├── qint.h           Headers for QInt.
├── qjson.c          JSON serialization.
├── qjson.h          Headers for JSON.
├── qlist.c          QList implementation.
├── qlist.h          Headers for QList.
├── QMP              Directory for QMP (QEMU Machine Protocol).
├── qmp-commands.hx  QMP commands definition.
├── qmp.c            QMP implementation.
├── qobject.h        Base QObject headers.
├── qstring.c        QString implementation.
├── qstring.h        Headers for QString.
├── range.h          Range management headers.
├── readline.c       Readline interface.
├── readline.h       Headers for readline.
├── README           Project readme.
├── roms             Directory for ROM images.
├── rules.mak        Build rules.
├── s390-dis.c       S/390 disassembler.
├── s390.ld          Linker script for S/390 target.
├── savevm.c         VM state save/restore.
├── scripts          Directory for build scripts.
├── sh4-dis.c        SH4 disassembler.
├── slirp            Directory for user-mode networking (SLIRP).
├── softmmu_defs.h   SoftMMU definitions.
├── softmmu_exec.h   SoftMMU execution headers.
├── softmmu_header.h SoftMMU template header.
├── softmmu_template.h SoftMMU code templates.
├── softmmu-semi.h   SoftMMU semihosting headers.
├── sparc-dis.c      SPARC disassembler.
├── sparc.ld         Linker script for SPARC target.
├── sparc64.ld       Linker script for SPARC64 target.
├── spice-qemu-char.c SPICE character device backend.
├── sysconfigs       Directory for system config files.
├── sysemu.h         System emulation headers.
├── target-alpha     Directory for Alpha target.
├── target-arm       Directory for ARM target.
├── target-cris      Directory for CRIS target.
├── target-i386      Directory for x86 target.
├── target-lm32      Directory for LM32 target.
├── target-m68k      Directory for m68k target.
├── target-microblaze Directory for Microblaze target.
├── target-mips      Directory for MIPS target.
├── target-ppc       Directory for PowerPC target.
├── target-s390x     Directory for S/390x target.
├── target-sh4       Directory for SH4 target.
├── target-sparc     Directory for SPARC target.
├── target-unicore32 Directory for Unicore32 target.
├── target-xtensa    Directory for Xtensa target.
├── targphys.h       Target physical address headers.
├── tcg              Directory for Tiny Code Generator.
├── tcg-runtime.c    TCG runtime helpers.
├── tci-dis.c        TCI (Tiny Code Interpreter) disassembler.
├── tci.c            Tiny Code Interpreter implementation.
├── test-coroutine.c Coroutine tests.
├── test-qmp-commands.c QMP command tests.
├── test-visitor.c   QAPI visitor tests.
├── tests            Directory for unit tests.
├── thunk.c          Cross-endian thunking.
├── thunk.h          Headers for thunking.
├── TODO             Todo list.
├── trace            Directory for tracing support.
├── trace-events     Trace event definitions.
├── translate-all.c  Translation block management.
├── uboot_image.h    U-Boot image format headers.
├── ui               Directory for user interface (VNC, SDL, etc.).
├── usb-bsd.c        BSD USB host support.
├── usb-linux.c      Linux USB host support.
├── usb-redir.c      USB redirection.
├── usb-stub.c       USB stub for non-USB builds.
├── user-exec.c      User-mode execution.
├── VERSION          Version string.
├── version.rc       Windows version resource.
├── vgafont.h        VGA font data.
├── vl.c             VL (Virtual Layer) helpers.
├── x86_64.ld        Linker script for x86_64 target.
├── xen-all.c        Xen support.
├── xen-mapcache.c   Xen mapcache management.
├── xen-mapcache.h   Headers for Xen mapcache.
├── xen-stub.c       Xen stub for non-Xen builds.
└── xtensa-semi.c    Xtensa semihosting support.
