.
├── accel
│   ├── accel-blocker.c
│   ├── accel-common.c
│   ├── accel-internal.h
│   ├── accel-system.c
│   ├── accel-target.c
│   ├── accel-user.c
│   ├── dummy-cpus.c
│   ├── hvf
│   │   ├── entitlements.plist
│   │   ├── hvf-accel-ops.c
│   │   ├── hvf-all.c
│   │   └── meson.build
│   ├── Kconfig
│   ├── kvm
│   │   ├── kvm-accel-ops.c
│   │   ├── kvm-all.c
│   │   ├── kvm-cpus.h
│   │   ├── meson.build
│   │   ├── trace-events
│   │   └── trace.h
│   ├── meson.build
│   ├── qtest
│   │   ├── meson.build
│   │   └── qtest.c
│   ├── stubs
│   │   ├── hvf-stub.c
│   │   ├── kvm-stub.c
│   │   ├── meson.build
│   │   ├── tcg-stub.c
│   │   └── xen-stub.c
│   ├── tcg
│   │   ├── atomic_common.c.inc
│   │   ├── atomic_template.h
│   │   ├── backend-ldst.h
│   │   ├── cpu-exec-common.c
│   │   ├── cpu-exec.c
│   │   ├── cputlb.c
│   │   ├── icount-common.c
│   │   ├── internal-common.h
│   │   ├── ldst_atomicity.c.inc
│   │   ├── ldst_common.c.inc
│   │   ├── meson.build
│   │   ├── monitor.c
│   │   ├── plugin-gen.c
│   │   ├── tb-context.h
│   │   ├── tb-hash.h
│   │   ├── tb-internal.h
│   │   ├── tb-jmp-cache.h
│   │   ├── tb-maint.c
│   │   ├── tcg-accel-ops-icount.c
│   │   ├── tcg-accel-ops-icount.h
│   │   ├── tcg-accel-ops-mttcg.c
│   │   ├── tcg-accel-ops-mttcg.h
│   │   ├── tcg-accel-ops-rr.c
│   │   ├── tcg-accel-ops-rr.h
│   │   ├── tcg-accel-ops.c
│   │   ├── tcg-accel-ops.h
│   │   ├── tcg-all.c
│   │   ├── tcg-runtime-gvec.c
│   │   ├── tcg-runtime.c
│   │   ├── tcg-runtime.h
│   │   ├── tlb-bounds.h
│   │   ├── trace-events
│   │   ├── trace.h
│   │   ├── translate-all.c
│   │   ├── translator.c
│   │   ├── user-exec-stub.c
│   │   ├── user-exec.c
│   │   ├── vcpu-state.h
│   │   └── watchpoint.c
│   └── xen
│       ├── meson.build
│       └── xen-all.c
├── audio
│   ├── alsaaudio.c
│   ├── audio_int.h
│   ├── audio_template.h
│   ├── audio_win_int.c
│   ├── audio_win_int.h
│   ├── audio-hmp-cmds.c
│   ├── audio.c
│   ├── audio.h
│   ├── coreaudio.m
│   ├── dbusaudio.c
│   ├── dsound_template.h
│   ├── dsoundaudio.c
│   ├── jackaudio.c
│   ├── meson.build
│   ├── mixeng_template.h
│   ├── mixeng.c
│   ├── mixeng.h
│   ├── noaudio.c
│   ├── ossaudio.c
│   ├── paaudio.c
│   ├── pwaudio.c
│   ├── rate_template.h
│   ├── sdlaudio.c
│   ├── sndioaudio.c
│   ├── spiceaudio.c
│   ├── trace-events
│   ├── trace.h
│   ├── wavaudio.c
│   └── wavcapture.c
├── authz
│   ├── base.c
│   ├── list.c
│   ├── listfile.c
│   ├── meson.build
│   ├── pamacct.c
│   ├── simple.c
│   ├── trace-events
│   └── trace.h
├── backends
│   ├── confidential-guest-support.c
│   ├── cryptodev-builtin.c
│   ├── cryptodev-hmp-cmds.c
│   ├── cryptodev-lkcf.c
│   ├── cryptodev-vhost-user.c
│   ├── cryptodev-vhost.c
│   ├── cryptodev.c
│   ├── dbus-vmstate.c
│   ├── dbus-vmstate1.xml
│   ├── host_iommu_device.c
│   ├── hostmem-epc.c
│   ├── hostmem-file.c
│   ├── hostmem-memfd.c
│   ├── hostmem-ram.c
│   ├── hostmem-shm.c
│   ├── hostmem.c
│   ├── iommufd.c
│   ├── Kconfig
│   ├── meson.build
│   ├── rng-builtin.c
│   ├── rng-egd.c
│   ├── rng-random.c
│   ├── rng.c
│   ├── spdm-socket.c
│   ├── tpm
│   │   ├── Kconfig
│   │   ├── meson.build
│   │   ├── tpm_backend.c
│   │   ├── tpm_emulator.c
│   │   ├── tpm_int.h
│   │   ├── tpm_ioctl.h
│   │   ├── tpm_passthrough.c
│   │   ├── tpm_util.c
│   │   ├── trace-events
│   │   └── trace.h
│   ├── trace-events
│   ├── trace.h
│   └── vhost-user.c
├── block
│   ├── accounting.c
│   ├── aio_task.c
│   ├── amend.c
│   ├── backup.c
│   ├── blkdebug.c
│   ├── blkio.c
│   ├── blklogwrites.c
│   ├── blkreplay.c
│   ├── blkverify.c
│   ├── block-backend.c
│   ├── block-copy.c
│   ├── block-gen.h
│   ├── block-ram-registrar.c
│   ├── bochs.c
│   ├── cloop.c
│   ├── commit.c
│   ├── copy-before-write.c
│   ├── copy-before-write.h
│   ├── copy-on-read.c
│   ├── copy-on-read.h
│   ├── coroutines.h
│   ├── create.c
│   ├── crypto.c
│   ├── crypto.h
│   ├── curl.c
│   ├── dirty-bitmap.c
│   ├── dmg-bz2.c
│   ├── dmg-lzfse.c
│   ├── dmg.c
│   ├── dmg.h
│   ├── export
│   │   ├── export.c
│   │   ├── fuse.c
│   │   ├── meson.build
│   │   ├── vduse-blk.c
│   │   ├── vduse-blk.h
│   │   ├── vhost-user-blk-server.c
│   │   ├── vhost-user-blk-server.h
│   │   ├── virtio-blk-handler.c
│   │   └── virtio-blk-handler.h
│   ├── file-posix.c
│   ├── file-win32.c
│   ├── filter-compress.c
│   ├── gluster.c
│   ├── graph-lock.c
│   ├── io_uring.c
│   ├── io.c
│   ├── iscsi-opts.c
│   ├── iscsi.c
│   ├── linux-aio.c
│   ├── meson.build
│   ├── mirror.c
│   ├── monitor
│   │   ├── bitmap-qmp-cmds.c
│   │   ├── block-hmp-cmds.c
│   │   └── meson.build
│   ├── nbd.c
│   ├── nfs.c
│   ├── null.c
│   ├── nvme.c
│   ├── parallels-ext.c
│   ├── parallels.c
│   ├── parallels.h
│   ├── preallocate.c
│   ├── progress_meter.c
│   ├── qapi-system.c
│   ├── qapi.c
│   ├── qcow.c
│   ├── qcow2-bitmap.c
│   ├── qcow2-cache.c
│   ├── qcow2-cluster.c
│   ├── qcow2-refcount.c
│   ├── qcow2-snapshot.c
│   ├── qcow2-threads.c
│   ├── qcow2.c
│   ├── qcow2.h
│   ├── qed-check.c
│   ├── qed-cluster.c
│   ├── qed-l2-cache.c
│   ├── qed-table.c
│   ├── qed.c
│   ├── qed.h
│   ├── quorum.c
│   ├── raw-format.c
│   ├── rbd.c
│   ├── replication.c
│   ├── reqlist.c
│   ├── snapshot-access.c
│   ├── snapshot.c
│   ├── ssh.c
│   ├── stream.c
│   ├── throttle-groups.c
│   ├── throttle.c
│   ├── trace-events
│   ├── trace.h
│   ├── vdi.c
│   ├── vhdx-endian.c
│   ├── vhdx-log.c
│   ├── vhdx.c
│   ├── vhdx.h
│   ├── vmdk.c
│   ├── vpc.c
│   ├── vvfat.c
│   ├── win32-aio.c
│   └── write-threshold.c
├── block.c
├── blockdev-nbd.c
├── blockdev.c
├── blockjob.c
├── bsd-user
│   ├── aarch64
│   │   ├── signal.c
│   │   ├── target_arch_cpu.c
│   │   ├── target_arch_cpu.h
│   │   ├── target_arch_elf.h
│   │   ├── target_arch_reg.h
│   │   ├── target_arch_signal.h
│   │   ├── target_arch_sigtramp.h
│   │   ├── target_arch_sysarch.h
│   │   ├── target_arch_thread.h
│   │   ├── target_arch_vmparam.h
│   │   ├── target_arch.h
│   │   ├── target_syscall.h
│   │   └── target.h
│   ├── arm
│   │   ├── signal.c
│   │   ├── target_arch_cpu.c
│   │   ├── target_arch_cpu.h
│   │   ├── target_arch_elf.h
│   │   ├── target_arch_reg.h
│   │   ├── target_arch_signal.h
│   │   ├── target_arch_sigtramp.h
│   │   ├── target_arch_sysarch.h
│   │   ├── target_arch_thread.h
│   │   ├── target_arch_vmparam.h
│   │   ├── target_arch.h
│   │   ├── target_syscall.h
│   │   └── target.h
│   ├── bsd-file.h
│   ├── bsd-mem.c
│   ├── bsd-mem.h
│   ├── bsd-proc.c
│   ├── bsd-proc.h
│   ├── bsdload.c
│   ├── elfcore.c
│   ├── elfload.c
│   ├── errno_defs.h
│   ├── freebsd
│   │   ├── host-os.h
│   │   ├── meson.build
│   │   ├── os-misc.h
│   │   ├── os-proc.c
│   │   ├── os-proc.h
│   │   ├── os-stat.c
│   │   ├── os-stat.h
│   │   ├── os-strace.h
│   │   ├── os-sys.c
│   │   ├── os-syscall.c
│   │   ├── qemu-os.h
│   │   ├── strace.list
│   │   ├── syscall_nr.h
│   │   ├── target_os_elf.h
│   │   ├── target_os_siginfo.h
│   │   ├── target_os_signal.h
│   │   ├── target_os_stack.h
│   │   ├── target_os_thread.h
│   │   ├── target_os_ucontext.h
│   │   ├── target_os_user.h
│   │   └── target_os_vmparam.h
│   ├── host
│   │   ├── arm
│   │   │   └── host-signal.h
│   │   ├── i386
│   │   │   └── host-signal.h
│   │   └── x86_64
│   │       └── host-signal.h
│   ├── i386
│   │   ├── signal.c
│   │   ├── target_arch_cpu.c
│   │   ├── target_arch_cpu.h
│   │   ├── target_arch_elf.h
│   │   ├── target_arch_reg.h
│   │   ├── target_arch_signal.h
│   │   ├── target_arch_sigtramp.h
│   │   ├── target_arch_sysarch.h
│   │   ├── target_arch_thread.h
│   │   ├── target_arch_vmparam.h
│   │   ├── target_arch.h
│   │   ├── target_syscall.h
│   │   └── target.h
│   ├── include
│   │   └── special-errno.h
│   ├── main.c
│   ├── meson.build
│   ├── mmap.c
│   ├── netbsd
│   │   ├── host-os.h
│   │   ├── os-strace.h
│   │   ├── strace.list
│   │   ├── syscall_nr.h
│   │   ├── target_os_elf.h
│   │   ├── target_os_siginfo.h
│   │   ├── target_os_signal.h
│   │   ├── target_os_stack.h
│   │   └── target_os_thread.h
│   ├── openbsd
│   │   ├── host-os.h
│   │   ├── os-strace.h
│   │   ├── strace.list
│   │   ├── syscall_nr.h
│   │   ├── target_os_elf.h
│   │   ├── target_os_siginfo.h
│   │   ├── target_os_signal.h
│   │   ├── target_os_stack.h
│   │   └── target_os_thread.h
│   ├── plugin-api.c
│   ├── qemu-bsd.h
│   ├── qemu.h
│   ├── riscv
│   │   ├── signal.c
│   │   ├── target_arch_cpu.c
│   │   ├── target_arch_cpu.h
│   │   ├── target_arch_elf.h
│   │   ├── target_arch_reg.h
│   │   ├── target_arch_signal.h
│   │   ├── target_arch_sigtramp.h
│   │   ├── target_arch_sysarch.h
│   │   ├── target_arch_thread.h
│   │   ├── target_arch_vmparam.h
│   │   ├── target_arch.h
│   │   ├── target_syscall.h
│   │   └── target.h
│   ├── signal-common.h
│   ├── signal.c
│   ├── strace.c
│   ├── syscall_defs.h
│   ├── trace-events
│   ├── trace.h
│   ├── uaccess.c
│   └── x86_64
│       ├── signal.c
│       ├── target_arch_cpu.c
│       ├── target_arch_cpu.h
│       ├── target_arch_elf.h
│       ├── target_arch_reg.h
│       ├── target_arch_signal.h
│       ├── target_arch_sigtramp.h
│       ├── target_arch_sysarch.h
│       ├── target_arch_thread.h
│       ├── target_arch_vmparam.h
│       ├── target_arch.h
│       ├── target_syscall.h
│       └── target.h
├── chardev
│   ├── baum.c
│   ├── char-console.c
│   ├── char-fd.c
│   ├── char-fe.c
│   ├── char-file.c
│   ├── char-hmp-cmds.c
│   ├── char-hub.c
│   ├── char-io.c
│   ├── char-mux.c
│   ├── char-null.c
│   ├── char-parallel.c
│   ├── char-pipe.c
│   ├── char-pty.c
│   ├── char-ringbuf.c
│   ├── char-serial.c
│   ├── char-socket.c
│   ├── char-stdio.c
│   ├── char-udp.c
│   ├── char-win-stdio.c
│   ├── char-win.c
│   ├── char.c
│   ├── chardev-internal.h
│   ├── meson.build
│   ├── msmouse.c
│   ├── spice.c
│   ├── testdev.c
│   ├── trace-events
│   ├── trace.h
│   └── wctablet.c
├── clippy.toml
├── common-user
│   ├── host
│   │   ├── aarch64
│   │   │   └── safe-syscall.inc.S
│   │   ├── arm
│   │   │   └── safe-syscall.inc.S
│   │   ├── i386
│   │   │   └── safe-syscall.inc.S
│   │   ├── loongarch64
│   │   │   └── safe-syscall.inc.S
│   │   ├── mips
│   │   │   └── safe-syscall.inc.S
│   │   ├── ppc
│   │   │   └── safe-syscall.inc.S
│   │   ├── ppc64
│   │   │   └── safe-syscall.inc.S
│   │   ├── riscv
│   │   │   └── safe-syscall.inc.S
│   │   ├── s390x
│   │   │   └── safe-syscall.inc.S
│   │   ├── sparc64
│   │   │   └── safe-syscall.inc.S
│   │   └── x86_64
│   │       └── safe-syscall.inc.S
│   ├── meson.build
│   ├── plugin-api.c.inc
│   ├── safe-syscall-error.c
│   └── safe-syscall.S
├── configs
│   ├── devices
│   │   ├── aarch64-softmmu
│   │   │   ├── default.mak
│   │   │   └── minimal.mak
│   │   ├── alpha-softmmu
│   │   │   └── default.mak
│   │   ├── arm-softmmu
│   │   │   └── default.mak
│   │   ├── avr-softmmu
│   │   │   └── default.mak
│   │   ├── hppa-softmmu
│   │   │   └── default.mak
│   │   ├── i386-softmmu
│   │   │   └── default.mak
│   │   ├── loongarch64-softmmu
│   │   │   └── default.mak
│   │   ├── m68k-softmmu
│   │   │   └── default.mak
│   │   ├── microblaze-softmmu
│   │   │   └── default.mak
│   │   ├── microblazeel-softmmu
│   │   │   └── default.mak
│   │   ├── mips-softmmu
│   │   │   ├── common.mak
│   │   │   └── default.mak
│   │   ├── mips64-softmmu
│   │   │   └── default.mak
│   │   ├── mips64el-softmmu
│   │   │   └── default.mak
│   │   ├── mipsel-softmmu
│   │   │   └── default.mak
│   │   ├── or1k-softmmu
│   │   │   └── default.mak
│   │   ├── ppc-softmmu
│   │   │   └── default.mak
│   │   ├── ppc64-softmmu
│   │   │   └── default.mak
│   │   ├── riscv32-softmmu
│   │   │   └── default.mak
│   │   ├── riscv64-softmmu
│   │   │   └── default.mak
│   │   ├── rx-softmmu
│   │   │   └── default.mak
│   │   ├── s390x-softmmu
│   │   │   └── default.mak
│   │   ├── sh4-softmmu
│   │   │   └── default.mak
│   │   ├── sh4eb-softmmu
│   │   │   └── default.mak
│   │   ├── sparc-softmmu
│   │   │   └── default.mak
│   │   ├── sparc64-softmmu
│   │   │   └── default.mak
│   │   ├── tricore-softmmu
│   │   │   └── default.mak
│   │   ├── x86_64-softmmu
│   │   │   └── default.mak
│   │   ├── xtensa-softmmu
│   │   │   └── default.mak
│   │   └── xtensaeb-softmmu
│   │       └── default.mak
│   ├── meson
│   │   ├── emscripten.txt
│   │   └── windows.txt
│   └── targets
│       ├── aarch64_be-linux-user.mak
│       ├── aarch64-bsd-user.mak
│       ├── aarch64-linux-user.mak
│       ├── aarch64-softmmu.mak
│       ├── alpha-linux-user.mak
│       ├── alpha-softmmu.mak
│       ├── arm-bsd-user.mak
│       ├── arm-linux-user.mak
│       ├── arm-softmmu.mak
│       ├── armeb-linux-user.mak
│       ├── avr-softmmu.mak
│       ├── hexagon-linux-user.mak
│       ├── hppa-linux-user.mak
│       ├── hppa-softmmu.mak
│       ├── i386-bsd-user.mak
│       ├── i386-linux-user.mak
│       ├── i386-softmmu.mak
│       ├── loongarch64-linux-user.mak
│       ├── loongarch64-softmmu.mak
│       ├── m68k-linux-user.mak
│       ├── m68k-softmmu.mak
│       ├── microblaze-linux-user.mak
│       ├── microblaze-softmmu.mak
│       ├── microblazeel-linux-user.mak
│       ├── microblazeel-softmmu.mak
│       ├── mips-linux-user.mak
│       ├── mips-softmmu.mak
│       ├── mips64-linux-user.mak
│       ├── mips64-softmmu.mak
│       ├── mips64el-linux-user.mak
│       ├── mips64el-softmmu.mak
│       ├── mipsel-linux-user.mak
│       ├── mipsel-softmmu.mak
│       ├── mipsn32-linux-user.mak
│       ├── mipsn32el-linux-user.mak
│       ├── or1k-linux-user.mak
│       ├── or1k-softmmu.mak
│       ├── ppc-linux-user.mak
│       ├── ppc-softmmu.mak
│       ├── ppc64-linux-user.mak
│       ├── ppc64-softmmu.mak
│       ├── ppc64le-linux-user.mak
│       ├── riscv32-linux-user.mak
│       ├── riscv32-softmmu.mak
│       ├── riscv64-bsd-user.mak
│       ├── riscv64-linux-user.mak
│       ├── riscv64-softmmu.mak
│       ├── rx-softmmu.mak
│       ├── s390x-linux-user.mak
│       ├── s390x-softmmu.mak
│       ├── sh4-linux-user.mak
│       ├── sh4-softmmu.mak
│       ├── sh4eb-linux-user.mak
│       ├── sh4eb-softmmu.mak
│       ├── sparc-linux-user.mak
│       ├── sparc-softmmu.mak
│       ├── sparc32plus-linux-user.mak
│       ├── sparc64-linux-user.mak
│       ├── sparc64-softmmu.mak
│       ├── tricore-softmmu.mak
│       ├── x86_64-bsd-user.mak
│       ├── x86_64-linux-user.mak
│       ├── x86_64-softmmu.mak
│       ├── xtensa-linux-user.mak
│       ├── xtensa-softmmu.mak
│       ├── xtensaeb-linux-user.mak
│       └── xtensaeb-softmmu.mak
├── configure
├── contrib
│   ├── elf2dmp
│   │   ├── addrspace.c
│   │   ├── addrspace.h
│   │   ├── download.c
│   │   ├── download.h
│   │   ├── err.h
│   │   ├── kdbg.h
│   │   ├── main.c
│   │   ├── meson.build
│   │   ├── pdb.c
│   │   ├── pdb.h
│   │   ├── pe.h
│   │   ├── qemu_elf.c
│   │   └── qemu_elf.h
│   ├── gitdm
│   │   ├── aliases
│   │   ├── domain-map
│   │   ├── filetypes.txt
│   │   ├── group-map-academics
│   │   ├── group-map-alibaba
│   │   ├── group-map-amd
│   │   ├── group-map-cadence
│   │   ├── group-map-codeweavers
│   │   ├── group-map-facebook
│   │   ├── group-map-ibm
│   │   ├── group-map-individuals
│   │   ├── group-map-interns
│   │   ├── group-map-janustech
│   │   ├── group-map-netflix
│   │   ├── group-map-redhat
│   │   ├── group-map-robots
│   │   └── group-map-wavecomp
│   ├── ivshmem-client
│   │   ├── ivshmem-client.c
│   │   ├── ivshmem-client.h
│   │   ├── main.c
│   │   └── meson.build
│   ├── ivshmem-server
│   │   ├── ivshmem-server.c
│   │   ├── ivshmem-server.h
│   │   ├── main.c
│   │   └── meson.build
│   ├── plugins
│   │   ├── bbv.c
│   │   ├── cache.c
│   │   ├── cflow.c
│   │   ├── drcov.c
│   │   ├── execlog.c
│   │   ├── hotblocks.c
│   │   ├── hotpages.c
│   │   ├── howvec.c
│   │   ├── hwprofile.c
│   │   ├── ips.c
│   │   ├── lockstep.c
│   │   ├── meson.build
│   │   ├── stoptrigger.c
│   │   └── win32_linker.c
│   ├── systemd
│   │   ├── qemu-guest-agent.service
│   │   ├── qemu-pr-helper.service
│   │   ├── qemu-pr-helper.socket
│   │   ├── qemu-vmsr-helper.service
│   │   └── qemu-vmsr-helper.socket
│   ├── vhost-user-blk
│   │   ├── meson.build
│   │   └── vhost-user-blk.c
│   ├── vhost-user-gpu
│   │   ├── 50-qemu-gpu.json.in
│   │   ├── meson.build
│   │   ├── vhost-user-gpu.c
│   │   ├── virgl.c
│   │   ├── virgl.h
│   │   ├── vugbm.c
│   │   ├── vugbm.h
│   │   └── vugpu.h
│   ├── vhost-user-input
│   │   ├── main.c
│   │   └── meson.build
│   ├── vhost-user-scsi
│   │   ├── meson.build
│   │   └── vhost-user-scsi.c
│   └── vmapple
│       └── uuid.sh
├── COPYING
├── COPYING.LIB
├── cpu-common.c
├── cpu-target.c
├── crypto
│   ├── aes.c
│   ├── afalg.c
│   ├── afalgpriv.h
│   ├── afsplit.c
│   ├── akcipher-gcrypt.c.inc
│   ├── akcipher-nettle.c.inc
│   ├── akcipher.c
│   ├── akcipherpriv.h
│   ├── block-luks-priv.h
│   ├── block-luks.c
│   ├── block-luks.h
│   ├── block-qcow.c
│   ├── block-qcow.h
│   ├── block.c
│   ├── blockpriv.h
│   ├── cipher-afalg.c
│   ├── cipher-gcrypt.c.inc
│   ├── cipher-gnutls.c.inc
│   ├── cipher-nettle.c.inc
│   ├── cipher-stub.c.inc
│   ├── cipher.c
│   ├── cipherpriv.h
│   ├── clmul.c
│   ├── der.c
│   ├── der.h
│   ├── hash-afalg.c
│   ├── hash-gcrypt.c
│   ├── hash-glib.c
│   ├── hash-gnutls.c
│   ├── hash-nettle.c
│   ├── hash.c
│   ├── hashpriv.h
│   ├── hmac-gcrypt.c
│   ├── hmac-glib.c
│   ├── hmac-gnutls.c
│   ├── hmac-nettle.c
│   ├── hmac.c
│   ├── hmacpriv.h
│   ├── init.c
│   ├── ivgen-essiv.c
│   ├── ivgen-essiv.h
│   ├── ivgen-plain.c
│   ├── ivgen-plain.h
│   ├── ivgen-plain64.c
│   ├── ivgen-plain64.h
│   ├── ivgen.c
│   ├── ivgenpriv.h
│   ├── meson.build
│   ├── pbkdf-gcrypt.c
│   ├── pbkdf-gnutls.c
│   ├── pbkdf-nettle.c
│   ├── pbkdf-stub.c
│   ├── pbkdf.c
│   ├── random-gcrypt.c
│   ├── random-gnutls.c
│   ├── random-none.c
│   ├── random-platform.c
│   ├── rsakey-builtin.c.inc
│   ├── rsakey-nettle.c.inc
│   ├── rsakey.c
│   ├── rsakey.h
│   ├── secret_common.c
│   ├── secret_keyring.c
│   ├── secret.c
│   ├── sm4.c
│   ├── tls-cipher-suites.c
│   ├── tlscreds.c
│   ├── tlscredsanon.c
│   ├── tlscredspriv.h
│   ├── tlscredspsk.c
│   ├── tlscredsx509.c
│   ├── tlssession.c
│   ├── trace-events
│   ├── trace.h
│   ├── x509-utils.c
│   └── xts.c
├── cscope.out
├── disas
│   ├── alpha.c
│   ├── capstone.c
│   ├── disas-common.c
│   ├── disas-host.c
│   ├── disas-internal.h
│   ├── disas-mon.c
│   ├── disas-target.c
│   ├── hexagon.c
│   ├── hppa.c
│   ├── m68k.c
│   ├── meson.build
│   ├── microblaze.c
│   ├── mips.c
│   ├── nanomips.c
│   ├── objdump.c
│   ├── riscv-xthead.c
│   ├── riscv-xthead.h
│   ├── riscv-xventana.c
│   ├── riscv-xventana.h
│   ├── riscv.c
│   ├── riscv.h
│   ├── sh4.c
│   ├── sparc.c
│   └── xtensa.c
├── docs
│   ├── _templates
│   │   └── footer.html
│   ├── about
│   │   ├── build-platforms.rst
│   │   ├── deprecated.rst
│   │   ├── emulation.rst
│   │   ├── index.rst
│   │   ├── license.rst
│   │   └── removed-features.rst
│   ├── block-replication.txt
│   ├── bypass-iommu.txt
│   ├── COLO-FT.txt
│   ├── colo-proxy.txt
│   ├── conf.py
│   ├── config
│   │   ├── ich9-ehci-uhci.cfg
│   │   ├── mach-virt-graphical.cfg
│   │   ├── mach-virt-serial.cfg
│   │   ├── q35-emulated.cfg
│   │   ├── q35-virtio-graphical.cfg
│   │   └── q35-virtio-serial.cfg
│   ├── defs.rst.inc
│   ├── devel
│   │   ├── atomics.rst
│   │   ├── bitops.rst
│   │   ├── block-coroutine-wrapper.rst
│   │   ├── build-environment.rst
│   │   ├── build-system.rst
│   │   ├── clocks.rst
│   │   ├── code-of-conduct.rst
│   │   ├── code-provenance.rst
│   │   ├── codebase.rst
│   │   ├── conflict-resolution.rst
│   │   ├── control-flow-integrity.rst
│   │   ├── crypto.rst
│   │   ├── decodetree.rst
│   │   ├── docs.rst
│   │   ├── ebpf_rss.rst
│   │   ├── index-api.rst
│   │   ├── index-build.rst
│   │   ├── index-internals.rst
│   │   ├── index-process.rst
│   │   ├── index-tcg.rst
│   │   ├── index.rst
│   │   ├── kconfig.rst
│   │   ├── loads-stores.rst
│   │   ├── lockcnt.rst
│   │   ├── luks-detached-header.rst
│   │   ├── maintainers.rst
│   │   ├── memory.rst
│   │   ├── migration
│   │   │   ├── best-practices.rst
│   │   │   ├── compatibility.rst
│   │   │   ├── CPR.rst
│   │   │   ├── dirty-limit.rst
│   │   │   ├── features.rst
│   │   │   ├── index.rst
│   │   │   ├── main.rst
│   │   │   ├── mapped-ram.rst
│   │   │   ├── postcopy.rst
│   │   │   ├── qatzip-compression.rst
│   │   │   ├── qpl-compression.rst
│   │   │   ├── uadk-compression.rst
│   │   │   ├── vfio.rst
│   │   │   └── virtio.rst
│   │   ├── modules.rst
│   │   ├── multi-process.rst
│   │   ├── multi-thread-tcg.rst
│   │   ├── multiple-iothreads.rst
│   │   ├── pci.rst
│   │   ├── qapi-code-gen.rst
│   │   ├── qapi-domain.rst
│   │   ├── qdev-api.rst
│   │   ├── qom-api.rst
│   │   ├── qom.rst
│   │   ├── rcu.rst
│   │   ├── replay.rst
│   │   ├── reset.rst
│   │   ├── rust.rst
│   │   ├── s390-cpu-topology.rst
│   │   ├── s390-dasd-ipl.rst
│   │   ├── secure-coding-practices.rst
│   │   ├── stable-process.rst
│   │   ├── style.rst
│   │   ├── submitting-a-patch.rst
│   │   ├── submitting-a-pull-request.rst
│   │   ├── tcg-icount.rst
│   │   ├── tcg-ops.rst
│   │   ├── tcg-plugins.rst
│   │   ├── tcg.rst
│   │   ├── testing
│   │   │   ├── acpi-bits.rst
│   │   │   ├── blkdebug.rst
│   │   │   ├── blkverify.rst
│   │   │   ├── ci-jobs.rst.inc
│   │   │   ├── ci-runners.rst.inc
│   │   │   ├── ci.rst
│   │   │   ├── functional.rst
│   │   │   ├── fuzzing.rst
│   │   │   ├── index.rst
│   │   │   ├── main.rst
│   │   │   ├── qgraph.rst
│   │   │   └── qtest.rst
│   │   ├── tracing.rst
│   │   ├── trivial-patches.rst
│   │   ├── uefi-vars.rst
│   │   ├── ui.rst
│   │   ├── vfio-iommufd.rst
│   │   ├── virtio-backends.rst
│   │   ├── writing-monitor-commands.rst
│   │   └── zoned-storage.rst
│   ├── glossary.rst
│   ├── igd-assign.txt
│   ├── image-fuzzer.txt
│   ├── index.rst
│   ├── interop
│   │   ├── barrier.rst
│   │   ├── bitmaps.rst
│   │   ├── dbus-display.rst
│   │   ├── dbus-vmstate.rst
│   │   ├── dbus.rst
│   │   ├── firmware.json
│   │   ├── index.rst
│   │   ├── live-block-operations.rst
│   │   ├── nbd.rst
│   │   ├── parallels.rst
│   │   ├── pr-helper.rst
│   │   ├── prl-xml.rst
│   │   ├── qcow2.rst
│   │   ├── qed_spec.rst
│   │   ├── qemu-ga-ref.rst
│   │   ├── qemu-ga.rst
│   │   ├── qemu-qmp-ref.rst
│   │   ├── qemu-storage-daemon-qmp-ref.rst
│   │   ├── qmp-spec.rst
│   │   ├── vhost-user-gpu.rst
│   │   ├── vhost-user.json
│   │   ├── vhost-user.rst
│   │   ├── vhost-vdpa.rst
│   │   ├── virtio-balloon-stats.rst
│   │   └── vnc-ledstate-pseudo-encoding.rst
│   ├── memory-hotplug.txt
│   ├── meson.build
│   ├── multi-thread-compression.txt
│   ├── multiseat.txt
│   ├── nvdimm.txt
│   ├── pci_expander_bridge.txt
│   ├── pcie_pci_bridge.txt
│   ├── pcie_sriov.txt
│   ├── pcie.txt
│   ├── qcow2-cache.txt
│   ├── qdev-device-use.txt
│   ├── qemu-option-trace.rst.inc
│   ├── qemupciserial.inf
│   ├── rdma.txt
│   ├── requirements.txt
│   ├── specs
│   │   ├── acpi_cpu_hotplug.rst
│   │   ├── acpi_erst.rst
│   │   ├── acpi_hest_ghes.rst
│   │   ├── acpi_hw_reduced_hotplug.rst
│   │   ├── acpi_mem_hotplug.rst
│   │   ├── acpi_nvdimm.rst
│   │   ├── acpi_pci_hotplug.rst
│   │   ├── aspeed-intc.rst
│   │   ├── edu.rst
│   │   ├── fsi.rst
│   │   ├── fw_cfg.rst
│   │   ├── index.rst
│   │   ├── ivshmem-spec.rst
│   │   ├── pci-ids.rst
│   │   ├── pci-serial.rst
│   │   ├── pci-testdev.rst
│   │   ├── ppc-spapr-hcalls.rst
│   │   ├── ppc-spapr-hotplug.rst
│   │   ├── ppc-spapr-numa.rst
│   │   ├── ppc-spapr-uv-hcalls.rst
│   │   ├── ppc-spapr-xive.rst
│   │   ├── ppc-xive.rst
│   │   ├── pvpanic.rst
│   │   ├── rapl-msr.rst
│   │   ├── riscv-aia.rst
│   │   ├── riscv-iommu.rst
│   │   ├── rocker.rst
│   │   ├── sev-guest-firmware.rst
│   │   ├── spdm.rst
│   │   ├── standard-vga.rst
│   │   ├── tpm.rst
│   │   ├── virt-ctlr.rst
│   │   ├── vmcoreinfo.rst
│   │   ├── vmgenid.rst
│   │   └── vmw_pvscsi-spec.rst
│   ├── sphinx
│   │   ├── compat.py
│   │   ├── dbusdoc.py
│   │   ├── dbusdomain.py
│   │   ├── dbusparser.py
│   │   ├── depfile.py
│   │   ├── fakedbusdoc.py
│   │   ├── hxtool.py
│   │   ├── kerneldoc.py
│   │   ├── qapi_domain.py
│   │   ├── qapidoc_legacy.py
│   │   ├── qapidoc.py
│   │   └── qmp_lexer.py
│   ├── sphinx-static
│   │   ├── custom.js
│   │   └── theme_overrides.css
│   ├── spice-port-fqdn.txt
│   ├── spin
│   │   ├── aio_notify_accept.promela
│   │   ├── aio_notify_bug.promela
│   │   ├── aio_notify.promela
│   │   ├── tcg-exclusive.promela
│   │   └── win32-qemu-event.promela
│   ├── system
│   │   ├── arm
│   │   │   ├── aspeed.rst
│   │   │   ├── b-l475e-iot01a.rst
│   │   │   ├── bananapi_m2u.rst
│   │   │   ├── collie.rst
│   │   │   ├── cpu-features.rst
│   │   │   ├── cubieboard.rst
│   │   │   ├── digic.rst
│   │   │   ├── emcraft-sf2.rst
│   │   │   ├── emulation.rst
│   │   │   ├── exynos.rst
│   │   │   ├── fby35.rst
│   │   │   ├── highbank.rst
│   │   │   ├── imx25-pdk.rst
│   │   │   ├── imx8mp-evk.rst
│   │   │   ├── integratorcp.rst
│   │   │   ├── kzm.rst
│   │   │   ├── mcimx6ul-evk.rst
│   │   │   ├── mcimx7d-sabre.rst
│   │   │   ├── mps2.rst
│   │   │   ├── musca.rst
│   │   │   ├── musicpal.rst
│   │   │   ├── nrf.rst
│   │   │   ├── nuvoton.rst
│   │   │   ├── orangepi.rst
│   │   │   ├── raspi.rst
│   │   │   ├── realview.rst
│   │   │   ├── sabrelite.rst
│   │   │   ├── sbsa.rst
│   │   │   ├── stellaris.rst
│   │   │   ├── stm32.rst
│   │   │   ├── sx1.rst
│   │   │   ├── versatile.rst
│   │   │   ├── vexpress.rst
│   │   │   ├── virt.rst
│   │   │   ├── vmapple.rst
│   │   │   ├── xenpvh.rst
│   │   │   ├── xlnx-versal-virt.rst
│   │   │   ├── xlnx-zcu102.rst
│   │   │   └── xlnx-zynq.rst
│   │   ├── authz.rst
│   │   ├── barrier.rst
│   │   ├── bootindex.rst
│   │   ├── confidential-guest-support.rst
│   │   ├── cpu-hotplug.rst
│   │   ├── cpu-models-mips.rst.inc
│   │   ├── cpu-models-x86-abi.csv
│   │   ├── cpu-models-x86.rst.inc
│   │   ├── device-emulation.rst
│   │   ├── device-url-syntax.rst.inc
│   │   ├── devices
│   │   │   ├── can.rst
│   │   │   ├── canokey.rst
│   │   │   ├── ccid.rst
│   │   │   ├── cxl.rst
│   │   │   ├── igb.rst
│   │   │   ├── ivshmem-flat.rst
│   │   │   ├── ivshmem.rst
│   │   │   ├── keyboard.rst
│   │   │   ├── net.rst
│   │   │   ├── nvme.rst
│   │   │   ├── usb-u2f.rst
│   │   │   ├── usb.rst
│   │   │   ├── vhost-user-input.rst
│   │   │   ├── vhost-user-rng.rst
│   │   │   ├── vhost-user.rst
│   │   │   ├── virtio-gpu.rst
│   │   │   ├── virtio-pmem.rst
│   │   │   └── virtio-snd.rst
│   │   ├── gdb.rst
│   │   ├── generic-loader.rst
│   │   ├── guest-loader.rst
│   │   ├── i386
│   │   │   ├── amd-memory-encryption.rst
│   │   │   ├── cpu.rst
│   │   │   ├── hyperv.rst
│   │   │   ├── kvm-pv.rst
│   │   │   ├── microvm.rst
│   │   │   ├── nitro-enclave.rst
│   │   │   ├── pc.rst
│   │   │   ├── sgx.rst
│   │   │   ├── tdx.rst
│   │   │   ├── xen.rst
│   │   │   └── xenpvh.rst
│   │   ├── images.rst
│   │   ├── index.rst
│   │   ├── introduction.rst
│   │   ├── invocation.rst
│   │   ├── keys.rst
│   │   ├── keys.rst.inc
│   │   ├── linuxboot.rst
│   │   ├── loongarch
│   │   │   └── virt.rst
│   │   ├── managed-startup.rst
│   │   ├── monitor.rst
│   │   ├── multi-process.rst
│   │   ├── mux-chardev.rst
│   │   ├── mux-chardev.rst.inc
│   │   ├── openrisc
│   │   │   ├── cpu-features.rst
│   │   │   ├── emulation.rst
│   │   │   ├── or1k-sim.rst
│   │   │   └── virt.rst
│   │   ├── ppc
│   │   │   ├── amigang.rst
│   │   │   ├── embedded.rst
│   │   │   ├── powermac.rst
│   │   │   ├── powernv.rst
│   │   │   ├── ppce500.rst
│   │   │   ├── prep.rst
│   │   │   └── pseries.rst
│   │   ├── pr-manager.rst
│   │   ├── qemu-block-drivers.rst
│   │   ├── qemu-block-drivers.rst.inc
│   │   ├── qemu-cpu-models.rst
│   │   ├── qemu-manpage.rst
│   │   ├── replay.rst
│   │   ├── riscv
│   │   │   ├── microblaze-v-generic.rst
│   │   │   ├── microchip-icicle-kit.rst
│   │   │   ├── shakti-c.rst
│   │   │   ├── sifive_u.rst
│   │   │   └── virt.rst
│   │   ├── s390x
│   │   │   ├── 3270.rst
│   │   │   ├── bootdevices.rst
│   │   │   ├── cpu-topology.rst
│   │   │   ├── css.rst
│   │   │   ├── pcidevices.rst
│   │   │   ├── protvirt.rst
│   │   │   ├── vfio-ap.rst
│   │   │   └── vfio-ccw.rst
│   │   ├── secrets.rst
│   │   ├── security.rst
│   │   ├── sriov.rst
│   │   ├── target-arm.rst
│   │   ├── target-avr.rst
│   │   ├── target-i386-desc.rst.inc
│   │   ├── target-i386.rst
│   │   ├── target-loongarch.rst
│   │   ├── target-m68k.rst
│   │   ├── target-mips.rst
│   │   ├── target-openrisc.rst
│   │   ├── target-ppc.rst
│   │   ├── target-riscv.rst
│   │   ├── target-rx.rst
│   │   ├── target-s390x.rst
│   │   ├── target-sparc.rst
│   │   ├── target-sparc64.rst
│   │   ├── target-xtensa.rst
│   │   ├── targets.rst
│   │   ├── tls.rst
│   │   ├── virtio-net-failover.rst
│   │   ├── vm-templating.rst
│   │   └── vnc-security.rst
│   ├── throttle.txt
│   ├── tools
│   │   ├── index.rst
│   │   ├── qemu-img.rst
│   │   ├── qemu-nbd.rst
│   │   ├── qemu-pr-helper.rst
│   │   ├── qemu-storage-daemon.rst
│   │   ├── qemu-trace-stap.rst
│   │   └── qemu-vmsr-helper.rst
│   ├── user
│   │   ├── index.rst
│   │   └── main.rst
│   ├── xbzrle.txt
│   └── xen-save-devices-state.txt
├── dump
│   ├── dump-hmp-cmds.c
│   ├── dump.c
│   ├── meson.build
│   ├── win_dump.c
│   └── win_dump.h
├── ebpf
│   ├── ebpf_rss-stub.c
│   ├── ebpf_rss.c
│   ├── ebpf_rss.h
│   ├── ebpf.c
│   ├── ebpf.h
│   ├── meson.build
│   ├── rss.bpf.skeleton.h
│   ├── trace-events
│   └── trace.h
├── event-loop-base.c
├── fpu
│   ├── meson.build
│   ├── softfloat-parts-addsub.c.inc
│   ├── softfloat-parts.c.inc
│   ├── softfloat-specialize.c.inc
│   └── softfloat.c
├── fsdev
│   ├── 9p-iov-marshal.c
│   ├── 9p-iov-marshal.h
│   ├── 9p-marshal.c
│   ├── 9p-marshal.h
│   ├── file-op-9p.h
│   ├── meson.build
│   ├── p9array.h
│   ├── qemu-fsdev-dummy.c
│   ├── qemu-fsdev-opts.c
│   ├── qemu-fsdev-throttle.c
│   ├── qemu-fsdev-throttle.h
│   ├── qemu-fsdev.c
│   └── qemu-fsdev.h
├── gdb-xml
│   ├── aarch64-core.xml
│   ├── aarch64-fpu.xml
│   ├── aarch64-mte.xml
│   ├── aarch64-pauth.xml
│   ├── arm-core.xml
│   ├── arm-m-profile-mve.xml
│   ├── arm-m-profile.xml
│   ├── arm-neon.xml
│   ├── arm-vfp-sysregs.xml
│   ├── arm-vfp.xml
│   ├── arm-vfp3.xml
│   ├── avr-cpu.xml
│   ├── cf-core.xml
│   ├── cf-fp.xml
│   ├── hexagon-core.xml
│   ├── hexagon-hvx.xml
│   ├── i386-32bit-linux.xml
│   ├── i386-32bit.xml
│   ├── i386-64bit-linux.xml
│   ├── i386-64bit.xml
│   ├── loongarch-base32.xml
│   ├── loongarch-base64.xml
│   ├── loongarch-fpu.xml
│   ├── loongarch-lasx.xml
│   ├── loongarch-lsx.xml
│   ├── m68k-core.xml
│   ├── m68k-fp.xml
│   ├── microblaze-core.xml
│   ├── microblaze-stack-protect.xml
│   ├── power-altivec.xml
│   ├── power-core.xml
│   ├── power-fpu.xml
│   ├── power-spe.xml
│   ├── power-vsx.xml
│   ├── power64-core.xml
│   ├── riscv-32bit-cpu.xml
│   ├── riscv-32bit-fpu.xml
│   ├── riscv-32bit-virtual.xml
│   ├── riscv-64bit-cpu.xml
│   ├── riscv-64bit-fpu.xml
│   ├── riscv-64bit-virtual.xml
│   ├── rx-core.xml
│   ├── s390-acr.xml
│   ├── s390-cr.xml
│   ├── s390-fpr.xml
│   ├── s390-gs.xml
│   ├── s390-virt-kvm.xml
│   ├── s390-virt.xml
│   ├── s390-vx.xml
│   └── s390x-core64.xml
├── gdbstub
│   ├── gdbstub.c
│   ├── internals.h
│   ├── meson.build
│   ├── syscalls.c
│   ├── system.c
│   ├── trace-events
│   ├── trace.h
│   ├── user-target.c
│   └── user.c
├── gitdm.config
├── hmp-commands-info.hx
├── hmp-commands.hx
├── host
│   └── include
│       ├── aarch64
│       │   └── host
│       │       ├── atomic128-cas.h
│       │       ├── atomic128-ldst.h.inc
│       │       ├── bufferiszero.c.inc
│       │       ├── cpuinfo.h
│       │       ├── crypto
│       │       │   ├── aes-round.h
│       │       │   └── clmul.h
│       │       ├── load-extract-al16-al8.h.inc
│       │       └── store-insert-al16.h.inc
│       ├── generic
│       │   └── host
│       │       ├── atomic128-cas.h.inc
│       │       ├── atomic128-ldst.h.inc
│       │       ├── bufferiszero.c.inc
│       │       ├── cpuinfo.h
│       │       ├── crypto
│       │       │   ├── aes-round.h
│       │       │   └── clmul.h
│       │       ├── load-extract-al16-al8.h.inc
│       │       └── store-insert-al16.h.inc
│       ├── i386
│       │   └── host
│       │       ├── bufferiszero.c.inc
│       │       ├── cpuinfo.h
│       │       └── crypto
│       │           ├── aes-round.h
│       │           └── clmul.h
│       ├── loongarch64
│       │   └── host
│       │       ├── atomic128-ldst.h.inc
│       │       ├── bufferiszero.c.inc
│       │       ├── cpuinfo.h
│       │       ├── load-extract-al16-al8.h.inc
│       │       └── store-insert-al16.h.inc
│       ├── ppc
│       │   └── host
│       │       ├── cpuinfo.h
│       │       └── crypto
│       │           └── aes-round.h
│       ├── ppc64
│       │   └── host
│       │       ├── cpuinfo.h
│       │       └── crypto
│       │           └── aes-round.h
│       ├── riscv
│       │   └── host
│       │       └── cpuinfo.h
│       └── x86_64
│           └── host
│               ├── atomic128-ldst.h.inc
│               ├── bufferiszero.c.inc
│               ├── cpuinfo.h
│               ├── crypto
│               │   ├── aes-round.h
│               │   └── clmul.h
│               └── load-extract-al16-al8.h.inc
├── hw
│   ├── 9pfs
│   │   ├── 9p-local.c
│   │   ├── 9p-local.h
│   │   ├── 9p-posix-acl.c
│   │   ├── 9p-synth.c
│   │   ├── 9p-synth.h
│   │   ├── 9p-util-darwin.c
│   │   ├── 9p-util-generic.c
│   │   ├── 9p-util-linux.c
│   │   ├── 9p-util.h
│   │   ├── 9p-xattr-user.c
│   │   ├── 9p-xattr.c
│   │   ├── 9p-xattr.h
│   │   ├── 9p.c
│   │   ├── 9p.h
│   │   ├── codir.c
│   │   ├── cofile.c
│   │   ├── cofs.c
│   │   ├── coth.c
│   │   ├── coth.h
│   │   ├── coxattr.c
│   │   ├── Kconfig
│   │   ├── meson.build
│   │   ├── trace-events
│   │   ├── trace.h
│   │   ├── virtio-9p-device.c
│   │   ├── virtio-9p.h
│   │   ├── xen-9p-backend.c
│   │   └── xen-9pfs.h
│   ├── acpi
│   │   ├── acpi_interface.c
│   │   ├── acpi-cpu-hotplug-stub.c
│   │   ├── acpi-mem-hotplug-stub.c
│   │   ├── acpi-nvdimm-stub.c
│   │   ├── acpi-pci-hotplug-stub.c
│   │   ├── acpi-qmp-cmds.c
│   │   ├── acpi-stub.c
│   │   ├── acpi-x86-stub.c
│   │   ├── aml-build-stub.c
│   │   ├── aml-build.c
│   │   ├── bios-linker-loader.c
│   │   ├── core.c
│   │   ├── cpu_hotplug.c
│   │   ├── cpu.c
│   │   ├── cxl-stub.c
│   │   ├── cxl.c
│   │   ├── erst.c
│   │   ├── generic_event_device.c
│   │   ├── ghes-stub.c
│   │   ├── ghes.c
│   │   ├── hmat.c
│   │   ├── hmat.h
│   │   ├── ich9_tco.c
│   │   ├── ich9_timer.c
│   │   ├── ich9.c
│   │   ├── ipmi-stub.c
│   │   ├── ipmi.c
│   │   ├── Kconfig
│   │   ├── memory_hotplug.c
│   │   ├── meson.build
│   │   ├── nvdimm.c
│   │   ├── pci-bridge-stub.c
│   │   ├── pci-bridge.c
│   │   ├── pci.c
│   │   ├── pcihp.c
│   │   ├── piix4.c
│   │   ├── tpm.c
│   │   ├── trace-events
│   │   ├── trace.h
│   │   ├── utils.c
│   │   ├── viot.c
│   │   ├── viot.h
│   │   ├── vmclock.c
│   │   └── vmgenid.c
│   ├── adc
│   │   ├── aspeed_adc.c
│   │   ├── Kconfig
│   │   ├── meson.build
│   │   ├── npcm7xx_adc.c
│   │   ├── stm32f2xx_adc.c
│   │   ├── trace-events
│   │   ├── trace.h
│   │   └── zynq-xadc.c
│   ├── alpha
│   │   ├── alpha_sys.h
│   │   ├── dp264.c
│   │   ├── Kconfig
│   │   ├── meson.build
│   │   ├── pci.c
│   │   ├── trace-events
│   │   ├── trace.h
│   │   └── typhoon.c
│   ├── arm
│   │   ├── allwinner-a10.c
│   │   ├── allwinner-h3.c
│   │   ├── allwinner-r40.c
│   │   ├── armsse.c
│   │   ├── armv7m.c
│   │   ├── aspeed_ast10x0.c
│   │   ├── aspeed_ast2400.c
│   │   ├── aspeed_ast2600.c
│   │   ├── aspeed_ast27x0-fc.c
│   │   ├── aspeed_ast27x0-ssp.c
│   │   ├── aspeed_ast27x0-tsp.c
│   │   ├── aspeed_ast27x0.c
│   │   ├── aspeed_eeprom.c
│   │   ├── aspeed_eeprom.h
│   │   ├── aspeed_soc_common.c
│   │   ├── aspeed.c
│   │   ├── b-l475e-iot01a.c
│   │   ├── bananapi_m2u.c
│   │   ├── bcm2835_peripherals.c
│   │   ├── bcm2836.c
│   │   ├── bcm2838_peripherals.c
│   │   ├── bcm2838.c
│   │   ├── boot.c
│   │   ├── collie.c
│   │   ├── cubieboard.c
│   │   ├── digic_boards.c
│   │   ├── digic.c
│   │   ├── exynos4_boards.c
│   │   ├── exynos4210.c
│   │   ├── fby35.c
│   │   ├── fsl-imx25.c
│   │   ├── fsl-imx31.c
│   │   ├── fsl-imx6.c
│   │   ├── fsl-imx6ul.c
│   │   ├── fsl-imx7.c
│   │   ├── fsl-imx8mp.c
│   │   ├── highbank.c
│   │   ├── imx25_pdk.c
│   │   ├── imx8mp-evk.c
│   │   ├── integratorcp.c
│   │   ├── Kconfig
│   │   ├── kzm.c
│   │   ├── mcimx6ul-evk.c
│   │   ├── mcimx7d-sabre.c
│   │   ├── meson.build
│   │   ├── microbit.c
│   │   ├── mps2-tz.c
│   │   ├── mps2.c
│   │   ├── mps3r.c
│   │   ├── msf2-soc.c
│   │   ├── msf2-som.c
│   │   ├── musca.c
│   │   ├── musicpal.c
│   │   ├── netduino2.c
│   │   ├── netduinoplus2.c
│   │   ├── npcm7xx_boards.c
│   │   ├── npcm7xx.c
│   │   ├── npcm8xx_boards.c
│   │   ├── npcm8xx.c
│   │   ├── nrf51_soc.c
│   │   ├── olimex-stm32-h405.c
│   │   ├── omap_sx1.c
│   │   ├── omap1.c
│   │   ├── orangepi.c
│   │   ├── raspi.c
│   │   ├── raspi4b.c
│   │   ├── realview.c
│   │   ├── sabrelite.c
│   │   ├── sbsa-ref.c
│   │   ├── smmu-common.c
│   │   ├── smmu-internal.h
│   │   ├── smmuv3-internal.h
│   │   ├── smmuv3.c
│   │   ├── stellaris.c
│   │   ├── stm32f100_soc.c
│   │   ├── stm32f205_soc.c
│   │   ├── stm32f405_soc.c
│   │   ├── stm32l4x5_soc.c
│   │   ├── stm32vldiscovery.c
│   │   ├── strongarm.c
│   │   ├── strongarm.h
│   │   ├── trace-events
│   │   ├── trace.h
│   │   ├── versatilepb.c
│   │   ├── vexpress.c
│   │   ├── virt-acpi-build.c
│   │   ├── virt.c
│   │   ├── xen-pvh.c
│   │   ├── xen-stubs.c
│   │   ├── xilinx_zynq.c
│   │   ├── xlnx-versal-virt.c
│   │   ├── xlnx-versal.c
│   │   ├── xlnx-zcu102.c
│   │   └── xlnx-zynqmp.c
│   ├── audio
│   │   ├── ac97.c
│   │   ├── ac97.h
│   │   ├── adlib.c
│   │   ├── asc.c
│   │   ├── cs4231.c
│   │   ├── cs4231a.c
│   │   ├── es1370.c
│   │   ├── fmopl.c
│   │   ├── fmopl.h
│   │   ├── gus.c
│   │   ├── gusemu_hal.c
│   │   ├── gusemu_mixer.c
│   │   ├── gusemu.h
│   │   ├── gustate.h
│   │   ├── hda-codec-common.h
│   │   ├── hda-codec.c
│   │   ├── intel-hda-defs.h
│   │   ├── intel-hda.c
│   │   ├── intel-hda.h
│   │   ├── Kconfig
│   │   ├── lm4549.c
│   │   ├── lm4549.h
│   │   ├── marvell_88w8618.c
│   │   ├── meson.build
│   │   ├── pcspk.c
│   │   ├── pl041.c
│   │   ├── pl041.h
│   │   ├── pl041.hx
│   │   ├── sb16.c
│   │   ├── soundhw.c
│   │   ├── trace-events
│   │   ├── trace.h
│   │   ├── via-ac97.c
│   │   ├── virtio-snd-pci.c
│   │   ├── virtio-snd.c
│   │   └── wm8750.c
│   ├── avr
│   │   ├── arduino.c
│   │   ├── atmega.c
│   │   ├── atmega.h
│   │   ├── boot.c
│   │   ├── boot.h
│   │   ├── Kconfig
│   │   └── meson.build
│   ├── block
│   │   ├── block.c
│   │   ├── cdrom.c
│   │   ├── dataplane
│   │   │   ├── meson.build
│   │   │   ├── xen-block.c
│   │   │   └── xen-block.h
│   │   ├── fdc-internal.h
│   │   ├── fdc-isa.c
│   │   ├── fdc-sysbus.c
│   │   ├── fdc.c
│   │   ├── hd-geometry.c
│   │   ├── Kconfig
│   │   ├── m25p80_sfdp.c
│   │   ├── m25p80_sfdp.h
│   │   ├── m25p80.c
│   │   ├── meson.build
│   │   ├── pflash_cfi01.c
│   │   ├── pflash_cfi02.c
│   │   ├── swim.c
│   │   ├── trace-events
│   │   ├── trace.h
│   │   ├── vhost-user-blk.c
│   │   ├── virtio-blk-common.c
│   │   ├── virtio-blk.c
│   │   ├── xen_blkif.h
│   │   └── xen-block.c
│   ├── char
│   │   ├── avr_usart.c
│   │   ├── bcm2835_aux.c
│   │   ├── cadence_uart.c
│   │   ├── cmsdk-apb-uart.c
│   │   ├── debugcon.c
│   │   ├── digic-uart.c
│   │   ├── diva-gsp.c
│   │   ├── escc.c
│   │   ├── exynos4210_uart.c
│   │   ├── goldfish_tty.c
│   │   ├── grlib_apbuart.c
│   │   ├── ibex_uart.c
│   │   ├── imx_serial.c
│   │   ├── ipoctal232.c
│   │   ├── Kconfig
│   │   ├── mcf_uart.c
│   │   ├── mchp_pfsoc_mmuart.c
│   │   ├── meson.build
│   │   ├── nrf51_uart.c
│   │   ├── omap_uart.c
│   │   ├── parallel-isa.c
│   │   ├── parallel.c
│   │   ├── pl011.c
│   │   ├── renesas_sci.c
│   │   ├── riscv_htif.c
│   │   ├── sclpconsole-lm.c
│   │   ├── sclpconsole.c
│   │   ├── serial-isa.c
│   │   ├── serial-mm.c
│   │   ├── serial-pci-multi.c
│   │   ├── serial-pci.c
│   │   ├── serial.c
│   │   ├── sh_serial.c
│   │   ├── shakti_uart.c
│   │   ├── sifive_uart.c
│   │   ├── spapr_vty.c
│   │   ├── stm32f2xx_usart.c
│   │   ├── stm32l4x5_usart.c
│   │   ├── terminal3270.c
│   │   ├── trace-events
│   │   ├── trace.h
│   │   ├── virtio-console.c
│   │   ├── virtio-serial-bus.c
│   │   ├── xen_console.c
│   │   └── xilinx_uartlite.c
│   ├── core
│   │   ├── bus.c
│   │   ├── clock-vmstate.c
│   │   ├── clock.c
│   │   ├── cpu-common.c
│   │   ├── cpu-system.c
│   │   ├── cpu-user.c
│   │   ├── eif.c
│   │   ├── eif.h
│   │   ├── fw-path-provider.c
│   │   ├── generic-loader.c
│   │   ├── gpio.c
│   │   ├── guest-loader.c
│   │   ├── guest-loader.h
│   │   ├── hotplug.c
│   │   ├── irq.c
│   │   ├── Kconfig
│   │   ├── loader-fit.c
│   │   ├── loader.c
│   │   ├── machine-hmp-cmds.c
│   │   ├── machine-qmp-cmds.c
│   │   ├── machine-smp.c
│   │   ├── machine.c
│   │   ├── meson.build
│   │   ├── nmi.c
│   │   ├── null-machine.c
│   │   ├── numa.c
│   │   ├── or-irq.c
│   │   ├── platform-bus.c
│   │   ├── ptimer.c
│   │   ├── qdev-clock.c
│   │   ├── qdev-fw.c
│   │   ├── qdev-hotplug.c
│   │   ├── qdev-prop-internal.h
│   │   ├── qdev-properties-system.c
│   │   ├── qdev-properties.c
│   │   ├── qdev-user.c
│   │   ├── qdev.c
│   │   ├── register.c
│   │   ├── reset.c
│   │   ├── resetcontainer.c
│   │   ├── resettable.c
│   │   ├── split-irq.c
│   │   ├── stream.c
│   │   ├── sysbus-fdt.c
│   │   ├── sysbus.c
│   │   ├── trace-events
│   │   ├── trace.h
│   │   ├── uboot_image.h
│   │   ├── vm-change-state-handler.c
│   │   └── vmstate-if.c
│   ├── cpu
│   │   ├── a15mpcore.c
│   │   ├── a9mpcore.c
│   │   ├── arm11mpcore.c
│   │   ├── cluster.c
│   │   ├── core.c
│   │   ├── Kconfig
│   │   ├── meson.build
│   │   └── realview_mpcore.c
│   ├── cxl
│   │   ├── cxl-cdat.c
│   │   ├── cxl-component-utils.c
│   │   ├── cxl-device-utils.c
│   │   ├── cxl-events.c
│   │   ├── cxl-host-stubs.c
│   │   ├── cxl-host.c
│   │   ├── cxl-mailbox-utils.c
│   │   ├── Kconfig
│   │   ├── meson.build
│   │   └── switch-mailbox-cci.c
│   ├── display
│   │   ├── acpi-vga-stub.c
│   │   ├── acpi-vga.c
│   │   ├── apple-gfx-mmio.m
│   │   ├── apple-gfx-pci.m
│   │   ├── apple-gfx.h
│   │   ├── apple-gfx.m
│   │   ├── artist.c
│   │   ├── ati_2d.c
│   │   ├── ati_dbg.c
│   │   ├── ati_int.h
│   │   ├── ati_regs.h
│   │   ├── ati.c
│   │   ├── bcm2835_fb.c
│   │   ├── bochs-display.c
│   │   ├── cg3.c
│   │   ├── cirrus_vga_internal.h
│   │   ├── cirrus_vga_isa.c
│   │   ├── cirrus_vga_rop.h
│   │   ├── cirrus_vga_rop2.h
│   │   ├── cirrus_vga.c
│   │   ├── dm163.c
│   │   ├── dpcd.c
│   │   ├── edid-generate.c
│   │   ├── edid-region.c
│   │   ├── exynos4210_fimd.c
│   │   ├── framebuffer.c
│   │   ├── framebuffer.h
│   │   ├── g364fb.c
│   │   ├── i2c-ddc.c
│   │   ├── jazz_led.c
│   │   ├── Kconfig
│   │   ├── macfb.c
│   │   ├── meson.build
│   │   ├── next-fb.c
│   │   ├── omap_lcdc.c
│   │   ├── pl110_template.h
│   │   ├── pl110.c
│   │   ├── qxl-logger.c
│   │   ├── qxl-render.c
│   │   ├── qxl.c
│   │   ├── qxl.h
│   │   ├── ramfb-standalone.c
│   │   ├── ramfb-stubs.c
│   │   ├── ramfb.c
│   │   ├── sii9022.c
│   │   ├── sm501.c
│   │   ├── ssd0303.c
│   │   ├── ssd0323.c
│   │   ├── tcx.c
│   │   ├── trace-events
│   │   ├── trace.h
│   │   ├── vga_int.h
│   │   ├── vga_regs.h
│   │   ├── vga-access.h
│   │   ├── vga-helpers.h
│   │   ├── vga-isa.c
│   │   ├── vga-mmio.c
│   │   ├── vga-pci.c
│   │   ├── vga.c
│   │   ├── vhost-user-gpu-pci.c
│   │   ├── vhost-user-gpu.c
│   │   ├── vhost-user-vga.c
│   │   ├── virtio-dmabuf.c
│   │   ├── virtio-gpu-base.c
│   │   ├── virtio-gpu-gl.c
│   │   ├── virtio-gpu-pci-gl.c
│   │   ├── virtio-gpu-pci-rutabaga.c
│   │   ├── virtio-gpu-pci.c
│   │   ├── virtio-gpu-rutabaga.c
│   │   ├── virtio-gpu-udmabuf-stubs.c
│   │   ├── virtio-gpu-udmabuf.c
│   │   ├── virtio-gpu-virgl.c
│   │   ├── virtio-gpu.c
│   │   ├── virtio-vga-gl.c
│   │   ├── virtio-vga-rutabaga.c
│   │   ├── virtio-vga.c
│   │   ├── virtio-vga.h
│   │   ├── vmware_vga.c
│   │   ├── xenfb.c
│   │   └── xlnx_dp.c
│   ├── dma
│   │   ├── bcm2835_dma.c
│   │   ├── i82374.c
│   │   ├── i8257.c
│   │   ├── Kconfig
│   │   ├── meson.build
│   │   ├── omap_dma.c
│   │   ├── pl080.c
│   │   ├── pl330.c
│   │   ├── rc4030.c
│   │   ├── sifive_pdma.c
│   │   ├── soc_dma.c
│   │   ├── sparc32_dma.c
│   │   ├── trace-events
│   │   ├── trace.h
│   │   ├── xilinx_axidma.c
│   │   ├── xlnx_csu_dma.c
│   │   ├── xlnx_dpdma.c
│   │   ├── xlnx-zdma.c
│   │   └── xlnx-zynq-devcfg.c
│   ├── fsi
│   │   ├── aspeed_apb2opb.c
│   │   ├── cfam.c
│   │   ├── fsi-master.c
│   │   ├── fsi.c
│   │   ├── Kconfig
│   │   ├── lbus.c
│   │   ├── meson.build
│   │   ├── trace-events
│   │   └── trace.h
│   ├── gpio
│   │   ├── aspeed_gpio.c
│   │   ├── bcm2835_gpio.c
│   │   ├── bcm2838_gpio.c
│   │   ├── gpio_key.c
│   │   ├── gpio_pwr.c
│   │   ├── imx_gpio.c
│   │   ├── Kconfig
│   │   ├── meson.build
│   │   ├── mpc8xxx.c
│   │   ├── npcm7xx_gpio.c
│   │   ├── nrf51_gpio.c
│   │   ├── omap_gpio.c
│   │   ├── pca9552.c
│   │   ├── pca9554.c
│   │   ├── pcf8574.c
│   │   ├── pl061.c
│   │   ├── sifive_gpio.c
│   │   ├── stm32l4x5_gpio.c
│   │   ├── trace-events
│   │   ├── trace.h
│   │   └── zaurus.c
│   ├── hppa
│   │   ├── hppa_hardware.h
│   │   ├── Kconfig
│   │   ├── machine.c
│   │   ├── meson.build
│   │   └── trace.h
│   ├── hyperv
│   │   ├── hv-balloon-internal.h
│   │   ├── hv-balloon-our_range_memslots.c
│   │   ├── hv-balloon-our_range_memslots.h
│   │   ├── hv-balloon-page_range_tree.c
│   │   ├── hv-balloon-page_range_tree.h
│   │   ├── hv-balloon-stub.c
│   │   ├── hv-balloon.c
│   │   ├── hyperv_testdev.c
│   │   ├── hyperv.c
│   │   ├── Kconfig
│   │   ├── meson.build
│   │   ├── syndbg.c
│   │   ├── trace-events
│   │   ├── trace.h
│   │   └── vmbus.c
│   ├── i2c
│   │   ├── allwinner-i2c.c
│   │   ├── arm_sbcon_i2c.c
│   │   ├── aspeed_i2c.c
│   │   ├── bcm2835_i2c.c
│   │   ├── bitbang_i2c.c
│   │   ├── core.c
│   │   ├── exynos4210_i2c.c
│   │   ├── i2c_mux_pca954x.c
│   │   ├── imx_i2c.c
│   │   ├── Kconfig
│   │   ├── meson.build
│   │   ├── microbit_i2c.c
│   │   ├── mpc_i2c.c
│   │   ├── npcm7xx_smbus.c
│   │   ├── omap_i2c.c
│   │   ├── pm_smbus.c
│   │   ├── pmbus_device.c
│   │   ├── ppc4xx_i2c.c
│   │   ├── smbus_eeprom.c
│   │   ├── smbus_ich9.c
│   │   ├── smbus_master.c
│   │   ├── smbus_slave.c
│   │   ├── trace-events
│   │   └── trace.h
│   ├── i386
│   │   ├── acpi-build.c
│   │   ├── acpi-build.h
│   │   ├── acpi-common.c
│   │   ├── acpi-common.h
│   │   ├── acpi-microvm.c
│   │   ├── acpi-microvm.h
│   │   ├── amd_iommu-stub.c
│   │   ├── amd_iommu.c
│   │   ├── amd_iommu.h
│   │   ├── e820_memory_layout.c
│   │   ├── e820_memory_layout.h
│   │   ├── fw_cfg.c
│   │   ├── fw_cfg.h
│   │   ├── intel_iommu_internal.h
│   │   ├── intel_iommu.c
│   │   ├── Kconfig
│   │   ├── kvm
│   │   │   ├── apic.c
│   │   │   ├── clock.c
│   │   │   ├── clock.h
│   │   │   ├── i8254.c
│   │   │   ├── i8259.c
│   │   │   ├── ioapic.c
│   │   │   ├── meson.build
│   │   │   ├── trace-events
│   │   │   ├── trace.h
│   │   │   ├── xen_evtchn.c
│   │   │   ├── xen_evtchn.h
│   │   │   ├── xen_gnttab.c
│   │   │   ├── xen_gnttab.h
│   │   │   ├── xen_overlay.c
│   │   │   ├── xen_overlay.h
│   │   │   ├── xen_primary_console.c
│   │   │   ├── xen_primary_console.h
│   │   │   ├── xen_xenstore.c
│   │   │   ├── xen_xenstore.h
│   │   │   ├── xen-stubs.c
│   │   │   ├── xenstore_impl.c
│   │   │   └── xenstore_impl.h
│   │   ├── meson.build
│   │   ├── microvm-dt.c
│   │   ├── microvm-dt.h
│   │   ├── microvm.c
│   │   ├── monitor.c
│   │   ├── multiboot.c
│   │   ├── multiboot.h
│   │   ├── nitro_enclave.c
│   │   ├── pc_piix.c
│   │   ├── pc_q35.c
│   │   ├── pc_sysfw_ovmf-stubs.c
│   │   ├── pc_sysfw_ovmf.c
│   │   ├── pc_sysfw.c
│   │   ├── pc.c
│   │   ├── port92.c
│   │   ├── sgx-epc.c
│   │   ├── sgx-stub.c
│   │   ├── sgx.c
│   │   ├── tdvf-hob.c
│   │   ├── tdvf-hob.h
│   │   ├── tdvf.c
│   │   ├── trace-events
│   │   ├── trace.h
│   │   ├── vapic.c
│   │   ├── vmmouse.c
│   │   ├── vmport.c
│   │   ├── x86-common.c
│   │   ├── x86-cpu.c
│   │   ├── x86-iommu-stub.c
│   │   ├── x86-iommu.c
│   │   ├── x86.c
│   │   └── xen
│   │       ├── meson.build
│   │       ├── trace-events
│   │       ├── trace.h
│   │       ├── xen_apic.c
│   │       ├── xen_platform.c
│   │       ├── xen_pvdevice.c
│   │       ├── xen-hvm.c
│   │       └── xen-pvh.c
│   ├── ide
│   │   ├── ahci-allwinner.c
│   │   ├── ahci-internal.h
│   │   ├── ahci-sysbus.c
│   │   ├── ahci.c
│   │   ├── atapi.c
│   │   ├── cf.c
│   │   ├── cmd646.c
│   │   ├── core.c
│   │   ├── ich.c
│   │   ├── ide-bus.c
│   │   ├── ide-dev.c
│   │   ├── ide-internal.h
│   │   ├── ioport.c
│   │   ├── isa.c
│   │   ├── Kconfig
│   │   ├── macio.c
│   │   ├── meson.build
│   │   ├── mmio.c
│   │   ├── pci.c
│   │   ├── piix.c
│   │   ├── sii3112.c
│   │   ├── trace-events
│   │   ├── trace.h
│   │   └── via.c
│   ├── input
│   │   ├── adb-internal.h
│   │   ├── adb-kbd.c
│   │   ├── adb-mouse.c
│   │   ├── adb.c
│   │   ├── hid.c
│   │   ├── Kconfig
│   │   ├── lasips2.c
│   │   ├── meson.build
│   │   ├── pckbd.c
│   │   ├── pl050.c
│   │   ├── ps2.c
│   │   ├── stellaris_gamepad.c
│   │   ├── trace-events
│   │   ├── trace.h
│   │   ├── virtio-input-hid.c
│   │   ├── virtio-input-host.c
│   │   └── virtio-input.c
│   ├── intc
│   │   ├── allwinner-a10-pic.c
│   │   ├── apic_common.c
│   │   ├── apic.c
│   │   ├── arm_gic_common.c
│   │   ├── arm_gic_kvm.c
│   │   ├── arm_gic.c
│   │   ├── arm_gicv2m.c
│   │   ├── arm_gicv3_common.c
│   │   ├── arm_gicv3_cpuif_common.c
│   │   ├── arm_gicv3_cpuif.c
│   │   ├── arm_gicv3_dist.c
│   │   ├── arm_gicv3_its_common.c
│   │   ├── arm_gicv3_its_kvm.c
│   │   ├── arm_gicv3_its.c
│   │   ├── arm_gicv3_kvm.c
│   │   ├── arm_gicv3_redist.c
│   │   ├── arm_gicv3.c
│   │   ├── armv7m_nvic.c
│   │   ├── aspeed_intc.c
│   │   ├── aspeed_vic.c
│   │   ├── bcm2835_ic.c
│   │   ├── bcm2836_control.c
│   │   ├── exynos4210_combiner.c
│   │   ├── exynos4210_gic.c
│   │   ├── gic_internal.h
│   │   ├── gicv3_internal.h
│   │   ├── goldfish_pic.c
│   │   ├── grlib_irqmp.c
│   │   ├── heathrow_pic.c
│   │   ├── i8259_common.c
│   │   ├── i8259.c
│   │   ├── imx_avic.c
│   │   ├── imx_gpcv2.c
│   │   ├── intc.c
│   │   ├── ioapic_common.c
│   │   ├── ioapic_internal.h
│   │   ├── ioapic-stub.c
│   │   ├── ioapic.c
│   │   ├── Kconfig
│   │   ├── kvm_irqcount.c
│   │   ├── loongarch_extioi_common.c
│   │   ├── loongarch_extioi_kvm.c
│   │   ├── loongarch_extioi.c
│   │   ├── loongarch_ipi_kvm.c
│   │   ├── loongarch_ipi.c
│   │   ├── loongarch_pch_msi.c
│   │   ├── loongarch_pch_pic.c
│   │   ├── loongarch_pic_common.c
│   │   ├── loongarch_pic_kvm.c
│   │   ├── loongson_ipi_common.c
│   │   ├── loongson_ipi.c
│   │   ├── loongson_liointc.c
│   │   ├── m68k_irqc.c
│   │   ├── meson.build
│   │   ├── mips_gic.c
│   │   ├── omap_intc.c
│   │   ├── ompic.c
│   │   ├── openpic_kvm.c
│   │   ├── openpic.c
│   │   ├── pl190.c
│   │   ├── pnv_xive_regs.h
│   │   ├── pnv_xive.c
│   │   ├── pnv_xive2_regs.h
│   │   ├── pnv_xive2.c
│   │   ├── ppc-uic.c
│   │   ├── realview_gic.c
│   │   ├── riscv_aclint.c
│   │   ├── riscv_aplic.c
│   │   ├── riscv_imsic.c
│   │   ├── rx_icu.c
│   │   ├── s390_flic_kvm.c
│   │   ├── s390_flic.c
│   │   ├── sh_intc.c
│   │   ├── sifive_plic.c
│   │   ├── slavio_intctl.c
│   │   ├── spapr_xive_kvm.c
│   │   ├── spapr_xive.c
│   │   ├── trace-events
│   │   ├── trace.h
│   │   ├── vgic_common.h
│   │   ├── xics_kvm.c
│   │   ├── xics_pnv.c
│   │   ├── xics_spapr.c
│   │   ├── xics.c
│   │   ├── xilinx_intc.c
│   │   ├── xive.c
│   │   ├── xive2.c
│   │   ├── xlnx-pmu-iomod-intc.c
│   │   └── xlnx-zynqmp-ipi.c
│   ├── ipack
│   │   ├── ipack.c
│   │   ├── Kconfig
│   │   ├── meson.build
│   │   └── tpci200.c
│   ├── ipmi
│   │   ├── ipmi_bmc_extern.c
│   │   ├── ipmi_bmc_sim.c
│   │   ├── ipmi_bt.c
│   │   ├── ipmi_kcs.c
│   │   ├── ipmi.c
│   │   ├── isa_ipmi_bt.c
│   │   ├── isa_ipmi_kcs.c
│   │   ├── Kconfig
│   │   ├── meson.build
│   │   ├── pci_ipmi_bt.c
│   │   ├── pci_ipmi_kcs.c
│   │   └── smbus_ipmi.c
│   ├── isa
│   │   ├── apm.c
│   │   ├── fdc37m81x-superio.c
│   │   ├── i82378.c
│   │   ├── isa-bus.c
│   │   ├── isa-superio.c
│   │   ├── Kconfig
│   │   ├── lpc_ich9.c
│   │   ├── meson.build
│   │   ├── pc87312.c
│   │   ├── piix.c
│   │   ├── smc37c669-superio.c
│   │   ├── trace-events
│   │   ├── trace.h
│   │   └── vt82c686.c
│   ├── Kconfig
│   ├── loongarch
│   │   ├── boot.c
│   │   ├── fw_cfg.c
│   │   ├── fw_cfg.h
│   │   ├── Kconfig
│   │   ├── meson.build
│   │   ├── virt-acpi-build.c
│   │   ├── virt-fdt-build.c
│   │   └── virt.c
│   ├── m68k
│   │   ├── an5206.c
│   │   ├── bootinfo.h
│   │   ├── Kconfig
│   │   ├── mcf_intc.c
│   │   ├── mcf5206.c
│   │   ├── mcf5208.c
│   │   ├── meson.build
│   │   ├── next-cube.c
│   │   ├── next-kbd.c
│   │   ├── q800-glue.c
│   │   ├── q800.c
│   │   └── virt.c
│   ├── mem
│   │   ├── cxl_type3_stubs.c
│   │   ├── cxl_type3.c
│   │   ├── Kconfig
│   │   ├── memory-device-stubs.c
│   │   ├── memory-device.c
│   │   ├── meson.build
│   │   ├── npcm7xx_mc.c
│   │   ├── nvdimm.c
│   │   ├── pc-dimm.c
│   │   ├── sparse-mem.c
│   │   ├── trace-events
│   │   └── trace.h
│   ├── meson.build
│   ├── microblaze
│   │   ├── boot.c
│   │   ├── boot.h
│   │   ├── Kconfig
│   │   ├── meson.build
│   │   ├── petalogix_ml605_mmu.c
│   │   ├── petalogix_s3adsp1800_mmu.c
│   │   └── xlnx-zynqmp-pmu.c
│   ├── mips
│   │   ├── bootloader.c
│   │   ├── boston.c
│   │   ├── cps.c
│   │   ├── fuloong2e.c
│   │   ├── fw_cfg.c
│   │   ├── fw_cfg.h
│   │   ├── jazz.c
│   │   ├── Kconfig
│   │   ├── loongson3_bootp.c
│   │   ├── loongson3_bootp.h
│   │   ├── loongson3_virt.c
│   │   ├── malta.c
│   │   ├── meson.build
│   │   ├── mips_int.c
│   │   ├── mipssim.c
│   │   ├── trace-events
│   │   └── trace.h
│   ├── misc
│   │   ├── a9scu.c
│   │   ├── allwinner-a10-ccm.c
│   │   ├── allwinner-a10-dramc.c
│   │   ├── allwinner-cpucfg.c
│   │   ├── allwinner-h3-ccu.c
│   │   ├── allwinner-h3-dramc.c
│   │   ├── allwinner-h3-sysctrl.c
│   │   ├── allwinner-r40-ccu.c
│   │   ├── allwinner-r40-dramc.c
│   │   ├── allwinner-sid.c
│   │   ├── allwinner-sramc.c
│   │   ├── applesmc.c
│   │   ├── arm_integrator_debug.c
│   │   ├── arm_l2x0.c
│   │   ├── arm_sysctl.c
│   │   ├── arm11scu.c
│   │   ├── armsse-cpu-pwrctrl.c
│   │   ├── armsse-cpuid.c
│   │   ├── armsse-mhu.c
│   │   ├── armv7m_ras.c
│   │   ├── aspeed_hace.c
│   │   ├── aspeed_i3c.c
│   │   ├── aspeed_lpc.c
│   │   ├── aspeed_peci.c
│   │   ├── aspeed_sbc.c
│   │   ├── aspeed_scu.c
│   │   ├── aspeed_sdmc.c
│   │   ├── aspeed_sli.c
│   │   ├── aspeed_xdma.c
│   │   ├── auxbus.c
│   │   ├── avr_power.c
│   │   ├── axp2xx.c
│   │   ├── bcm2835_cprman.c
│   │   ├── bcm2835_mbox.c
│   │   ├── bcm2835_mphi.c
│   │   ├── bcm2835_powermgt.c
│   │   ├── bcm2835_property.c
│   │   ├── bcm2835_rng.c
│   │   ├── bcm2835_thermal.c
│   │   ├── debugexit.c
│   │   ├── djmemc.c
│   │   ├── eccmemctl.c
│   │   ├── edu.c
│   │   ├── empty_slot.c
│   │   ├── exynos4210_clk.c
│   │   ├── exynos4210_pmu.c
│   │   ├── exynos4210_rng.c
│   │   ├── grlib_ahb_apb_pnp.c
│   │   ├── i2c-echo.c
│   │   ├── imx_ccm.c
│   │   ├── imx_rngc.c
│   │   ├── imx25_ccm.c
│   │   ├── imx31_ccm.c
│   │   ├── imx6_ccm.c
│   │   ├── imx6_src.c
│   │   ├── imx6ul_ccm.c
│   │   ├── imx7_ccm.c
│   │   ├── imx7_gpr.c
│   │   ├── imx7_snvs.c
│   │   ├── imx7_src.c
│   │   ├── imx8mp_analog.c
│   │   ├── imx8mp_ccm.c
│   │   ├── iosb.c
│   │   ├── iotkit-secctl.c
│   │   ├── iotkit-sysctl.c
│   │   ├── iotkit-sysinfo.c
│   │   ├── ivshmem-flat.c
│   │   ├── ivshmem-pci.c
│   │   ├── Kconfig
│   │   ├── lasi.c
│   │   ├── led.c
│   │   ├── mac_via.c
│   │   ├── macio
│   │   │   ├── cuda.c
│   │   │   ├── gpio.c
│   │   │   ├── Kconfig
│   │   │   ├── mac_dbdma.c
│   │   │   ├── macio.c
│   │   │   ├── meson.build
│   │   │   ├── pmu.c
│   │   │   ├── trace-events
│   │   │   └── trace.h
│   │   ├── mchp_pfsoc_dmc.c
│   │   ├── mchp_pfsoc_ioscb.c
│   │   ├── mchp_pfsoc_sysreg.c
│   │   ├── meson.build
│   │   ├── mips_cmgcr.c
│   │   ├── mips_cpc.c
│   │   ├── mips_itu.c
│   │   ├── mos6522.c
│   │   ├── mps2-fpgaio.c
│   │   ├── mps2-scc.c
│   │   ├── msf2-sysreg.c
│   │   ├── npcm_clk.c
│   │   ├── npcm_gcr.c
│   │   ├── npcm7xx_mft.c
│   │   ├── npcm7xx_pwm.c
│   │   ├── npcm7xx_rng.c
│   │   ├── nrf51_rng.c
│   │   ├── omap_clk.c
│   │   ├── pc-testdev.c
│   │   ├── pci-testdev.c
│   │   ├── pvpanic-isa.c
│   │   ├── pvpanic-mmio.c
│   │   ├── pvpanic-pci.c
│   │   ├── pvpanic.c
│   │   ├── sbsa_ec.c
│   │   ├── sifive_e_aon.c
│   │   ├── sifive_e_prci.c
│   │   ├── sifive_test.c
│   │   ├── sifive_u_otp.c
│   │   ├── sifive_u_prci.c
│   │   ├── slavio_misc.c
│   │   ├── stm32_rcc.c
│   │   ├── stm32f2xx_syscfg.c
│   │   ├── stm32f4xx_exti.c
│   │   ├── stm32f4xx_syscfg.c
│   │   ├── stm32l4x5_exti.c
│   │   ├── stm32l4x5_rcc.c
│   │   ├── stm32l4x5_syscfg.c
│   │   ├── trace-events
│   │   ├── trace.h
│   │   ├── tz-mpc.c
│   │   ├── tz-msc.c
│   │   ├── tz-ppc.c
│   │   ├── unimp.c
│   │   ├── virt_ctrl.c
│   │   ├── vmcoreinfo.c
│   │   ├── xlnx-cfi-if.c
│   │   ├── xlnx-versal-cframe-reg.c
│   │   ├── xlnx-versal-cfu.c
│   │   ├── xlnx-versal-crl.c
│   │   ├── xlnx-versal-pmc-iou-slcr.c
│   │   ├── xlnx-versal-trng.c
│   │   ├── xlnx-versal-xramc.c
│   │   ├── xlnx-zynqmp-apu-ctrl.c
│   │   ├── xlnx-zynqmp-crf.c
│   │   └── zynq_slcr.c
│   ├── net
│   │   ├── allwinner_emac.c
│   │   ├── allwinner-sun8i-emac.c
│   │   ├── cadence_gem.c
│   │   ├── can
│   │   │   ├── can_kvaser_pci.c
│   │   │   ├── can_mioe3680_pci.c
│   │   │   ├── can_pcm3680_pci.c
│   │   │   ├── can_sja1000.c
│   │   │   ├── can_sja1000.h
│   │   │   ├── ctu_can_fd_frame.h
│   │   │   ├── ctu_can_fd_regs.h
│   │   │   ├── ctucan_core.c
│   │   │   ├── ctucan_core.h
│   │   │   ├── ctucan_pci.c
│   │   │   ├── meson.build
│   │   │   ├── trace-events
│   │   │   ├── trace.h
│   │   │   ├── xlnx-versal-canfd.c
│   │   │   └── xlnx-zynqmp-can.c
│   │   ├── dp8393x.c
│   │   ├── e1000_common.h
│   │   ├── e1000_regs.h
│   │   ├── e1000.c
│   │   ├── e1000e_core.c
│   │   ├── e1000e_core.h
│   │   ├── e1000e.c
│   │   ├── e1000x_common.c
│   │   ├── e1000x_common.h
│   │   ├── e1000x_regs.h
│   │   ├── eepro100.c
│   │   ├── fsl_etsec
│   │   │   ├── etsec.c
│   │   │   ├── etsec.h
│   │   │   ├── miim.c
│   │   │   ├── registers.c
│   │   │   ├── registers.h
│   │   │   └── rings.c
│   │   ├── ftgmac100.c
│   │   ├── i82596.c
│   │   ├── i82596.h
│   │   ├── igb_common.h
│   │   ├── igb_core.c
│   │   ├── igb_core.h
│   │   ├── igb_regs.h
│   │   ├── igb.c
│   │   ├── igbvf.c
│   │   ├── imx_fec.c
│   │   ├── Kconfig
│   │   ├── lan9118_phy.c
│   │   ├── lan9118.c
│   │   ├── lance.c
│   │   ├── lasi_i82596.c
│   │   ├── mcf_fec.c
│   │   ├── meson.build
│   │   ├── mipsnet.c
│   │   ├── msf2-emac.c
│   │   ├── mv88w8618_eth.c
│   │   ├── ne2000-isa.c
│   │   ├── ne2000-pci.c
│   │   ├── ne2000.c
│   │   ├── ne2000.h
│   │   ├── net_rx_pkt.c
│   │   ├── net_rx_pkt.h
│   │   ├── net_tx_pkt.c
│   │   ├── net_tx_pkt.h
│   │   ├── npcm_gmac.c
│   │   ├── npcm_pcs.c
│   │   ├── npcm7xx_emc.c
│   │   ├── opencores_eth.c
│   │   ├── pcnet-pci.c
│   │   ├── pcnet.c
│   │   ├── pcnet.h
│   │   ├── rocker
│   │   │   ├── qmp-norocker.c
│   │   │   ├── rocker_desc.c
│   │   │   ├── rocker_desc.h
│   │   │   ├── rocker_fp.c
│   │   │   ├── rocker_fp.h
│   │   │   ├── rocker_hw.h
│   │   │   ├── rocker_of_dpa.c
│   │   │   ├── rocker_of_dpa.h
│   │   │   ├── rocker_tlv.h
│   │   │   ├── rocker_world.c
│   │   │   ├── rocker_world.h
│   │   │   ├── rocker-hmp-cmds.c
│   │   │   ├── rocker.c
│   │   │   └── rocker.h
│   │   ├── rtl8139.c
│   │   ├── smc91c111.c
│   │   ├── spapr_llan.c
│   │   ├── stellaris_enet.c
│   │   ├── sungem.c
│   │   ├── sunhme.c
│   │   ├── trace-events
│   │   ├── trace.h
│   │   ├── tulip.c
│   │   ├── tulip.h
│   │   ├── vhost_net-stub.c
│   │   ├── vhost_net.c
│   │   ├── virtio-net.c
│   │   ├── vmware_utils.h
│   │   ├── vmxnet_debug.h
│   │   ├── vmxnet3_defs.h
│   │   ├── vmxnet3.c
│   │   ├── vmxnet3.h
│   │   ├── xen_nic.c
│   │   ├── xgmac.c
│   │   ├── xilinx_axienet.c
│   │   └── xilinx_ethlite.c
│   ├── nubus
│   │   ├── Kconfig
│   │   ├── mac-nubus-bridge.c
│   │   ├── meson.build
│   │   ├── nubus-bridge.c
│   │   ├── nubus-bus.c
│   │   ├── nubus-device.c
│   │   ├── nubus-virtio-mmio.c
│   │   ├── trace-events
│   │   └── trace.h
│   ├── nvme
│   │   ├── ctrl.c
│   │   ├── dif.c
│   │   ├── dif.h
│   │   ├── Kconfig
│   │   ├── meson.build
│   │   ├── nguid.c
│   │   ├── ns.c
│   │   ├── nvme.h
│   │   ├── subsys.c
│   │   ├── trace-events
│   │   └── trace.h
│   ├── nvram
│   │   ├── bcm2835_otp.c
│   │   ├── chrp_nvram.c
│   │   ├── ds1225y.c
│   │   ├── eeprom_at24c.c
│   │   ├── eeprom93xx.c
│   │   ├── fw_cfg-acpi.c
│   │   ├── fw_cfg-interface.c
│   │   ├── fw_cfg.c
│   │   ├── Kconfig
│   │   ├── mac_nvram.c
│   │   ├── meson.build
│   │   ├── npcm7xx_otp.c
│   │   ├── nrf51_nvm.c
│   │   ├── spapr_nvram.c
│   │   ├── trace-events
│   │   ├── trace.h
│   │   ├── xlnx-bbram.c
│   │   ├── xlnx-efuse-crc.c
│   │   ├── xlnx-efuse.c
│   │   ├── xlnx-versal-efuse-cache.c
│   │   ├── xlnx-versal-efuse-ctrl.c
│   │   └── xlnx-zynqmp-efuse.c
│   ├── openrisc
│   │   ├── boot.c
│   │   ├── cputimer.c
│   │   ├── Kconfig
│   │   ├── meson.build
│   │   ├── openrisc_sim.c
│   │   └── virt.c
│   ├── pci
│   │   ├── Kconfig
│   │   ├── meson.build
│   │   ├── msi.c
│   │   ├── msix.c
│   │   ├── pci_bridge.c
│   │   ├── pci_host.c
│   │   ├── pci-hmp-cmds.c
│   │   ├── pci-internal.h
│   │   ├── pci-qmp-cmds.c
│   │   ├── pci-stub.c
│   │   ├── pci.c
│   │   ├── pcie_aer.c
│   │   ├── pcie_doe.c
│   │   ├── pcie_host.c
│   │   ├── pcie_port.c
│   │   ├── pcie_sriov.c
│   │   ├── pcie.c
│   │   ├── shpc.c
│   │   ├── slotid_cap.c
│   │   ├── trace-events
│   │   └── trace.h
│   ├── pci-bridge
│   │   ├── cxl_downstream.c
│   │   ├── cxl_root_port.c
│   │   ├── cxl_upstream.c
│   │   ├── gen_pcie_root_port.c
│   │   ├── i82801b11.c
│   │   ├── ioh3420.c
│   │   ├── Kconfig
│   │   ├── meson.build
│   │   ├── pci_bridge_dev.c
│   │   ├── pci_expander_bridge_stubs.c
│   │   ├── pci_expander_bridge.c
│   │   ├── pcie_pci_bridge.c
│   │   ├── pcie_root_port.c
│   │   ├── simba.c
│   │   ├── xio3130_downstream.c
│   │   └── xio3130_upstream.c
│   ├── pci-host
│   │   ├── articia.c
│   │   ├── astro.c
│   │   ├── bonito.c
│   │   ├── designware.c
│   │   ├── dino.c
│   │   ├── fsl_imx8m_phy.c
│   │   ├── gpex-acpi.c
│   │   ├── gpex.c
│   │   ├── grackle.c
│   │   ├── gt64120.c
│   │   ├── i440fx.c
│   │   ├── Kconfig
│   │   ├── meson.build
│   │   ├── mv64361.c
│   │   ├── mv643xx.h
│   │   ├── pam.c
│   │   ├── pnv_phb.c
│   │   ├── pnv_phb.h
│   │   ├── pnv_phb3_msi.c
│   │   ├── pnv_phb3_pbcq.c
│   │   ├── pnv_phb3.c
│   │   ├── pnv_phb4_pec.c
│   │   ├── pnv_phb4.c
│   │   ├── ppc440_pcix.c
│   │   ├── ppc4xx_pci.c
│   │   ├── ppce500.c
│   │   ├── q35.c
│   │   ├── raven.c
│   │   ├── remote.c
│   │   ├── sabre.c
│   │   ├── sh_pci.c
│   │   ├── trace-events
│   │   ├── trace.h
│   │   ├── uninorth.c
│   │   ├── versatile.c
│   │   ├── xen_igd_pt.c
│   │   └── xilinx-pcie.c
│   ├── ppc
│   │   ├── amigaone.c
│   │   ├── e500-ccsr.h
│   │   ├── e500.c
│   │   ├── e500.h
│   │   ├── e500plat.c
│   │   ├── fdt.c
│   │   ├── fw_cfg.c
│   │   ├── Kconfig
│   │   ├── mac_newworld.c
│   │   ├── mac_oldworld.c
│   │   ├── meson.build
│   │   ├── mpc8544_guts.c
│   │   ├── mpc8544ds.c
│   │   ├── pef.c
│   │   ├── pegasos2.c
│   │   ├── pnv_adu.c
│   │   ├── pnv_bmc.c
│   │   ├── pnv_chiptod.c
│   │   ├── pnv_core.c
│   │   ├── pnv_homer.c
│   │   ├── pnv_i2c.c
│   │   ├── pnv_lpc.c
│   │   ├── pnv_n1_chiplet.c
│   │   ├── pnv_nest_pervasive.c
│   │   ├── pnv_occ.c
│   │   ├── pnv_pnor.c
│   │   ├── pnv_psi.c
│   │   ├── pnv_sbe.c
│   │   ├── pnv_xscom.c
│   │   ├── pnv.c
│   │   ├── ppc_booke.c
│   │   ├── ppc.c
│   │   ├── ppc440_bamboo.c
│   │   ├── ppc440_uc.c
│   │   ├── ppc440.h
│   │   ├── ppc4xx_devs.c
│   │   ├── ppc4xx_sdram.c
│   │   ├── ppce500_spin.c
│   │   ├── prep_systemio.c
│   │   ├── prep.c
│   │   ├── rs6000_mc.c
│   │   ├── sam460ex.c
│   │   ├── spapr_caps.c
│   │   ├── spapr_cpu_core.c
│   │   ├── spapr_drc.c
│   │   ├── spapr_events.c
│   │   ├── spapr_hcall.c
│   │   ├── spapr_iommu.c
│   │   ├── spapr_irq.c
│   │   ├── spapr_nested.c
│   │   ├── spapr_numa.c
│   │   ├── spapr_nvdimm.c
│   │   ├── spapr_ovec.c
│   │   ├── spapr_pci_vfio.c
│   │   ├── spapr_pci.c
│   │   ├── spapr_rng.c
│   │   ├── spapr_rtas_ddw.c
│   │   ├── spapr_rtas.c
│   │   ├── spapr_rtc.c
│   │   ├── spapr_tpm_proxy.c
│   │   ├── spapr_vhyp_mmu.c
│   │   ├── spapr_vio.c
│   │   ├── spapr_vof.c
│   │   ├── spapr.c
│   │   ├── trace-events
│   │   ├── trace.h
│   │   ├── virtex_ml507.c
│   │   └── vof.c
│   ├── remote
│   │   ├── iohub.c
│   │   ├── iommu.c
│   │   ├── Kconfig
│   │   ├── machine.c
│   │   ├── memory.c
│   │   ├── meson.build
│   │   ├── message.c
│   │   ├── mpqemu-link.c
│   │   ├── proxy-memory-listener.c
│   │   ├── proxy.c
│   │   ├── remote-obj.c
│   │   ├── trace-events
│   │   ├── trace.h
│   │   ├── vfio-user-obj-stub.c
│   │   └── vfio-user-obj.c
│   ├── riscv
│   │   ├── boot.c
│   │   ├── Kconfig
│   │   ├── meson.build
│   │   ├── microblaze-v-generic.c
│   │   ├── microchip_pfsoc.c
│   │   ├── numa.c
│   │   ├── opentitan.c
│   │   ├── riscv_hart.c
│   │   ├── riscv-iommu-bits.h
│   │   ├── riscv-iommu-hpm.c
│   │   ├── riscv-iommu-hpm.h
│   │   ├── riscv-iommu-pci.c
│   │   ├── riscv-iommu-sys.c
│   │   ├── riscv-iommu.c
│   │   ├── riscv-iommu.h
│   │   ├── shakti_c.c
│   │   ├── sifive_e.c
│   │   ├── sifive_u.c
│   │   ├── spike.c
│   │   ├── trace-events
│   │   ├── trace.h
│   │   ├── virt-acpi-build.c
│   │   └── virt.c
│   ├── rtc
│   │   ├── allwinner-rtc.c
│   │   ├── aspeed_rtc.c
│   │   ├── ds1338.c
│   │   ├── exynos4210_rtc.c
│   │   ├── goldfish_rtc.c
│   │   ├── Kconfig
│   │   ├── ls7a_rtc.c
│   │   ├── m41t80.c
│   │   ├── m48t59-internal.h
│   │   ├── m48t59-isa.c
│   │   ├── m48t59.c
│   │   ├── mc146818rtc.c
│   │   ├── meson.build
│   │   ├── pl031.c
│   │   ├── rs5c372.c
│   │   ├── sun4v-rtc.c
│   │   ├── trace-events
│   │   ├── trace.h
│   │   └── xlnx-zynqmp-rtc.c
│   ├── rx
│   │   ├── Kconfig
│   │   ├── meson.build
│   │   ├── rx-gdbsim.c
│   │   └── rx62n.c
│   ├── s390x
│   │   ├── 3270-ccw.c
│   │   ├── ap-bridge.c
│   │   ├── ap-device.c
│   │   ├── ap-stub.c
│   │   ├── ccw-device.c
│   │   ├── ccw-device.h
│   │   ├── cpu-topology.c
│   │   ├── css-bridge.c
│   │   ├── css.c
│   │   ├── event-facility.c
│   │   ├── ipl.c
│   │   ├── ipl.h
│   │   ├── Kconfig
│   │   ├── meson.build
│   │   ├── s390-ccw.c
│   │   ├── s390-hypercall.c
│   │   ├── s390-hypercall.h
│   │   ├── s390-pci-bus.c
│   │   ├── s390-pci-inst.c
│   │   ├── s390-pci-kvm.c
│   │   ├── s390-pci-vfio.c
│   │   ├── s390-skeys-kvm.c
│   │   ├── s390-skeys.c
│   │   ├── s390-stattrib-kvm.c
│   │   ├── s390-stattrib.c
│   │   ├── s390-virtio-ccw.c
│   │   ├── sclp.c
│   │   ├── sclpcpu.c
│   │   ├── sclpquiesce.c
│   │   ├── tod-kvm.c
│   │   ├── tod-tcg.c
│   │   ├── tod.c
│   │   ├── trace-events
│   │   ├── trace.h
│   │   ├── vhost-scsi-ccw.c
│   │   ├── vhost-user-fs-ccw.c
│   │   ├── vhost-vsock-ccw.c
│   │   ├── virtio-ccw-9p.c
│   │   ├── virtio-ccw-balloon.c
│   │   ├── virtio-ccw-blk.c
│   │   ├── virtio-ccw-crypto.c
│   │   ├── virtio-ccw-gpu.c
│   │   ├── virtio-ccw-input.c
│   │   ├── virtio-ccw-md-stubs.c
│   │   ├── virtio-ccw-md.c
│   │   ├── virtio-ccw-md.h
│   │   ├── virtio-ccw-mem.c
│   │   ├── virtio-ccw-mem.h
│   │   ├── virtio-ccw-net.c
│   │   ├── virtio-ccw-rng.c
│   │   ├── virtio-ccw-scsi.c
│   │   ├── virtio-ccw-serial.c
│   │   ├── virtio-ccw.c
│   │   └── virtio-ccw.h
│   ├── scsi
│   │   ├── emulation.c
│   │   ├── esp-pci.c
│   │   ├── esp.c
│   │   ├── Kconfig
│   │   ├── lsi53c895a.c
│   │   ├── megasas.c
│   │   ├── meson.build
│   │   ├── mfi.h
│   │   ├── mpi.h
│   │   ├── mptconfig.c
│   │   ├── mptendian.c
│   │   ├── mptsas.c
│   │   ├── mptsas.h
│   │   ├── scsi-bus.c
│   │   ├── scsi-disk.c
│   │   ├── scsi-generic.c
│   │   ├── spapr_vscsi.c
│   │   ├── srp.h
│   │   ├── trace-events
│   │   ├── trace.h
│   │   ├── vhost-scsi-common.c
│   │   ├── vhost-scsi.c
│   │   ├── vhost-user-scsi.c
│   │   ├── viosrp.h
│   │   ├── virtio-scsi-dataplane.c
│   │   ├── virtio-scsi.c
│   │   ├── vmw_pvscsi.c
│   │   └── vmw_pvscsi.h
│   ├── sd
│   │   ├── allwinner-sdhost.c
│   │   ├── aspeed_sdhci.c
│   │   ├── bcm2835_sdhost.c
│   │   ├── cadence_sdhci.c
│   │   ├── core.c
│   │   ├── Kconfig
│   │   ├── meson.build
│   │   ├── npcm7xx_sdhci.c
│   │   ├── omap_mmc.c
│   │   ├── pl181.c
│   │   ├── sd.c
│   │   ├── sdhci-internal.h
│   │   ├── sdhci-pci.c
│   │   ├── sdhci.c
│   │   ├── sdmmc-internal.h
│   │   ├── ssi-sd.c
│   │   ├── trace-events
│   │   └── trace.h
│   ├── sensor
│   │   ├── adm1266.c
│   │   ├── adm1272.c
│   │   ├── dps310.c
│   │   ├── emc141x.c
│   │   ├── isl_pmbus_vr.c
│   │   ├── Kconfig
│   │   ├── lsm303dlhc_mag.c
│   │   ├── max31785.c
│   │   ├── max34451.c
│   │   ├── meson.build
│   │   ├── tmp105.c
│   │   ├── tmp421.c
│   │   ├── trace-events
│   │   └── trace.h
│   ├── sh4
│   │   ├── Kconfig
│   │   ├── meson.build
│   │   ├── r2d.c
│   │   ├── sh7750_regnames.c
│   │   ├── sh7750_regnames.h
│   │   ├── sh7750_regs.h
│   │   ├── sh7750.c
│   │   ├── trace-events
│   │   └── trace.h
│   ├── smbios
│   │   ├── Kconfig
│   │   ├── meson.build
│   │   ├── smbios_build.h
│   │   ├── smbios_legacy_stub.c
│   │   ├── smbios_legacy.c
│   │   ├── smbios_type_38-stub.c
│   │   ├── smbios_type_38.c
│   │   ├── smbios-stub.c
│   │   └── smbios.c
│   ├── sparc
│   │   ├── Kconfig
│   │   ├── leon3.c
│   │   ├── meson.build
│   │   ├── sun4m_iommu.c
│   │   ├── sun4m.c
│   │   ├── trace-events
│   │   └── trace.h
│   ├── sparc64
│   │   ├── Kconfig
│   │   ├── meson.build
│   │   ├── niagara.c
│   │   ├── sparc64.c
│   │   ├── sun4u_iommu.c
│   │   ├── sun4u.c
│   │   ├── trace-events
│   │   └── trace.h
│   ├── ssi
│   │   ├── allwinner-a10-spi.c
│   │   ├── aspeed_smc.c
│   │   ├── bcm2835_spi.c
│   │   ├── ibex_spi_host.c
│   │   ├── imx_spi.c
│   │   ├── Kconfig
│   │   ├── meson.build
│   │   ├── mss-spi.c
│   │   ├── npcm_pspi.c
│   │   ├── npcm7xx_fiu.c
│   │   ├── pl022.c
│   │   ├── pnv_spi.c
│   │   ├── sifive_spi.c
│   │   ├── ssi.c
│   │   ├── stm32f2xx_spi.c
│   │   ├── trace-events
│   │   ├── trace.h
│   │   ├── xilinx_spi.c
│   │   ├── xilinx_spips.c
│   │   └── xlnx-versal-ospi.c
│   ├── timer
│   │   ├── a9gtimer.c
│   │   ├── allwinner-a10-pit.c
│   │   ├── arm_mptimer.c
│   │   ├── arm_timer.c
│   │   ├── armv7m_systick.c
│   │   ├── aspeed_timer.c
│   │   ├── avr_timer16.c
│   │   ├── bcm2835_systmr.c
│   │   ├── cadence_ttc.c
│   │   ├── cmsdk-apb-dualtimer.c
│   │   ├── cmsdk-apb-timer.c
│   │   ├── digic-timer.c
│   │   ├── exynos4210_mct.c
│   │   ├── exynos4210_pwm.c
│   │   ├── grlib_gptimer.c
│   │   ├── hpet.c
│   │   ├── i8254_common.c
│   │   ├── i8254.c
│   │   ├── ibex_timer.c
│   │   ├── imx_epit.c
│   │   ├── imx_gpt.c
│   │   ├── Kconfig
│   │   ├── meson.build
│   │   ├── mips_gictimer.c
│   │   ├── mss-timer.c
│   │   ├── npcm7xx_timer.c
│   │   ├── nrf51_timer.c
│   │   ├── pxa2xx_timer.c
│   │   ├── renesas_cmt.c
│   │   ├── renesas_tmr.c
│   │   ├── sh_timer.c
│   │   ├── sifive_pwm.c
│   │   ├── slavio_timer.c
│   │   ├── sse-counter.c
│   │   ├── sse-timer.c
│   │   ├── stellaris-gptm.c
│   │   ├── stm32f2xx_timer.c
│   │   ├── trace-events
│   │   ├── trace.h
│   │   └── xilinx_timer.c
│   ├── tpm
│   │   ├── Kconfig
│   │   ├── meson.build
│   │   ├── tpm_crb.c
│   │   ├── tpm_ppi.c
│   │   ├── tpm_ppi.h
│   │   ├── tpm_prop.h
│   │   ├── tpm_spapr.c
│   │   ├── tpm_tis_common.c
│   │   ├── tpm_tis_i2c.c
│   │   ├── tpm_tis_isa.c
│   │   ├── tpm_tis_sysbus.c
│   │   ├── tpm_tis.h
│   │   ├── trace-events
│   │   └── trace.h
│   ├── tricore
│   │   ├── Kconfig
│   │   ├── meson.build
│   │   ├── tc27x_soc.c
│   │   ├── triboard.c
│   │   ├── tricore_testboard.c
│   │   └── tricore_testdevice.c
│   ├── uefi
│   │   ├── hardware-info.c
│   │   ├── Kconfig
│   │   ├── LIMITATIONS.md
│   │   ├── meson.build
│   │   ├── trace-events
│   │   ├── var-service-auth.c
│   │   ├── var-service-core.c
│   │   ├── var-service-guid.c
│   │   ├── var-service-json.c
│   │   ├── var-service-pkcs7-stub.c
│   │   ├── var-service-pkcs7.c
│   │   ├── var-service-policy.c
│   │   ├── var-service-siglist.c
│   │   ├── var-service-sysbus.c
│   │   ├── var-service-utils.c
│   │   └── var-service-vars.c
│   ├── ufs
│   │   ├── Kconfig
│   │   ├── lu.c
│   │   ├── meson.build
│   │   ├── trace-events
│   │   ├── trace.h
│   │   ├── ufs.c
│   │   └── ufs.h
│   ├── usb
│   │   ├── bus-stub.c
│   │   ├── bus.c
│   │   ├── canokey.c
│   │   ├── canokey.h
│   │   ├── ccid-card-emulated.c
│   │   ├── ccid-card-passthru.c
│   │   ├── ccid.h
│   │   ├── chipidea.c
│   │   ├── combined-packet.c
│   │   ├── core.c
│   │   ├── desc-msos.c
│   │   ├── desc.c
│   │   ├── desc.h
│   │   ├── dev-audio.c
│   │   ├── dev-hid.c
│   │   ├── dev-hub.c
│   │   ├── dev-mtp.c
│   │   ├── dev-network.c
│   │   ├── dev-serial.c
│   │   ├── dev-smartcard-reader.c
│   │   ├── dev-storage-bot.c
│   │   ├── dev-storage-classic.c
│   │   ├── dev-storage.c
│   │   ├── dev-uas.c
│   │   ├── dev-wacom.c
│   │   ├── hcd-dwc2.c
│   │   ├── hcd-dwc2.h
│   │   ├── hcd-dwc3.c
│   │   ├── hcd-ehci-pci.c
│   │   ├── hcd-ehci-sysbus.c
│   │   ├── hcd-ehci.c
│   │   ├── hcd-ehci.h
│   │   ├── hcd-ohci-pci.c
│   │   ├── hcd-ohci-sysbus.c
│   │   ├── hcd-ohci.c
│   │   ├── hcd-ohci.h
│   │   ├── hcd-uhci.c
│   │   ├── hcd-uhci.h
│   │   ├── hcd-xhci-nec.c
│   │   ├── hcd-xhci-pci.c
│   │   ├── hcd-xhci-pci.h
│   │   ├── hcd-xhci-sysbus.c
│   │   ├── hcd-xhci-sysbus.h
│   │   ├── hcd-xhci.c
│   │   ├── hcd-xhci.h
│   │   ├── host-libusb.c
│   │   ├── imx-usb-phy.c
│   │   ├── Kconfig
│   │   ├── libhw.c
│   │   ├── meson.build
│   │   ├── pcap.c
│   │   ├── quirks-ftdi-ids.h
│   │   ├── quirks-pl2303-ids.h
│   │   ├── quirks.c
│   │   ├── quirks.h
│   │   ├── redirect.c
│   │   ├── trace-events
│   │   ├── trace.h
│   │   ├── u2f-emulated.c
│   │   ├── u2f-passthru.c
│   │   ├── u2f.c
│   │   ├── u2f.h
│   │   ├── vt82c686-uhci-pci.c
│   │   ├── xen-usb.c
│   │   ├── xlnx-usb-subsystem.c
│   │   └── xlnx-versal-usb2-ctrl-regs.c
│   ├── vfio
│   │   ├── amd-xgbe.c
│   │   ├── ap.c
│   │   ├── calxeda-xgmac.c
│   │   ├── ccw.c
│   │   ├── container-base.c
│   │   ├── container.c
│   │   ├── cpr-legacy.c
│   │   ├── cpr.c
│   │   ├── device.c
│   │   ├── display.c
│   │   ├── helpers.c
│   │   ├── igd.c
│   │   ├── iommufd.c
│   │   ├── Kconfig
│   │   ├── listener.c
│   │   ├── meson.build
│   │   ├── migration-multifd.c
│   │   ├── migration-multifd.h
│   │   ├── migration.c
│   │   ├── pci-quirks.c
│   │   ├── pci-quirks.h
│   │   ├── pci.c
│   │   ├── pci.h
│   │   ├── platform.c
│   │   ├── region.c
│   │   ├── spapr.c
│   │   ├── trace-events
│   │   ├── trace.h
│   │   ├── vfio-display.h
│   │   ├── vfio-helpers.h
│   │   ├── vfio-iommufd.h
│   │   ├── vfio-listener.h
│   │   └── vfio-migration-internal.h
│   ├── virtio
│   │   ├── cbor-helpers.c
│   │   ├── iothread-vq-mapping.c
│   │   ├── Kconfig
│   │   ├── meson.build
│   │   ├── trace-events
│   │   ├── trace.h
│   │   ├── vdpa-dev-pci.c
│   │   ├── vdpa-dev.c
│   │   ├── vhost-backend.c
│   │   ├── vhost-iova-tree.c
│   │   ├── vhost-iova-tree.h
│   │   ├── vhost-scsi-pci.c
│   │   ├── vhost-shadow-virtqueue.c
│   │   ├── vhost-shadow-virtqueue.h
│   │   ├── vhost-stub.c
│   │   ├── vhost-user-base.c
│   │   ├── vhost-user-blk-pci.c
│   │   ├── vhost-user-device-pci.c
│   │   ├── vhost-user-device.c
│   │   ├── vhost-user-fs-pci.c
│   │   ├── vhost-user-fs.c
│   │   ├── vhost-user-gpio-pci.c
│   │   ├── vhost-user-gpio.c
│   │   ├── vhost-user-i2c-pci.c
│   │   ├── vhost-user-i2c.c
│   │   ├── vhost-user-input-pci.c
│   │   ├── vhost-user-input.c
│   │   ├── vhost-user-rng-pci.c
│   │   ├── vhost-user-rng.c
│   │   ├── vhost-user-scmi-pci.c
│   │   ├── vhost-user-scmi.c
│   │   ├── vhost-user-scsi-pci.c
│   │   ├── vhost-user-snd-pci.c
│   │   ├── vhost-user-snd.c
│   │   ├── vhost-user-vsock-pci.c
│   │   ├── vhost-user-vsock.c
│   │   ├── vhost-user.c
│   │   ├── vhost-vdpa.c
│   │   ├── vhost-vsock-common.c
│   │   ├── vhost-vsock-pci.c
│   │   ├── vhost-vsock.c
│   │   ├── vhost.c
│   │   ├── virtio-9p-pci.c
│   │   ├── virtio-acpi.c
│   │   ├── virtio-balloon-pci.c
│   │   ├── virtio-balloon.c
│   │   ├── virtio-blk-pci.c
│   │   ├── virtio-bus.c
│   │   ├── virtio-config-io.c
│   │   ├── virtio-crypto-pci.c
│   │   ├── virtio-crypto.c
│   │   ├── virtio-hmp-cmds.c
│   │   ├── virtio-input-host-pci.c
│   │   ├── virtio-input-pci.c
│   │   ├── virtio-iommu-pci.c
│   │   ├── virtio-iommu.c
│   │   ├── virtio-md-pci.c
│   │   ├── virtio-md-stubs.c
│   │   ├── virtio-mem-pci.c
│   │   ├── virtio-mem-pci.h
│   │   ├── virtio-mem.c
│   │   ├── virtio-mmio.c
│   │   ├── virtio-net-pci.c
│   │   ├── virtio-nsm-pci.c
│   │   ├── virtio-nsm.c
│   │   ├── virtio-pci.c
│   │   ├── virtio-pmem-pci.c
│   │   ├── virtio-pmem-pci.h
│   │   ├── virtio-pmem.c
│   │   ├── virtio-qmp.c
│   │   ├── virtio-qmp.h
│   │   ├── virtio-rng-pci.c
│   │   ├── virtio-rng.c
│   │   ├── virtio-scsi-pci.c
│   │   ├── virtio-serial-pci.c
│   │   ├── virtio-stub.c
│   │   └── virtio.c
│   ├── vmapple
│   │   ├── aes.c
│   │   ├── bdif.c
│   │   ├── cfg.c
│   │   ├── Kconfig
│   │   ├── meson.build
│   │   ├── trace-events
│   │   ├── trace.h
│   │   ├── virtio-blk.c
│   │   └── vmapple.c
│   ├── watchdog
│   │   ├── allwinner-wdt.c
│   │   ├── cmsdk-apb-watchdog.c
│   │   ├── Kconfig
│   │   ├── meson.build
│   │   ├── sbsa_gwdt.c
│   │   ├── spapr_watchdog.c
│   │   ├── trace-events
│   │   ├── trace.h
│   │   ├── watchdog.c
│   │   ├── wdt_aspeed.c
│   │   ├── wdt_diag288.c
│   │   ├── wdt_i6300esb.c
│   │   ├── wdt_ib700.c
│   │   └── wdt_imx2.c
│   ├── xen
│   │   ├── Kconfig
│   │   ├── meson.build
│   │   ├── trace-events
│   │   ├── trace.h
│   │   ├── xen_devconfig.c
│   │   ├── xen_pt_config_init.c
│   │   ├── xen_pt_graphics.c
│   │   ├── xen_pt_load_rom.c
│   │   ├── xen_pt_msi.c
│   │   ├── xen_pt_stub.c
│   │   ├── xen_pt.c
│   │   ├── xen_pt.h
│   │   ├── xen_pvdev.c
│   │   ├── xen_stubs.c
│   │   ├── xen-backend.c
│   │   ├── xen-bus-helper.c
│   │   ├── xen-bus.c
│   │   ├── xen-host-pci-device.c
│   │   ├── xen-host-pci-device.h
│   │   ├── xen-hvm-common.c
│   │   ├── xen-legacy-backend.c
│   │   ├── xen-mapcache.c
│   │   ├── xen-operations.c
│   │   └── xen-pvh-common.c
│   ├── xenpv
│   │   ├── meson.build
│   │   └── xen_machine_pv.c
│   └── xtensa
│       ├── bootparam.h
│       ├── Kconfig
│       ├── meson.build
│       ├── mx_pic.c
│       ├── pic_cpu.c
│       ├── sim.c
│       ├── virt.c
│       ├── xtensa_memory.c
│       ├── xtensa_memory.h
│       ├── xtensa_sim.h
│       └── xtfpga.c
├── include
│   ├── accel
│   │   ├── accel-cpu-target.h
│   │   ├── accel-cpu.h
│   │   └── tcg
│   │       ├── cpu-ldst-common.h
│   │       ├── cpu-ldst.h
│   │       ├── cpu-mmu-index.h
│   │       ├── cpu-ops.h
│   │       ├── getpc.h
│   │       ├── helper-retaddr.h
│   │       ├── iommu.h
│   │       ├── probe.h
│   │       └── tb-cpu-state.h
│   ├── authz
│   │   ├── base.h
│   │   ├── list.h
│   │   ├── listfile.h
│   │   ├── pamacct.h
│   │   └── simple.h
│   ├── block
│   │   ├── accounting.h
│   │   ├── aio_task.h
│   │   ├── aio-wait.h
│   │   ├── aio.h
│   │   ├── block_backup.h
│   │   ├── block_int-common.h
│   │   ├── block_int-global-state.h
│   │   ├── block_int-io.h
│   │   ├── block_int.h
│   │   ├── block-common.h
│   │   ├── block-copy.h
│   │   ├── block-global-state.h
│   │   ├── block-hmp-cmds.h
│   │   ├── block-io.h
│   │   ├── block.h
│   │   ├── blockjob_int.h
│   │   ├── blockjob.h
│   │   ├── dirty-bitmap.h
│   │   ├── export.h
│   │   ├── fuse.h
│   │   ├── graph-lock.h
│   │   ├── nbd.h
│   │   ├── nvme.h
│   │   ├── qapi.h
│   │   ├── qdict.h
│   │   ├── raw-aio.h
│   │   ├── replication.h
│   │   ├── reqlist.h
│   │   ├── snapshot.h
│   │   ├── thread-pool.h
│   │   ├── throttle-groups.h
│   │   ├── ufs.h
│   │   └── write-threshold.h
│   ├── chardev
│   │   ├── char-fd.h
│   │   ├── char-fe.h
│   │   ├── char-io.h
│   │   ├── char-parallel.h
│   │   ├── char-serial.h
│   │   ├── char-socket.h
│   │   ├── char-win-stdio.h
│   │   ├── char-win.h
│   │   ├── char.h
│   │   └── spice.h
│   ├── crypto
│   │   ├── aes-round.h
│   │   ├── aes.h
│   │   ├── afsplit.h
│   │   ├── akcipher.h
│   │   ├── block.h
│   │   ├── cipher.h
│   │   ├── clmul.h
│   │   ├── desrfb.h
│   │   ├── hash.h
│   │   ├── hmac.h
│   │   ├── init.h
│   │   ├── ivgen.h
│   │   ├── pbkdf.h
│   │   ├── random.h
│   │   ├── secret_common.h
│   │   ├── secret_keyring.h
│   │   ├── secret.h
│   │   ├── sm4.h
│   │   ├── tls-cipher-suites.h
│   │   ├── tlscreds.h
│   │   ├── tlscredsanon.h
│   │   ├── tlscredspsk.h
│   │   ├── tlscredsx509.h
│   │   ├── tlssession.h
│   │   ├── x509-utils.h
│   │   └── xts.h
│   ├── disas
│   │   ├── capstone.h
│   │   ├── dis-asm.h
│   │   └── disas.h
│   ├── elf.h
│   ├── exec
│   │   ├── abi_ptr.h
│   │   ├── breakpoint.h
│   │   ├── cpu-common.h
│   │   ├── cpu-defs.h
│   │   ├── cpu-interrupt.h
│   │   ├── cputlb.h
│   │   ├── gdbstub.h
│   │   ├── helper-gen-common.h
│   │   ├── helper-gen.h
│   │   ├── helper-gen.h.inc
│   │   ├── helper-head.h.inc
│   │   ├── helper-info.c.inc
│   │   ├── helper-proto-common.h
│   │   ├── helper-proto.h
│   │   ├── helper-proto.h.inc
│   │   ├── hwaddr.h
│   │   ├── icount.h
│   │   ├── log.h
│   │   ├── memattrs.h
│   │   ├── memop.h
│   │   ├── memopidx.h
│   │   ├── memory_ldst_cached.h.inc
│   │   ├── memory_ldst_phys.h.inc
│   │   ├── memory_ldst.h.inc
│   │   ├── mmap-lock.h
│   │   ├── mmu-access-type.h
│   │   ├── page-protection.h
│   │   ├── page-vary.h
│   │   ├── plugin-gen.h
│   │   ├── poison.h
│   │   ├── ramlist.h
│   │   ├── replay-core.h
│   │   ├── target_long.h
│   │   ├── target_page.h
│   │   ├── tb-flush.h
│   │   ├── tlb-common.h
│   │   ├── tlb-flags.h
│   │   ├── translation-block.h
│   │   ├── translator.h
│   │   ├── tswap.h
│   │   ├── vaddr.h
│   │   └── watchpoint.h
│   ├── fpu
│   │   ├── softfloat-helpers.h
│   │   ├── softfloat-macros.h
│   │   ├── softfloat-types.h
│   │   └── softfloat.h
│   ├── gdbstub
│   │   ├── commands.h
│   │   ├── enums.h
│   │   ├── helpers.h
│   │   ├── syscalls.h
│   │   └── user.h
│   ├── glib-compat.h
│   ├── hw
│   │   ├── acpi
│   │   │   ├── acpi_aml_interface.h
│   │   │   ├── acpi_dev_interface.h
│   │   │   ├── acpi-defs.h
│   │   │   ├── acpi.h
│   │   │   ├── aml-build.h
│   │   │   ├── bios-linker-loader.h
│   │   │   ├── cpu_hotplug.h
│   │   │   ├── cpu.h
│   │   │   ├── cxl.h
│   │   │   ├── erst.h
│   │   │   ├── generic_event_device.h
│   │   │   ├── ghes.h
│   │   │   ├── ich9_tco.h
│   │   │   ├── ich9_timer.h
│   │   │   ├── ich9.h
│   │   │   ├── ipmi.h
│   │   │   ├── memory_hotplug.h
│   │   │   ├── pc-hotplug.h
│   │   │   ├── pci.h
│   │   │   ├── pcihp.h
│   │   │   ├── piix4.h
│   │   │   ├── tpm.h
│   │   │   ├── utils.h
│   │   │   ├── vmclock.h
│   │   │   └── vmgenid.h
│   │   ├── adc
│   │   │   ├── aspeed_adc.h
│   │   │   ├── npcm7xx_adc.h
│   │   │   ├── stm32f2xx_adc.h
│   │   │   └── zynq-xadc.h
│   │   ├── arm
│   │   │   ├── allwinner-a10.h
│   │   │   ├── allwinner-h3.h
│   │   │   ├── allwinner-r40.h
│   │   │   ├── armsse-version.h
│   │   │   ├── armsse.h
│   │   │   ├── armv7m.h
│   │   │   ├── aspeed_soc.h
│   │   │   ├── aspeed.h
│   │   │   ├── bcm2835_peripherals.h
│   │   │   ├── bcm2836.h
│   │   │   ├── bcm2838_peripherals.h
│   │   │   ├── bcm2838.h
│   │   │   ├── boot.h
│   │   │   ├── bsa.h
│   │   │   ├── digic.h
│   │   │   ├── exynos4210.h
│   │   │   ├── fdt.h
│   │   │   ├── fsl-imx25.h
│   │   │   ├── fsl-imx31.h
│   │   │   ├── fsl-imx6.h
│   │   │   ├── fsl-imx6ul.h
│   │   │   ├── fsl-imx7.h
│   │   │   ├── fsl-imx8mp.h
│   │   │   ├── linux-boot-if.h
│   │   │   ├── msf2-soc.h
│   │   │   ├── npcm7xx.h
│   │   │   ├── npcm8xx.h
│   │   │   ├── nrf51_soc.h
│   │   │   ├── nrf51.h
│   │   │   ├── omap.h
│   │   │   ├── primecell.h
│   │   │   ├── raspberrypi-fw-defs.h
│   │   │   ├── raspi_platform.h
│   │   │   ├── sharpsl.h
│   │   │   ├── smmu-common.h
│   │   │   ├── smmuv3.h
│   │   │   ├── soc_dma.h
│   │   │   ├── stm32f100_soc.h
│   │   │   ├── stm32f205_soc.h
│   │   │   ├── stm32f405_soc.h
│   │   │   ├── stm32l4x5_soc.h
│   │   │   ├── virt.h
│   │   │   ├── xen_arch_hvm.h
│   │   │   ├── xlnx-versal.h
│   │   │   └── xlnx-zynqmp.h
│   │   ├── audio
│   │   │   ├── asc.h
│   │   │   ├── pcspk.h
│   │   │   ├── soundhw.h
│   │   │   ├── virtio-snd.h
│   │   │   └── wm8750.h
│   │   ├── block
│   │   │   ├── block.h
│   │   │   ├── fdc.h
│   │   │   ├── flash.h
│   │   │   └── swim.h
│   │   ├── boards.h
│   │   ├── char
│   │   │   ├── avr_usart.h
│   │   │   ├── bcm2835_aux.h
│   │   │   ├── cadence_uart.h
│   │   │   ├── cmsdk-apb-uart.h
│   │   │   ├── digic-uart.h
│   │   │   ├── escc.h
│   │   │   ├── goldfish_tty.h
│   │   │   ├── grlib_uart.h
│   │   │   ├── ibex_uart.h
│   │   │   ├── imx_serial.h
│   │   │   ├── mchp_pfsoc_mmuart.h
│   │   │   ├── nrf51_uart.h
│   │   │   ├── parallel-isa.h
│   │   │   ├── parallel.h
│   │   │   ├── pl011.h
│   │   │   ├── renesas_sci.h
│   │   │   ├── riscv_htif.h
│   │   │   ├── serial-isa.h
│   │   │   ├── serial-mm.h
│   │   │   ├── serial.h
│   │   │   ├── shakti_uart.h
│   │   │   ├── sifive_uart.h
│   │   │   ├── stm32f2xx_usart.h
│   │   │   ├── stm32l4x5_usart.h
│   │   │   └── xilinx_uartlite.h
│   │   ├── clock.h
│   │   ├── core
│   │   │   ├── cpu.h
│   │   │   ├── generic-loader.h
│   │   │   ├── resetcontainer.h
│   │   │   ├── split-irq.h
│   │   │   ├── sysbus-fdt.h
│   │   │   └── sysemu-cpu-ops.h
│   │   ├── cpu
│   │   │   ├── a15mpcore.h
│   │   │   ├── a9mpcore.h
│   │   │   ├── arm11mpcore.h
│   │   │   ├── cluster.h
│   │   │   └── core.h
│   │   ├── cxl
│   │   │   ├── cxl_cdat.h
│   │   │   ├── cxl_component.h
│   │   │   ├── cxl_device.h
│   │   │   ├── cxl_events.h
│   │   │   ├── cxl_host.h
│   │   │   ├── cxl_mailbox.h
│   │   │   ├── cxl_pci.h
│   │   │   └── cxl.h
│   │   ├── display
│   │   │   ├── bcm2835_fb.h
│   │   │   ├── bochs-vbe.h
│   │   │   ├── dm163.h
│   │   │   ├── dpcd.h
│   │   │   ├── edid.h
│   │   │   ├── i2c-ddc.h
│   │   │   ├── macfb.h
│   │   │   ├── ramfb.h
│   │   │   ├── vga.h
│   │   │   └── xlnx_dp.h
│   │   ├── dma
│   │   │   ├── bcm2835_dma.h
│   │   │   ├── i8257.h
│   │   │   ├── pl080.h
│   │   │   ├── sifive_pdma.h
│   │   │   ├── xlnx_csu_dma.h
│   │   │   ├── xlnx_dpdma.h
│   │   │   ├── xlnx-zdma.h
│   │   │   └── xlnx-zynq-devcfg.h
│   │   ├── elf_ops.h.inc
│   │   ├── firmware
│   │   │   └── smbios.h
│   │   ├── fsi
│   │   │   ├── aspeed_apb2opb.h
│   │   │   ├── cfam.h
│   │   │   ├── fsi-master.h
│   │   │   ├── fsi.h
│   │   │   └── lbus.h
│   │   ├── fw-path-provider.h
│   │   ├── gpio
│   │   │   ├── aspeed_gpio.h
│   │   │   ├── bcm2835_gpio.h
│   │   │   ├── bcm2838_gpio.h
│   │   │   ├── imx_gpio.h
│   │   │   ├── npcm7xx_gpio.h
│   │   │   ├── nrf51_gpio.h
│   │   │   ├── pca9552_regs.h
│   │   │   ├── pca9552.h
│   │   │   ├── pca9554_regs.h
│   │   │   ├── pca9554.h
│   │   │   ├── pcf8574.h
│   │   │   ├── sifive_gpio.h
│   │   │   └── stm32l4x5_gpio.h
│   │   ├── hotplug.h
│   │   ├── hw.h
│   │   ├── hyperv
│   │   │   ├── dynmem-proto.h
│   │   │   ├── hv-balloon.h
│   │   │   ├── hyperv-proto.h
│   │   │   ├── hyperv.h
│   │   │   ├── vmbus-bridge.h
│   │   │   ├── vmbus-proto.h
│   │   │   └── vmbus.h
│   │   ├── i2c
│   │   │   ├── allwinner-i2c.h
│   │   │   ├── arm_sbcon_i2c.h
│   │   │   ├── aspeed_i2c.h
│   │   │   ├── bcm2835_i2c.h
│   │   │   ├── bitbang_i2c.h
│   │   │   ├── i2c_mux_pca954x.h
│   │   │   ├── i2c.h
│   │   │   ├── imx_i2c.h
│   │   │   ├── microbit_i2c.h
│   │   │   ├── npcm7xx_smbus.h
│   │   │   ├── pm_smbus.h
│   │   │   ├── pmbus_device.h
│   │   │   ├── pnv_i2c_regs.h
│   │   │   ├── ppc4xx_i2c.h
│   │   │   ├── smbus_eeprom.h
│   │   │   ├── smbus_master.h
│   │   │   └── smbus_slave.h
│   │   ├── i386
│   │   │   ├── apic_internal.h
│   │   │   ├── apic-msidef.h
│   │   │   ├── apic.h
│   │   │   ├── hostmem-epc.h
│   │   │   ├── intel_iommu.h
│   │   │   ├── microvm.h
│   │   │   ├── nitro_enclave.h
│   │   │   ├── pc.h
│   │   │   ├── sgx-epc.h
│   │   │   ├── tdvf.h
│   │   │   ├── topology.h
│   │   │   ├── vmport.h
│   │   │   ├── x86-iommu.h
│   │   │   ├── x86.h
│   │   │   └── xen_arch_hvm.h
│   │   ├── ide
│   │   │   ├── ahci-pci.h
│   │   │   ├── ahci-sysbus.h
│   │   │   ├── ahci.h
│   │   │   ├── ide-bus.h
│   │   │   ├── ide-dev.h
│   │   │   ├── ide-dma.h
│   │   │   ├── isa.h
│   │   │   ├── mmio.h
│   │   │   ├── pci.h
│   │   │   └── piix.h
│   │   ├── input
│   │   │   ├── adb-keys.h
│   │   │   ├── adb.h
│   │   │   ├── hid.h
│   │   │   ├── i8042.h
│   │   │   ├── lasips2.h
│   │   │   ├── pl050.h
│   │   │   ├── ps2.h
│   │   │   └── stellaris_gamepad.h
│   │   ├── intc
│   │   │   ├── allwinner-a10-pic.h
│   │   │   ├── arm_gic_common.h
│   │   │   ├── arm_gic.h
│   │   │   ├── arm_gicv3_common.h
│   │   │   ├── arm_gicv3_its_common.h
│   │   │   ├── arm_gicv3.h
│   │   │   ├── armv7m_nvic.h
│   │   │   ├── aspeed_intc.h
│   │   │   ├── aspeed_vic.h
│   │   │   ├── bcm2835_ic.h
│   │   │   ├── bcm2836_control.h
│   │   │   ├── exynos4210_combiner.h
│   │   │   ├── exynos4210_gic.h
│   │   │   ├── goldfish_pic.h
│   │   │   ├── grlib_irqmp.h
│   │   │   ├── heathrow_pic.h
│   │   │   ├── i8259.h
│   │   │   ├── imx_avic.h
│   │   │   ├── imx_gpcv2.h
│   │   │   ├── intc.h
│   │   │   ├── ioapic.h
│   │   │   ├── kvm_irqcount.h
│   │   │   ├── loongarch_extioi_common.h
│   │   │   ├── loongarch_extioi.h
│   │   │   ├── loongarch_ipi.h
│   │   │   ├── loongarch_pch_msi.h
│   │   │   ├── loongarch_pch_pic.h
│   │   │   ├── loongarch_pic_common.h
│   │   │   ├── loongson_ipi_common.h
│   │   │   ├── loongson_ipi.h
│   │   │   ├── loongson_liointc.h
│   │   │   ├── m68k_irqc.h
│   │   │   ├── mips_gic.h
│   │   │   ├── ppc-uic.h
│   │   │   ├── realview_gic.h
│   │   │   ├── riscv_aclint.h
│   │   │   ├── riscv_aplic.h
│   │   │   ├── riscv_imsic.h
│   │   │   ├── rx_icu.h
│   │   │   ├── sifive_plic.h
│   │   │   ├── xlnx-pmu-iomod-intc.h
│   │   │   └── xlnx-zynqmp-ipi.h
│   │   ├── ipack
│   │   │   └── ipack.h
│   │   ├── ipmi
│   │   │   ├── ipmi_bt.h
│   │   │   ├── ipmi_kcs.h
│   │   │   └── ipmi.h
│   │   ├── irq.h
│   │   ├── isa
│   │   │   ├── apm.h
│   │   │   ├── i8259_internal.h
│   │   │   ├── isa.h
│   │   │   ├── pc87312.h
│   │   │   ├── superio.h
│   │   │   └── vt82c686.h
│   │   ├── loader-fit.h
│   │   ├── loader.h
│   │   ├── loongarch
│   │   │   ├── boot.h
│   │   │   └── virt.h
│   │   ├── m68k
│   │   │   ├── mcf_fec.h
│   │   │   ├── mcf.h
│   │   │   ├── next-cube.h
│   │   │   ├── q800-glue.h
│   │   │   └── q800.h
│   │   ├── mem
│   │   │   ├── memory-device.h
│   │   │   ├── npcm7xx_mc.h
│   │   │   ├── nvdimm.h
│   │   │   ├── pc-dimm.h
│   │   │   └── sparse-mem.h
│   │   ├── mips
│   │   │   ├── bootloader.h
│   │   │   ├── cps.h
│   │   │   └── mips.h
│   │   ├── misc
│   │   │   ├── a9scu.h
│   │   │   ├── allwinner-a10-ccm.h
│   │   │   ├── allwinner-a10-dramc.h
│   │   │   ├── allwinner-cpucfg.h
│   │   │   ├── allwinner-h3-ccu.h
│   │   │   ├── allwinner-h3-dramc.h
│   │   │   ├── allwinner-h3-sysctrl.h
│   │   │   ├── allwinner-r40-ccu.h
│   │   │   ├── allwinner-r40-dramc.h
│   │   │   ├── allwinner-sid.h
│   │   │   ├── allwinner-sramc.h
│   │   │   ├── arm_integrator_debug.h
│   │   │   ├── arm11scu.h
│   │   │   ├── armsse-cpu-pwrctrl.h
│   │   │   ├── armsse-cpuid.h
│   │   │   ├── armsse-mhu.h
│   │   │   ├── armv7m_ras.h
│   │   │   ├── aspeed_hace.h
│   │   │   ├── aspeed_i3c.h
│   │   │   ├── aspeed_lpc.h
│   │   │   ├── aspeed_peci.h
│   │   │   ├── aspeed_sbc.h
│   │   │   ├── aspeed_scu.h
│   │   │   ├── aspeed_sdmc.h
│   │   │   ├── aspeed_sli.h
│   │   │   ├── aspeed_xdma.h
│   │   │   ├── auxbus.h
│   │   │   ├── avr_power.h
│   │   │   ├── bcm2835_cprman_internals.h
│   │   │   ├── bcm2835_cprman.h
│   │   │   ├── bcm2835_mbox_defs.h
│   │   │   ├── bcm2835_mbox.h
│   │   │   ├── bcm2835_mphi.h
│   │   │   ├── bcm2835_powermgt.h
│   │   │   ├── bcm2835_property.h
│   │   │   ├── bcm2835_rng.h
│   │   │   ├── bcm2835_thermal.h
│   │   │   ├── djmemc.h
│   │   │   ├── empty_slot.h
│   │   │   ├── grlib_ahb_apb_pnp.h
│   │   │   ├── imx_ccm.h
│   │   │   ├── imx_rngc.h
│   │   │   ├── imx25_ccm.h
│   │   │   ├── imx31_ccm.h
│   │   │   ├── imx6_ccm.h
│   │   │   ├── imx6_src.h
│   │   │   ├── imx6ul_ccm.h
│   │   │   ├── imx7_ccm.h
│   │   │   ├── imx7_gpr.h
│   │   │   ├── imx7_snvs.h
│   │   │   ├── imx7_src.h
│   │   │   ├── imx8mp_analog.h
│   │   │   ├── imx8mp_ccm.h
│   │   │   ├── iosb.h
│   │   │   ├── iotkit-secctl.h
│   │   │   ├── iotkit-sysctl.h
│   │   │   ├── iotkit-sysinfo.h
│   │   │   ├── ivshmem-flat.h
│   │   │   ├── ivshmem.h
│   │   │   ├── lasi.h
│   │   │   ├── led.h
│   │   │   ├── mac_via.h
│   │   │   ├── macio
│   │   │   │   ├── cuda.h
│   │   │   │   ├── gpio.h
│   │   │   │   ├── macio.h
│   │   │   │   └── pmu.h
│   │   │   ├── mchp_pfsoc_dmc.h
│   │   │   ├── mchp_pfsoc_ioscb.h
│   │   │   ├── mchp_pfsoc_sysreg.h
│   │   │   ├── mips_cmgcr.h
│   │   │   ├── mips_cpc.h
│   │   │   ├── mips_itu.h
│   │   │   ├── mos6522.h
│   │   │   ├── mps2-fpgaio.h
│   │   │   ├── mps2-scc.h
│   │   │   ├── msf2-sysreg.h
│   │   │   ├── npcm_clk.h
│   │   │   ├── npcm_gcr.h
│   │   │   ├── npcm7xx_mft.h
│   │   │   ├── npcm7xx_pwm.h
│   │   │   ├── npcm7xx_rng.h
│   │   │   ├── nrf51_rng.h
│   │   │   ├── pvpanic.h
│   │   │   ├── sifive_e_aon.h
│   │   │   ├── sifive_e_prci.h
│   │   │   ├── sifive_test.h
│   │   │   ├── sifive_u_otp.h
│   │   │   ├── sifive_u_prci.h
│   │   │   ├── stm32_rcc.h
│   │   │   ├── stm32f2xx_syscfg.h
│   │   │   ├── stm32f4xx_exti.h
│   │   │   ├── stm32f4xx_syscfg.h
│   │   │   ├── stm32l4x5_exti.h
│   │   │   ├── stm32l4x5_rcc_internals.h
│   │   │   ├── stm32l4x5_rcc.h
│   │   │   ├── stm32l4x5_syscfg.h
│   │   │   ├── tz-mpc.h
│   │   │   ├── tz-msc.h
│   │   │   ├── tz-ppc.h
│   │   │   ├── unimp.h
│   │   │   ├── virt_ctrl.h
│   │   │   ├── vmcoreinfo.h
│   │   │   ├── xlnx-cfi-if.h
│   │   │   ├── xlnx-versal-cframe-reg.h
│   │   │   ├── xlnx-versal-cfu.h
│   │   │   ├── xlnx-versal-crl.h
│   │   │   ├── xlnx-versal-pmc-iou-slcr.h
│   │   │   ├── xlnx-versal-trng.h
│   │   │   ├── xlnx-versal-xramc.h
│   │   │   ├── xlnx-zynqmp-apu-ctrl.h
│   │   │   └── xlnx-zynqmp-crf.h
│   │   ├── net
│   │   │   ├── allwinner_emac.h
│   │   │   ├── allwinner-sun8i-emac.h
│   │   │   ├── cadence_gem.h
│   │   │   ├── dp8393x.h
│   │   │   ├── ftgmac100.h
│   │   │   ├── imx_fec.h
│   │   │   ├── lan9118_phy.h
│   │   │   ├── lan9118.h
│   │   │   ├── lance.h
│   │   │   ├── lasi_82596.h
│   │   │   ├── mii.h
│   │   │   ├── msf2-emac.h
│   │   │   ├── mv88w8618_eth.h
│   │   │   ├── ne2000-isa.h
│   │   │   ├── npcm_gmac.h
│   │   │   ├── npcm_pcs.h
│   │   │   ├── npcm7xx_emc.h
│   │   │   ├── smc91c111.h
│   │   │   ├── xlnx-versal-canfd.h
│   │   │   └── xlnx-zynqmp-can.h
│   │   ├── nmi.h
│   │   ├── nubus
│   │   │   ├── mac-nubus-bridge.h
│   │   │   ├── nubus-virtio-mmio.h
│   │   │   └── nubus.h
│   │   ├── nvram
│   │   │   ├── bcm2835_otp.h
│   │   │   ├── chrp_nvram.h
│   │   │   ├── eeprom_at24c.h
│   │   │   ├── eeprom93xx.h
│   │   │   ├── fw_cfg_acpi.h
│   │   │   ├── fw_cfg.h
│   │   │   ├── mac_nvram.h
│   │   │   ├── npcm7xx_otp.h
│   │   │   ├── nrf51_nvm.h
│   │   │   ├── sun_nvram.h
│   │   │   ├── xlnx-bbram.h
│   │   │   ├── xlnx-efuse.h
│   │   │   ├── xlnx-versal-efuse.h
│   │   │   └── xlnx-zynqmp-efuse.h
│   │   ├── openrisc
│   │   │   └── boot.h
│   │   ├── or-irq.h
│   │   ├── pci
│   │   │   ├── msi.h
│   │   │   ├── msix.h
│   │   │   ├── pci_bridge.h
│   │   │   ├── pci_bus.h
│   │   │   ├── pci_device.h
│   │   │   ├── pci_host.h
│   │   │   ├── pci_ids.h
│   │   │   ├── pci_regs.h
│   │   │   ├── pci.h
│   │   │   ├── pcie_aer.h
│   │   │   ├── pcie_doe.h
│   │   │   ├── pcie_host.h
│   │   │   ├── pcie_port.h
│   │   │   ├── pcie_regs.h
│   │   │   ├── pcie_sriov.h
│   │   │   ├── pcie.h
│   │   │   ├── shpc.h
│   │   │   └── slotid_cap.h
│   │   ├── pci-bridge
│   │   │   ├── cxl_upstream_port.h
│   │   │   ├── pci_expander_bridge.h
│   │   │   ├── simba.h
│   │   │   └── xio3130_downstream.h
│   │   ├── pci-host
│   │   │   ├── articia.h
│   │   │   ├── astro.h
│   │   │   ├── bonito.h
│   │   │   ├── designware.h
│   │   │   ├── dino.h
│   │   │   ├── fsl_imx8m_phy.h
│   │   │   ├── gpex.h
│   │   │   ├── grackle.h
│   │   │   ├── i440fx.h
│   │   │   ├── ls7a.h
│   │   │   ├── mv64361.h
│   │   │   ├── pam.h
│   │   │   ├── pnv_phb3_regs.h
│   │   │   ├── pnv_phb3.h
│   │   │   ├── pnv_phb4_regs.h
│   │   │   ├── pnv_phb4.h
│   │   │   ├── ppc4xx.h
│   │   │   ├── ppce500.h
│   │   │   ├── q35.h
│   │   │   ├── remote.h
│   │   │   ├── sabre.h
│   │   │   ├── spapr.h
│   │   │   ├── uninorth.h
│   │   │   └── xilinx-pcie.h
│   │   ├── platform-bus.h
│   │   ├── ppc
│   │   │   ├── fdt.h
│   │   │   ├── mac_dbdma.h
│   │   │   ├── openpic_kvm.h
│   │   │   ├── openpic.h
│   │   │   ├── pnv_adu.h
│   │   │   ├── pnv_chip.h
│   │   │   ├── pnv_chiptod.h
│   │   │   ├── pnv_core.h
│   │   │   ├── pnv_homer.h
│   │   │   ├── pnv_i2c.h
│   │   │   ├── pnv_lpc.h
│   │   │   ├── pnv_n1_chiplet.h
│   │   │   ├── pnv_nest_pervasive.h
│   │   │   ├── pnv_occ.h
│   │   │   ├── pnv_pnor.h
│   │   │   ├── pnv_psi.h
│   │   │   ├── pnv_sbe.h
│   │   │   ├── pnv_xive.h
│   │   │   ├── pnv_xscom.h
│   │   │   ├── pnv.h
│   │   │   ├── ppc_e500.h
│   │   │   ├── ppc.h
│   │   │   ├── ppc4xx.h
│   │   │   ├── spapr_cpu_core.h
│   │   │   ├── spapr_drc.h
│   │   │   ├── spapr_irq.h
│   │   │   ├── spapr_nested.h
│   │   │   ├── spapr_numa.h
│   │   │   ├── spapr_nvdimm.h
│   │   │   ├── spapr_ovec.h
│   │   │   ├── spapr_tpm_proxy.h
│   │   │   ├── spapr_vio.h
│   │   │   ├── spapr_xive.h
│   │   │   ├── spapr.h
│   │   │   ├── vof.h
│   │   │   ├── xics_spapr.h
│   │   │   ├── xics.h
│   │   │   ├── xive_regs.h
│   │   │   ├── xive.h
│   │   │   ├── xive2_regs.h
│   │   │   └── xive2.h
│   │   ├── ptimer.h
│   │   ├── qdev-clock.h
│   │   ├── qdev-core.h
│   │   ├── qdev-dma.h
│   │   ├── qdev-properties-system.h
│   │   ├── qdev-properties.h
│   │   ├── register.h
│   │   ├── registerfields.h
│   │   ├── remote
│   │   │   ├── iohub.h
│   │   │   ├── iommu.h
│   │   │   ├── machine.h
│   │   │   ├── memory.h
│   │   │   ├── mpqemu-link.h
│   │   │   ├── proxy-memory-listener.h
│   │   │   ├── proxy.h
│   │   │   └── vfio-user-obj.h
│   │   ├── resettable.h
│   │   ├── riscv
│   │   │   ├── boot_opensbi.h
│   │   │   ├── boot.h
│   │   │   ├── iommu.h
│   │   │   ├── microchip_pfsoc.h
│   │   │   ├── numa.h
│   │   │   ├── opentitan.h
│   │   │   ├── riscv_hart.h
│   │   │   ├── shakti_c.h
│   │   │   ├── sifive_cpu.h
│   │   │   ├── sifive_e.h
│   │   │   ├── sifive_u.h
│   │   │   ├── spike.h
│   │   │   └── virt.h
│   │   ├── rtc
│   │   │   ├── allwinner-rtc.h
│   │   │   ├── aspeed_rtc.h
│   │   │   ├── goldfish_rtc.h
│   │   │   ├── m48t59.h
│   │   │   ├── mc146818rtc_regs.h
│   │   │   ├── mc146818rtc.h
│   │   │   ├── pl031.h
│   │   │   ├── sun4v-rtc.h
│   │   │   └── xlnx-zynqmp-rtc.h
│   │   ├── rx
│   │   │   └── rx62n.h
│   │   ├── s390x
│   │   │   ├── 3270-ccw.h
│   │   │   ├── adapter.h
│   │   │   ├── ap-bridge.h
│   │   │   ├── ap-device.h
│   │   │   ├── cpu-topology.h
│   │   │   ├── css-bridge.h
│   │   │   ├── css.h
│   │   │   ├── ebcdic.h
│   │   │   ├── event-facility.h
│   │   │   ├── ioinst.h
│   │   │   ├── ipl
│   │   │   │   └── qipl.h
│   │   │   ├── s390_flic.h
│   │   │   ├── s390-ccw.h
│   │   │   ├── s390-pci-bus.h
│   │   │   ├── s390-pci-clp.h
│   │   │   ├── s390-pci-inst.h
│   │   │   ├── s390-pci-kvm.h
│   │   │   ├── s390-pci-vfio.h
│   │   │   ├── s390-virtio-ccw.h
│   │   │   ├── sclp.h
│   │   │   ├── storage-attributes.h
│   │   │   ├── storage-keys.h
│   │   │   ├── tod.h
│   │   │   └── vfio-ccw.h
│   │   ├── scsi
│   │   │   ├── emulation.h
│   │   │   ├── esp.h
│   │   │   └── scsi.h
│   │   ├── sd
│   │   │   ├── allwinner-sdhost.h
│   │   │   ├── aspeed_sdhci.h
│   │   │   ├── bcm2835_sdhost.h
│   │   │   ├── cadence_sdhci.h
│   │   │   ├── npcm7xx_sdhci.h
│   │   │   ├── sd.h
│   │   │   └── sdhci.h
│   │   ├── sensor
│   │   │   ├── emc141x_regs.h
│   │   │   ├── isl_pmbus_vr.h
│   │   │   ├── tmp105_regs.h
│   │   │   └── tmp105.h
│   │   ├── sh4
│   │   │   ├── sh_intc.h
│   │   │   └── sh.h
│   │   ├── southbridge
│   │   │   ├── ich9.h
│   │   │   └── piix.h
│   │   ├── sparc
│   │   │   ├── sparc32_dma.h
│   │   │   ├── sparc64.h
│   │   │   ├── sun4m_iommu.h
│   │   │   └── sun4u_iommu.h
│   │   ├── ssi
│   │   │   ├── allwinner-a10-spi.h
│   │   │   ├── aspeed_smc.h
│   │   │   ├── bcm2835_spi.h
│   │   │   ├── ibex_spi_host.h
│   │   │   ├── imx_spi.h
│   │   │   ├── mss-spi.h
│   │   │   ├── npcm_pspi.h
│   │   │   ├── npcm7xx_fiu.h
│   │   │   ├── pl022.h
│   │   │   ├── pnv_spi_regs.h
│   │   │   ├── pnv_spi.h
│   │   │   ├── sifive_spi.h
│   │   │   ├── ssi.h
│   │   │   ├── stm32f2xx_spi.h
│   │   │   ├── xilinx_spips.h
│   │   │   └── xlnx-versal-ospi.h
│   │   ├── stream.h
│   │   ├── sysbus.h
│   │   ├── timer
│   │   │   ├── a9gtimer.h
│   │   │   ├── allwinner-a10-pit.h
│   │   │   ├── arm_mptimer.h
│   │   │   ├── armv7m_systick.h
│   │   │   ├── aspeed_timer.h
│   │   │   ├── avr_timer16.h
│   │   │   ├── bcm2835_systmr.h
│   │   │   ├── cadence_ttc.h
│   │   │   ├── cmsdk-apb-dualtimer.h
│   │   │   ├── cmsdk-apb-timer.h
│   │   │   ├── digic-timer.h
│   │   │   ├── grlib_gptimer.h
│   │   │   ├── hpet.h
│   │   │   ├── i8254_internal.h
│   │   │   ├── i8254.h
│   │   │   ├── ibex_timer.h
│   │   │   ├── imx_epit.h
│   │   │   ├── imx_gpt.h
│   │   │   ├── mips_gictimer.h
│   │   │   ├── mss-timer.h
│   │   │   ├── npcm7xx_timer.h
│   │   │   ├── nrf51_timer.h
│   │   │   ├── renesas_cmt.h
│   │   │   ├── renesas_tmr.h
│   │   │   ├── sifive_pwm.h
│   │   │   ├── sse-counter.h
│   │   │   ├── sse-timer.h
│   │   │   ├── stellaris-gptm.h
│   │   │   ├── stm32f2xx_timer.h
│   │   │   └── tmu012.h
│   │   ├── tricore
│   │   │   ├── tc27x_soc.h
│   │   │   ├── triboard.h
│   │   │   ├── tricore_testdevice.h
│   │   │   └── tricore.h
│   │   ├── uefi
│   │   │   ├── hardware-info.h
│   │   │   ├── var-service-api.h
│   │   │   ├── var-service-edk2.h
│   │   │   └── var-service.h
│   │   ├── usb
│   │   │   ├── chipidea.h
│   │   │   ├── dwc2-regs.h
│   │   │   ├── ehci-regs.h
│   │   │   ├── hcd-dwc3.h
│   │   │   ├── hid.h
│   │   │   ├── imx-usb-phy.h
│   │   │   ├── msd.h
│   │   │   ├── uhci-regs.h
│   │   │   ├── xhci.h
│   │   │   ├── xlnx-usb-subsystem.h
│   │   │   └── xlnx-versal-usb2-ctrl-regs.h
│   │   ├── usb.h
│   │   ├── vfio
│   │   │   ├── vfio-amd-xgbe.h
│   │   │   ├── vfio-calxeda-xgmac.h
│   │   │   ├── vfio-container-base.h
│   │   │   ├── vfio-container.h
│   │   │   ├── vfio-cpr.h
│   │   │   ├── vfio-device.h
│   │   │   ├── vfio-migration.h
│   │   │   ├── vfio-platform.h
│   │   │   └── vfio-region.h
│   │   ├── virtio
│   │   │   ├── cbor-helpers.h
│   │   │   ├── iothread-vq-mapping.h
│   │   │   ├── vdpa-dev.h
│   │   │   ├── vhost-backend.h
│   │   │   ├── vhost-scsi-common.h
│   │   │   ├── vhost-scsi.h
│   │   │   ├── vhost-user-base.h
│   │   │   ├── vhost-user-blk.h
│   │   │   ├── vhost-user-fs.h
│   │   │   ├── vhost-user-gpio.h
│   │   │   ├── vhost-user-i2c.h
│   │   │   ├── vhost-user-rng.h
│   │   │   ├── vhost-user-scmi.h
│   │   │   ├── vhost-user-scsi.h
│   │   │   ├── vhost-user-snd.h
│   │   │   ├── vhost-user-vsock.h
│   │   │   ├── vhost-user.h
│   │   │   ├── vhost-vdpa.h
│   │   │   ├── vhost-vsock-common.h
│   │   │   ├── vhost-vsock.h
│   │   │   ├── vhost.h
│   │   │   ├── virtio-access.h
│   │   │   ├── virtio-acpi.h
│   │   │   ├── virtio-balloon.h
│   │   │   ├── virtio-blk-common.h
│   │   │   ├── virtio-blk.h
│   │   │   ├── virtio-bus.h
│   │   │   ├── virtio-crypto.h
│   │   │   ├── virtio-dmabuf.h
│   │   │   ├── virtio-gpu-bswap.h
│   │   │   ├── virtio-gpu-pci.h
│   │   │   ├── virtio-gpu-pixman.h
│   │   │   ├── virtio-gpu.h
│   │   │   ├── virtio-input.h
│   │   │   ├── virtio-iommu.h
│   │   │   ├── virtio-md-pci.h
│   │   │   ├── virtio-mem.h
│   │   │   ├── virtio-mmio.h
│   │   │   ├── virtio-net.h
│   │   │   ├── virtio-nsm.h
│   │   │   ├── virtio-pci.h
│   │   │   ├── virtio-pmem.h
│   │   │   ├── virtio-rng.h
│   │   │   ├── virtio-scsi.h
│   │   │   ├── virtio-serial.h
│   │   │   └── virtio.h
│   │   ├── vmapple
│   │   │   └── vmapple.h
│   │   ├── vmstate-if.h
│   │   ├── watchdog
│   │   │   ├── allwinner-wdt.h
│   │   │   ├── cmsdk-apb-watchdog.h
│   │   │   ├── sbsa_gwdt.h
│   │   │   ├── wdt_aspeed.h
│   │   │   ├── wdt_diag288.h
│   │   │   └── wdt_imx2.h
│   │   ├── xen
│   │   │   ├── arch_hvm.h
│   │   │   ├── interface
│   │   │   │   ├── arch-arm.h
│   │   │   │   ├── arch-x86
│   │   │   │   │   ├── cpuid.h
│   │   │   │   │   ├── xen-x86_32.h
│   │   │   │   │   ├── xen-x86_64.h
│   │   │   │   │   └── xen.h
│   │   │   │   ├── event_channel.h
│   │   │   │   ├── features.h
│   │   │   │   ├── grant_table.h
│   │   │   │   ├── hvm
│   │   │   │   │   ├── hvm_op.h
│   │   │   │   │   └── params.h
│   │   │   │   ├── io
│   │   │   │   │   ├── blkif.h
│   │   │   │   │   ├── console.h
│   │   │   │   │   ├── fbif.h
│   │   │   │   │   ├── kbdif.h
│   │   │   │   │   ├── netif.h
│   │   │   │   │   ├── protocols.h
│   │   │   │   │   ├── ring.h
│   │   │   │   │   ├── usbif.h
│   │   │   │   │   ├── xenbus.h
│   │   │   │   │   └── xs_wire.h
│   │   │   │   ├── memory.h
│   │   │   │   ├── physdev.h
│   │   │   │   ├── sched.h
│   │   │   │   ├── trace.h
│   │   │   │   ├── vcpu.h
│   │   │   │   ├── version.h
│   │   │   │   ├── xen-compat.h
│   │   │   │   └── xen.h
│   │   │   ├── start_info.h
│   │   │   ├── xen_backend_ops.h
│   │   │   ├── xen_igd.h
│   │   │   ├── xen_native.h
│   │   │   ├── xen_pvdev.h
│   │   │   ├── xen-backend.h
│   │   │   ├── xen-block.h
│   │   │   ├── xen-bus-helper.h
│   │   │   ├── xen-bus.h
│   │   │   ├── xen-hvm-common.h
│   │   │   ├── xen-legacy-backend.h
│   │   │   ├── xen-pvh-common.h
│   │   │   ├── xen-x86.h
│   │   │   └── xen.h
│   │   └── xtensa
│   │       ├── mx_pic.h
│   │       └── xtensa-isa.h
│   ├── io
│   │   ├── channel-buffer.h
│   │   ├── channel-command.h
│   │   ├── channel-file.h
│   │   ├── channel-null.h
│   │   ├── channel-socket.h
│   │   ├── channel-tls.h
│   │   ├── channel-util.h
│   │   ├── channel-watch.h
│   │   ├── channel-websock.h
│   │   ├── channel.h
│   │   ├── dns-resolver.h
│   │   ├── net-listener.h
│   │   └── task.h
│   ├── libdecnumber
│   │   ├── dconfig.h
│   │   ├── decContext.h
│   │   ├── decDPD.h
│   │   ├── decNumber.h
│   │   ├── decNumberLocal.h
│   │   └── dpd
│   │       ├── decimal128.h
│   │       ├── decimal128Local.h
│   │       ├── decimal32.h
│   │       └── decimal64.h
│   ├── migration
│   │   ├── blocker.h
│   │   ├── client-options.h
│   │   ├── colo.h
│   │   ├── cpr.h
│   │   ├── cpu.h
│   │   ├── failover.h
│   │   ├── global_state.h
│   │   ├── misc.h
│   │   ├── qemu-file-types.h
│   │   ├── register.h
│   │   ├── snapshot.h
│   │   └── vmstate.h
│   ├── monitor
│   │   ├── hmp-target.h
│   │   ├── hmp.h
│   │   ├── monitor.h
│   │   ├── qdev.h
│   │   └── qmp-helpers.h
│   ├── net
│   │   ├── announce.h
│   │   ├── can_emu.h
│   │   ├── can_host.h
│   │   ├── checksum.h
│   │   ├── eth.h
│   │   ├── filter.h
│   │   ├── net.h
│   │   ├── queue.h
│   │   ├── slirp.h
│   │   ├── tap.h
│   │   ├── vhost_net.h
│   │   ├── vhost-user.h
│   │   └── vhost-vdpa.h
│   ├── qapi
│   │   ├── clone-visitor.h
│   │   ├── compat-policy.h
│   │   ├── dealloc-visitor.h
│   │   ├── error-internal.h
│   │   ├── error.h
│   │   ├── forward-visitor.h
│   │   ├── opts-visitor.h
│   │   ├── qmp
│   │   │   └── qerror.h
│   │   ├── qmp-event.h
│   │   ├── qmp-registry.h
│   │   ├── qobject-input-visitor.h
│   │   ├── qobject-output-visitor.h
│   │   ├── string-input-visitor.h
│   │   ├── string-output-visitor.h
│   │   ├── type-helpers.h
│   │   ├── util.h
│   │   ├── visitor-impl.h
│   │   └── visitor.h
│   ├── qemu
│   │   ├── accel.h
│   │   ├── async-teardown.h
│   │   ├── atomic.h
│   │   ├── atomic128.h
│   │   ├── base64.h
│   │   ├── bcd.h
│   │   ├── bitmap.h
│   │   ├── bitops.h
│   │   ├── bswap.h
│   │   ├── buffer.h
│   │   ├── cacheflush.h
│   │   ├── cacheinfo.h
│   │   ├── chardev_open.h
│   │   ├── co-shared-resource.h
│   │   ├── compiler.h
│   │   ├── config-file.h
│   │   ├── coroutine_int.h
│   │   ├── coroutine-core.h
│   │   ├── coroutine-tls.h
│   │   ├── coroutine.h
│   │   ├── cpu-float.h
│   │   ├── cpuid.h
│   │   ├── crc-ccitt.h
│   │   ├── crc32c.h
│   │   ├── ctype.h
│   │   ├── cutils.h
│   │   ├── datadir.h
│   │   ├── dbus.h
│   │   ├── defer-call.h
│   │   ├── drm.h
│   │   ├── envlist.h
│   │   ├── error-report.h
│   │   ├── event_notifier.h
│   │   ├── fifo32.h
│   │   ├── fifo8.h
│   │   ├── filemonitor.h
│   │   ├── futex.h
│   │   ├── guest-random.h
│   │   ├── hbitmap.h
│   │   ├── help_option.h
│   │   ├── help-texts.h
│   │   ├── host-pci-mmio.h
│   │   ├── host-utils.h
│   │   ├── hw-version.h
│   │   ├── id.h
│   │   ├── int128.h
│   │   ├── interval-tree.h
│   │   ├── iov.h
│   │   ├── iova-tree.h
│   │   ├── jhash.h
│   │   ├── job.h
│   │   ├── keyval.h
│   │   ├── lockable.h
│   │   ├── lockcnt.h
│   │   ├── log-for-trace.h
│   │   ├── log.h
│   │   ├── madvise.h
│   │   ├── main-loop.h
│   │   ├── memalign.h
│   │   ├── memfd.h
│   │   ├── mmap-alloc.h
│   │   ├── module.h
│   │   ├── mprotect.h
│   │   ├── notify.h
│   │   ├── nvdimm-utils.h
│   │   ├── option_int.h
│   │   ├── option.h
│   │   ├── osdep.h
│   │   ├── path.h
│   │   ├── plugin-event.h
│   │   ├── plugin-memory.h
│   │   ├── plugin.h
│   │   ├── pmem.h
│   │   ├── processor.h
│   │   ├── progress_meter.h
│   │   ├── qdist.h
│   │   ├── qemu-plugin.h
│   │   ├── qemu-print.h
│   │   ├── qemu-progress.h
│   │   ├── qht.h
│   │   ├── qsp.h
│   │   ├── qtree.h
│   │   ├── queue.h
│   │   ├── range.h
│   │   ├── ratelimit.h
│   │   ├── rcu_queue.h
│   │   ├── rcu.h
│   │   ├── readline.h
│   │   ├── reserved-region.h
│   │   ├── s390x_pci_mmio.h
│   │   ├── selfmap.h
│   │   ├── seqlock.h
│   │   ├── sockets.h
│   │   ├── stats64.h
│   │   ├── sys_membarrier.h
│   │   ├── systemd.h
│   │   ├── target-info-impl.h
│   │   ├── target-info.h
│   │   ├── thread-context.h
│   │   ├── thread-posix.h
│   │   ├── thread-win32.h
│   │   ├── thread.h
│   │   ├── throttle-options.h
│   │   ├── throttle.h
│   │   ├── timed-average.h
│   │   ├── timer.h
│   │   ├── transactions.h
│   │   ├── tsan.h
│   │   ├── typedefs.h
│   │   ├── unicode.h
│   │   ├── units.h
│   │   ├── userfaultfd.h
│   │   ├── uuid.h
│   │   ├── vfio-helpers.h
│   │   ├── vhost-user-server.h
│   │   ├── win_dump_defs.h
│   │   ├── xattr.h
│   │   ├── xxhash.h
│   │   └── yank.h
│   ├── qemu-io.h
│   ├── qemu-main.h
│   ├── qobject
│   │   ├── json-parser.h
│   │   ├── json-writer.h
│   │   ├── qbool.h
│   │   ├── qdict.h
│   │   ├── qjson.h
│   │   ├── qlist.h
│   │   ├── qlit.h
│   │   ├── qnull.h
│   │   ├── qnum.h
│   │   ├── qobject.h
│   │   └── qstring.h
│   ├── qom
│   │   ├── object_interfaces.h
│   │   ├── object.h
│   │   └── qom-qobject.h
│   ├── scsi
│   │   ├── constants.h
│   │   ├── pr-manager.h
│   │   └── utils.h
│   ├── semihosting
│   │   ├── common-semi.h
│   │   ├── console.h
│   │   ├── guestfd.h
│   │   ├── semihost.h
│   │   ├── syscalls.h
│   │   └── uaccess.h
│   ├── standard-headers
│   │   ├── asm-m68k
│   │   │   ├── bootinfo-mac.h
│   │   │   ├── bootinfo-virt.h
│   │   │   └── bootinfo.h
│   │   ├── asm-s390
│   │   │   └── virtio-ccw.h
│   │   ├── asm-x86
│   │   │   ├── bootparam.h
│   │   │   ├── kvm_para.h
│   │   │   └── setup_data.h
│   │   ├── drm
│   │   │   └── drm_fourcc.h
│   │   ├── linux
│   │   │   ├── const.h
│   │   │   ├── ethtool.h
│   │   │   ├── fuse.h
│   │   │   ├── if_ether.h
│   │   │   ├── input-event-codes.h
│   │   │   ├── input.h
│   │   │   ├── kernel.h
│   │   │   ├── kvm_para.h
│   │   │   ├── pci_regs.h
│   │   │   ├── qemu_fw_cfg.h
│   │   │   ├── sysinfo.h
│   │   │   ├── types.h
│   │   │   ├── udmabuf.h
│   │   │   ├── vhost_types.h
│   │   │   ├── virtio_9p.h
│   │   │   ├── virtio_balloon.h
│   │   │   ├── virtio_blk.h
│   │   │   ├── virtio_bt.h
│   │   │   ├── virtio_config.h
│   │   │   ├── virtio_console.h
│   │   │   ├── virtio_crypto.h
│   │   │   ├── virtio_fs.h
│   │   │   ├── virtio_gpio.h
│   │   │   ├── virtio_gpu.h
│   │   │   ├── virtio_i2c.h
│   │   │   ├── virtio_ids.h
│   │   │   ├── virtio_input.h
│   │   │   ├── virtio_iommu.h
│   │   │   ├── virtio_mem.h
│   │   │   ├── virtio_mmio.h
│   │   │   ├── virtio_net.h
│   │   │   ├── virtio_pci.h
│   │   │   ├── virtio_pcidev.h
│   │   │   ├── virtio_pmem.h
│   │   │   ├── virtio_ring.h
│   │   │   ├── virtio_rng.h
│   │   │   ├── virtio_scmi.h
│   │   │   ├── virtio_scsi.h
│   │   │   ├── virtio_snd.h
│   │   │   ├── virtio_types.h
│   │   │   ├── virtio_vsock.h
│   │   │   └── vmclock-abi.h
│   │   ├── misc
│   │   │   └── pvpanic.h
│   │   └── uefi
│   │       └── uefi.h
│   ├── system
│   │   ├── accel-blocker.h
│   │   ├── accel-ops.h
│   │   ├── address-spaces.h
│   │   ├── arch_init.h
│   │   ├── balloon.h
│   │   ├── block-backend-common.h
│   │   ├── block-backend-global-state.h
│   │   ├── block-backend-io.h
│   │   ├── block-backend.h
│   │   ├── block-ram-registrar.h
│   │   ├── blockdev.h
│   │   ├── confidential-guest-support.h
│   │   ├── cpu-throttle.h
│   │   ├── cpu-timers-internal.h
│   │   ├── cpu-timers.h
│   │   ├── cpus.h
│   │   ├── cryptodev-vhost-user.h
│   │   ├── cryptodev-vhost.h
│   │   ├── cryptodev.h
│   │   ├── device_tree.h
│   │   ├── dirtylimit.h
│   │   ├── dirtyrate.h
│   │   ├── dma.h
│   │   ├── dump-arch.h
│   │   ├── dump.h
│   │   ├── event-loop-base.h
│   │   ├── host_iommu_device.h
│   │   ├── hostmem.h
│   │   ├── hvf_int.h
│   │   ├── hvf.h
│   │   ├── hw_accel.h
│   │   ├── iommufd.h
│   │   ├── ioport.h
│   │   ├── iothread.h
│   │   ├── kvm_int.h
│   │   ├── kvm_xen.h
│   │   ├── kvm.h
│   │   ├── memory_mapping.h
│   │   ├── memory.h
│   │   ├── numa.h
│   │   ├── nvmm.h
│   │   ├── os-posix.h
│   │   ├── os-wasm.h
│   │   ├── os-win32.h
│   │   ├── qtest.h
│   │   ├── ram_addr.h
│   │   ├── ramblock.h
│   │   ├── replay.h
│   │   ├── reset.h
│   │   ├── rng-random.h
│   │   ├── rng.h
│   │   ├── rtc.h
│   │   ├── runstate-action.h
│   │   ├── runstate.h
│   │   ├── seccomp.h
│   │   ├── spdm-socket.h
│   │   ├── stats.h
│   │   ├── system.h
│   │   ├── tcg.h
│   │   ├── tpm_backend.h
│   │   ├── tpm_util.h
│   │   ├── tpm.h
│   │   ├── vhost-user-backend.h
│   │   ├── watchdog.h
│   │   ├── whpx.h
│   │   ├── xen-mapcache.h
│   │   └── xen.h
│   ├── tcg
│   │   ├── debug-assert.h
│   │   ├── debuginfo.h
│   │   ├── helper-info.h
│   │   ├── insn-start-words.h
│   │   ├── perf.h
│   │   ├── startup.h
│   │   ├── tcg-cond.h
│   │   ├── tcg-gvec-desc.h
│   │   ├── tcg-ldst.h
│   │   ├── tcg-mo.h
│   │   ├── tcg-op-common.h
│   │   ├── tcg-op-gvec-common.h
│   │   ├── tcg-op-gvec.h
│   │   ├── tcg-op.h
│   │   ├── tcg-opc.h
│   │   ├── tcg-temp-internal.h
│   │   └── tcg.h
│   ├── ui
│   │   ├── clipboard.h
│   │   ├── console.h
│   │   ├── dbus-display.h
│   │   ├── dbus-module.h
│   │   ├── dmabuf.h
│   │   ├── egl-context.h
│   │   ├── egl-helpers.h
│   │   ├── gtk.h
│   │   ├── input.h
│   │   ├── kbd-state.h
│   │   ├── pixel_ops.h
│   │   ├── pixman-minimal.h
│   │   ├── qemu-pixman.h
│   │   ├── qemu-spice-module.h
│   │   ├── qemu-spice.h
│   │   ├── rect.h
│   │   ├── sdl2.h
│   │   ├── shader.h
│   │   ├── spice-display.h
│   │   ├── surface.h
│   │   └── win32-kbd-hook.h
│   └── user
│       ├── abitypes.h
│       ├── cpu_loop.h
│       ├── guest-base.h
│       ├── guest-host.h
│       ├── mmap.h
│       ├── page-protection.h
│       ├── safe-syscall.h
│       ├── signal.h
│       ├── syscall-trace.h
│       ├── thunk.h
│       └── tswap-target.h
├── io
│   ├── channel-buffer.c
│   ├── channel-command.c
│   ├── channel-file.c
│   ├── channel-null.c
│   ├── channel-socket.c
│   ├── channel-tls.c
│   ├── channel-util.c
│   ├── channel-watch.c
│   ├── channel-websock.c
│   ├── channel.c
│   ├── dns-resolver.c
│   ├── meson.build
│   ├── net-listener.c
│   ├── task.c
│   ├── trace-events
│   └── trace.h
├── iothread.c
├── job-qmp.c
├── job.c
├── Kconfig
├── Kconfig.host
├── libdecnumber
│   ├── decContext.c
│   ├── decNumber.c
│   ├── dpd
│   │   ├── decimal128.c
│   │   ├── decimal32.c
│   │   └── decimal64.c
│   └── meson.build
├── LICENSE
├── linux-headers
│   ├── asm-arm
│   │   ├── bitsperlong.h
│   │   ├── kvm.h
│   │   ├── mman.h
│   │   ├── unistd-common.h
│   │   ├── unistd-eabi.h
│   │   ├── unistd-oabi.h
│   │   └── unistd.h
│   ├── asm-arm64
│   │   ├── bitsperlong.h
│   │   ├── kvm.h
│   │   ├── mman.h
│   │   ├── sve_context.h
│   │   ├── unistd_64.h
│   │   └── unistd.h
│   ├── asm-generic
│   │   ├── bitsperlong.h
│   │   ├── hugetlb_encode.h
│   │   ├── mman-common.h
│   │   ├── mman.h
│   │   └── unistd.h
│   ├── asm-loongarch
│   │   ├── bitsperlong.h
│   │   ├── kvm_para.h
│   │   ├── kvm.h
│   │   ├── mman.h
│   │   ├── unistd_64.h
│   │   └── unistd.h
│   ├── asm-mips
│   │   ├── bitsperlong.h
│   │   ├── kvm.h
│   │   ├── mman.h
│   │   ├── sgidefs.h
│   │   ├── unistd_n32.h
│   │   ├── unistd_n64.h
│   │   ├── unistd_o32.h
│   │   └── unistd.h
│   ├── asm-powerpc
│   │   ├── bitsperlong.h
│   │   ├── kvm.h
│   │   ├── mman.h
│   │   ├── unistd_32.h
│   │   ├── unistd_64.h
│   │   └── unistd.h
│   ├── asm-riscv
│   │   ├── bitsperlong.h
│   │   ├── kvm.h
│   │   ├── mman.h
│   │   ├── ptrace.h
│   │   ├── unistd_32.h
│   │   ├── unistd_64.h
│   │   └── unistd.h
│   ├── asm-s390
│   │   ├── bitsperlong.h
│   │   ├── kvm.h
│   │   ├── mman.h
│   │   ├── unistd_32.h
│   │   ├── unistd_64.h
│   │   └── unistd.h
│   ├── asm-x86
│   │   ├── bitsperlong.h
│   │   ├── kvm_para.h
│   │   ├── kvm.h
│   │   ├── mman.h
│   │   ├── unistd_32.h
│   │   ├── unistd_64.h
│   │   ├── unistd_x32.h
│   │   └── unistd.h
│   ├── COPYING
│   ├── LICENSES
│   │   ├── exceptions
│   │   │   └── Linux-syscall-note
│   │   └── preferred
│   │       ├── BSD-2-Clause
│   │       ├── BSD-3-Clause
│   │       └── GPL-2.0
│   ├── linux
│   │   ├── bits.h
│   │   ├── const.h
│   │   ├── iommufd.h
│   │   ├── kvm_para.h
│   │   ├── kvm.h
│   │   ├── memfd.h
│   │   ├── mman.h
│   │   ├── nvme_ioctl.h
│   │   ├── psci.h
│   │   ├── psp-sev.h
│   │   ├── stddef.h
│   │   ├── userfaultfd.h
│   │   ├── vduse.h
│   │   ├── vfio_ccw.h
│   │   ├── vfio_zdev.h
│   │   ├── vfio.h
│   │   ├── vhost_types.h
│   │   ├── vhost.h
│   │   ├── virtio_config.h
│   │   └── virtio_ring.h
│   └── README
├── linux-user
│   ├── aarch64
│   │   ├── cpu_loop.c
│   │   ├── Makefile.vdso
│   │   ├── meson.build
│   │   ├── mte_user_helper.c
│   │   ├── mte_user_helper.h
│   │   ├── signal.c
│   │   ├── sockbits.h
│   │   ├── syscall_64.tbl
│   │   ├── syscall_nr.h
│   │   ├── syscallhdr.sh
│   │   ├── target_cpu.h
│   │   ├── target_elf.h
│   │   ├── target_errno_defs.h
│   │   ├── target_fcntl.h
│   │   ├── target_flat.h
│   │   ├── target_mman.h
│   │   ├── target_prctl.h
│   │   ├── target_proc.h
│   │   ├── target_resource.h
│   │   ├── target_signal.h
│   │   ├── target_structs.h
│   │   ├── target_syscall.h
│   │   ├── termbits.h
│   │   ├── vdso-be.so
│   │   ├── vdso-le.so
│   │   ├── vdso.ld
│   │   └── vdso.S
│   ├── alpha
│   │   ├── cpu_loop.c
│   │   ├── meson.build
│   │   ├── signal.c
│   │   ├── sockbits.h
│   │   ├── syscall.tbl
│   │   ├── syscallhdr.sh
│   │   ├── target_cpu.h
│   │   ├── target_elf.h
│   │   ├── target_errno_defs.h
│   │   ├── target_fcntl.h
│   │   ├── target_mman.h
│   │   ├── target_prctl.h
│   │   ├── target_proc.h
│   │   ├── target_resource.h
│   │   ├── target_signal.h
│   │   ├── target_structs.h
│   │   ├── target_syscall.h
│   │   └── termbits.h
│   ├── arm
│   │   ├── cpu_loop.c
│   │   ├── Makefile.vdso
│   │   ├── meson.build
│   │   ├── nwfpe
│   │   │   ├── double_cpdo.c
│   │   │   ├── extended_cpdo.c
│   │   │   ├── fpa11_cpdo.c
│   │   │   ├── fpa11_cpdt.c
│   │   │   ├── fpa11_cprt.c
│   │   │   ├── fpa11.c
│   │   │   ├── fpa11.h
│   │   │   ├── fpa11.inl
│   │   │   ├── fpopcode.c
│   │   │   ├── fpopcode.h
│   │   │   ├── fpsr.h
│   │   │   ├── meson.build
│   │   │   └── single_cpdo.c
│   │   ├── signal.c
│   │   ├── sockbits.h
│   │   ├── syscall.tbl
│   │   ├── syscallhdr.sh
│   │   ├── target_cpu.h
│   │   ├── target_elf.h
│   │   ├── target_errno_defs.h
│   │   ├── target_fcntl.h
│   │   ├── target_flat.h
│   │   ├── target_mman.h
│   │   ├── target_prctl.h
│   │   ├── target_proc.h
│   │   ├── target_resource.h
│   │   ├── target_signal.h
│   │   ├── target_structs.h
│   │   ├── target_syscall.h
│   │   ├── termbits.h
│   │   ├── vdso-asmoffset.h
│   │   ├── vdso-be32.so
│   │   ├── vdso-be8.so
│   │   ├── vdso-le.so
│   │   ├── vdso.ld
│   │   └── vdso.S
│   ├── elfload.c
│   ├── errnos.c.inc
│   ├── exit.c
│   ├── fd-trans.c
│   ├── fd-trans.h
│   ├── flat.h
│   ├── flatload.c
│   ├── gen-vdso-elfn.c.inc
│   ├── gen-vdso.c
│   ├── generic
│   │   ├── fcntl.h
│   │   ├── signal.h
│   │   ├── sockbits.h
│   │   ├── target_errno_defs.h
│   │   ├── target_flat.h
│   │   ├── target_mman.h
│   │   ├── target_prctl_unalign.h
│   │   ├── target_resource.h
│   │   ├── target_structs.h
│   │   └── termbits.h
│   ├── hexagon
│   │   ├── cpu_loop.c
│   │   ├── meson.build
│   │   ├── signal.c
│   │   ├── sockbits.h
│   │   ├── syscall.tbl
│   │   ├── syscallhdr.sh
│   │   ├── target_cpu.h
│   │   ├── target_elf.h
│   │   ├── target_errno_defs.h
│   │   ├── target_fcntl.h
│   │   ├── target_mman.h
│   │   ├── target_prctl.h
│   │   ├── target_proc.h
│   │   ├── target_resource.h
│   │   ├── target_signal.h
│   │   ├── target_structs.h
│   │   ├── target_syscall.h
│   │   └── termbits.h
│   ├── hppa
│   │   ├── cpu_loop.c
│   │   ├── Makefile.vdso
│   │   ├── meson.build
│   │   ├── signal.c
│   │   ├── sockbits.h
│   │   ├── syscall.tbl
│   │   ├── syscallhdr.sh
│   │   ├── target_cpu.h
│   │   ├── target_elf.h
│   │   ├── target_errno_defs.h
│   │   ├── target_fcntl.h
│   │   ├── target_mman.h
│   │   ├── target_prctl.h
│   │   ├── target_proc.h
│   │   ├── target_resource.h
│   │   ├── target_signal.h
│   │   ├── target_structs.h
│   │   ├── target_syscall.h
│   │   ├── termbits.h
│   │   ├── vdso-asmoffset.h
│   │   ├── vdso.ld
│   │   ├── vdso.S
│   │   └── vdso.so
│   ├── i386
│   │   ├── cpu_loop.c
│   │   ├── Makefile.vdso
│   │   ├── meson.build
│   │   ├── signal.c
│   │   ├── sockbits.h
│   │   ├── syscall_32.tbl
│   │   ├── syscall_nr.h
│   │   ├── syscallhdr.sh
│   │   ├── target_cpu.h
│   │   ├── target_elf.h
│   │   ├── target_errno_defs.h
│   │   ├── target_fcntl.h
│   │   ├── target_mman.h
│   │   ├── target_prctl.h
│   │   ├── target_proc.h
│   │   ├── target_resource.h
│   │   ├── target_signal.h
│   │   ├── target_structs.h
│   │   ├── target_syscall.h
│   │   ├── termbits.h
│   │   ├── vdso-asmoffset.h
│   │   ├── vdso.ld
│   │   ├── vdso.S
│   │   └── vdso.so
│   ├── include
│   │   ├── host
│   │   │   ├── aarch64
│   │   │   │   └── host-signal.h
│   │   │   ├── arm
│   │   │   │   └── host-signal.h
│   │   │   ├── i386
│   │   │   │   └── host-signal.h
│   │   │   ├── loongarch64
│   │   │   │   └── host-signal.h
│   │   │   ├── mips
│   │   │   │   └── host-signal.h
│   │   │   ├── ppc
│   │   │   │   └── host-signal.h
│   │   │   ├── ppc64
│   │   │   │   └── host-signal.h
│   │   │   ├── riscv
│   │   │   │   └── host-signal.h
│   │   │   ├── s390x
│   │   │   │   └── host-signal.h
│   │   │   ├── sparc64
│   │   │   │   └── host-signal.h
│   │   │   └── x86_64
│   │   │       └── host-signal.h
│   │   └── special-errno.h
│   ├── ioctls.h
│   ├── linux_loop.h
│   ├── linuxload.c
│   ├── loader.h
│   ├── loongarch64
│   │   ├── cpu_loop.c
│   │   ├── Makefile.vdso
│   │   ├── meson.build
│   │   ├── signal.c
│   │   ├── sockbits.h
│   │   ├── syscall.tbl
│   │   ├── syscallhdr.sh
│   │   ├── target_cpu.h
│   │   ├── target_elf.h
│   │   ├── target_errno_defs.h
│   │   ├── target_fcntl.h
│   │   ├── target_mman.h
│   │   ├── target_prctl.h
│   │   ├── target_proc.h
│   │   ├── target_resource.h
│   │   ├── target_signal.h
│   │   ├── target_structs.h
│   │   ├── target_syscall.h
│   │   ├── termbits.h
│   │   ├── vdso-asmoffset.h
│   │   ├── vdso.ld
│   │   ├── vdso.S
│   │   └── vdso.so
│   ├── m68k
│   │   ├── cpu_loop.c
│   │   ├── meson.build
│   │   ├── signal.c
│   │   ├── sockbits.h
│   │   ├── syscall.tbl
│   │   ├── syscallhdr.sh
│   │   ├── target_cpu.h
│   │   ├── target_elf.h
│   │   ├── target_errno_defs.h
│   │   ├── target_fcntl.h
│   │   ├── target_flat.h
│   │   ├── target_mman.h
│   │   ├── target_prctl.h
│   │   ├── target_proc.h
│   │   ├── target_resource.h
│   │   ├── target_signal.h
│   │   ├── target_structs.h
│   │   ├── target_syscall.h
│   │   └── termbits.h
│   ├── main.c
│   ├── meson.build
│   ├── microblaze
│   │   ├── cpu_loop.c
│   │   ├── meson.build
│   │   ├── signal.c
│   │   ├── sockbits.h
│   │   ├── syscall.tbl
│   │   ├── syscallhdr.sh
│   │   ├── target_cpu.h
│   │   ├── target_elf.h
│   │   ├── target_errno_defs.h
│   │   ├── target_fcntl.h
│   │   ├── target_flat.h
│   │   ├── target_mman.h
│   │   ├── target_prctl.h
│   │   ├── target_proc.h
│   │   ├── target_resource.h
│   │   ├── target_signal.h
│   │   ├── target_structs.h
│   │   ├── target_syscall.h
│   │   └── termbits.h
│   ├── mips
│   │   ├── cpu_loop.c
│   │   ├── meson.build
│   │   ├── signal.c
│   │   ├── sockbits.h
│   │   ├── syscall_nr.h
│   │   ├── syscall_o32.tbl
│   │   ├── syscall-args-o32.c.inc
│   │   ├── syscallhdr.sh
│   │   ├── target_cpu.h
│   │   ├── target_elf.h
│   │   ├── target_errno_defs.h
│   │   ├── target_fcntl.h
│   │   ├── target_mman.h
│   │   ├── target_prctl.h
│   │   ├── target_proc.h
│   │   ├── target_resource.h
│   │   ├── target_signal.h
│   │   ├── target_structs.h
│   │   ├── target_syscall.h
│   │   └── termbits.h
│   ├── mips64
│   │   ├── cpu_loop.c
│   │   ├── meson.build
│   │   ├── signal.c
│   │   ├── sockbits.h
│   │   ├── syscall_n32.tbl
│   │   ├── syscall_n64.tbl
│   │   ├── syscall_nr.h
│   │   ├── syscallhdr.sh
│   │   ├── target_cpu.h
│   │   ├── target_elf.h
│   │   ├── target_errno_defs.h
│   │   ├── target_fcntl.h
│   │   ├── target_mman.h
│   │   ├── target_prctl.h
│   │   ├── target_proc.h
│   │   ├── target_resource.h
│   │   ├── target_signal.h
│   │   ├── target_structs.h
│   │   ├── target_syscall.h
│   │   └── termbits.h
│   ├── mmap.c
│   ├── openrisc
│   │   ├── cpu_loop.c
│   │   ├── meson.build
│   │   ├── signal.c
│   │   ├── sockbits.h
│   │   ├── syscall.tbl
│   │   ├── syscallhdr.sh
│   │   ├── target_cpu.h
│   │   ├── target_elf.h
│   │   ├── target_errno_defs.h
│   │   ├── target_fcntl.h
│   │   ├── target_mman.h
│   │   ├── target_prctl.h
│   │   ├── target_proc.h
│   │   ├── target_resource.h
│   │   ├── target_signal.h
│   │   ├── target_structs.h
│   │   ├── target_syscall.h
│   │   └── termbits.h
│   ├── plugin-api.c
│   ├── ppc
│   │   ├── cpu_loop.c
│   │   ├── Makefile.vdso
│   │   ├── meson.build
│   │   ├── signal.c
│   │   ├── sockbits.h
│   │   ├── syscall.tbl
│   │   ├── syscallhdr.sh
│   │   ├── target_cpu.h
│   │   ├── target_elf.h
│   │   ├── target_errno_defs.h
│   │   ├── target_fcntl.h
│   │   ├── target_mman.h
│   │   ├── target_prctl.h
│   │   ├── target_proc.h
│   │   ├── target_resource.h
│   │   ├── target_signal.h
│   │   ├── target_structs.h
│   │   ├── target_syscall.h
│   │   ├── termbits.h
│   │   ├── vdso-32.ld
│   │   ├── vdso-32.so
│   │   ├── vdso-64.ld
│   │   ├── vdso-64.so
│   │   ├── vdso-64le.so
│   │   ├── vdso-asmoffset.h
│   │   └── vdso.S
│   ├── qemu.h
│   ├── riscv
│   │   ├── cpu_loop.c
│   │   ├── Makefile.vdso
│   │   ├── meson.build
│   │   ├── signal.c
│   │   ├── sockbits.h
│   │   ├── syscall.tbl
│   │   ├── syscallhdr.sh
│   │   ├── target_cpu.h
│   │   ├── target_elf.h
│   │   ├── target_errno_defs.h
│   │   ├── target_fcntl.h
│   │   ├── target_mman.h
│   │   ├── target_prctl.h
│   │   ├── target_proc.h
│   │   ├── target_resource.h
│   │   ├── target_signal.h
│   │   ├── target_structs.h
│   │   ├── target_syscall.h
│   │   ├── termbits.h
│   │   ├── vdso-32.so
│   │   ├── vdso-64.so
│   │   ├── vdso-asmoffset.h
│   │   ├── vdso.ld
│   │   └── vdso.S
│   ├── s390x
│   │   ├── cpu_loop.c
│   │   ├── Makefile.vdso
│   │   ├── meson.build
│   │   ├── signal.c
│   │   ├── sockbits.h
│   │   ├── syscall.tbl
│   │   ├── syscallhdr.sh
│   │   ├── target_cpu.h
│   │   ├── target_elf.h
│   │   ├── target_errno_defs.h
│   │   ├── target_fcntl.h
│   │   ├── target_mman.h
│   │   ├── target_prctl.h
│   │   ├── target_proc.h
│   │   ├── target_resource.h
│   │   ├── target_signal.h
│   │   ├── target_structs.h
│   │   ├── target_syscall.h
│   │   ├── termbits.h
│   │   ├── vdso-asmoffset.h
│   │   ├── vdso.ld
│   │   ├── vdso.S
│   │   └── vdso.so
│   ├── semihost.c
│   ├── sh4
│   │   ├── cpu_loop.c
│   │   ├── meson.build
│   │   ├── signal.c
│   │   ├── sockbits.h
│   │   ├── syscall.tbl
│   │   ├── syscallhdr.sh
│   │   ├── target_cpu.h
│   │   ├── target_elf.h
│   │   ├── target_errno_defs.h
│   │   ├── target_fcntl.h
│   │   ├── target_flat.h
│   │   ├── target_mman.h
│   │   ├── target_prctl.h
│   │   ├── target_proc.h
│   │   ├── target_resource.h
│   │   ├── target_signal.h
│   │   ├── target_structs.h
│   │   ├── target_syscall.h
│   │   └── termbits.h
│   ├── signal-common.h
│   ├── signal.c
│   ├── socket.h
│   ├── sparc
│   │   ├── cpu_loop.c
│   │   ├── meson.build
│   │   ├── signal.c
│   │   ├── sockbits.h
│   │   ├── syscall.tbl
│   │   ├── syscallhdr.sh
│   │   ├── target_cpu.h
│   │   ├── target_elf.h
│   │   ├── target_errno_defs.h
│   │   ├── target_fcntl.h
│   │   ├── target_mman.h
│   │   ├── target_prctl.h
│   │   ├── target_proc.h
│   │   ├── target_resource.h
│   │   ├── target_signal.h
│   │   ├── target_structs.h
│   │   ├── target_syscall.h
│   │   └── termbits.h
│   ├── strace.c
│   ├── strace.h
│   ├── strace.list
│   ├── syscall_defs.h
│   ├── syscall_types.h
│   ├── syscall.c
│   ├── thunk.c
│   ├── trace-events
│   ├── trace.h
│   ├── uaccess.c
│   ├── uname.c
│   ├── uname.h
│   ├── user-internals.h
│   ├── user-mmap.h
│   ├── vm86.c
│   ├── x86_64
│   │   ├── cpu_loop.c
│   │   ├── Makefile.vdso
│   │   ├── meson.build
│   │   ├── signal.c
│   │   ├── sockbits.h
│   │   ├── syscall_64.tbl
│   │   ├── syscall_nr.h
│   │   ├── syscallhdr.sh
│   │   ├── target_cpu.h
│   │   ├── target_elf.h
│   │   ├── target_errno_defs.h
│   │   ├── target_fcntl.h
│   │   ├── target_mman.h
│   │   ├── target_prctl.h
│   │   ├── target_proc.h
│   │   ├── target_resource.h
│   │   ├── target_signal.h
│   │   ├── target_structs.h
│   │   ├── target_syscall.h
│   │   ├── termbits.h
│   │   ├── vdso.ld
│   │   ├── vdso.S
│   │   └── vdso.so
│   └── xtensa
│       ├── cpu_loop.c
│       ├── meson.build
│       ├── signal.c
│       ├── sockbits.h
│       ├── syscall.tbl
│       ├── syscallhdr.sh
│       ├── target_cpu.h
│       ├── target_elf.h
│       ├── target_errno_defs.h
│       ├── target_fcntl.h
│       ├── target_flat.h
│       ├── target_mman.h
│       ├── target_prctl.h
│       ├── target_proc.h
│       ├── target_resource.h
│       ├── target_signal.h
│       ├── target_structs.h
│       ├── target_syscall.h
│       └── termbits.h
├── MAINTAINERS
├── Makefile
├── meson_options.txt
├── meson.build
├── migration
│   ├── block-active.c
│   ├── block-dirty-bitmap.c
│   ├── channel-block.c
│   ├── channel-block.h
│   ├── channel.c
│   ├── channel.h
│   ├── colo-failover.c
│   ├── colo-stubs.c
│   ├── colo.c
│   ├── cpr-transfer.c
│   ├── cpr.c
│   ├── cpu-throttle.c
│   ├── dirtyrate.c
│   ├── dirtyrate.h
│   ├── exec.c
│   ├── exec.h
│   ├── fd.c
│   ├── fd.h
│   ├── file.c
│   ├── file.h
│   ├── global_state.c
│   ├── meson.build
│   ├── migration-hmp-cmds.c
│   ├── migration-stats.c
│   ├── migration-stats.h
│   ├── migration.c
│   ├── migration.h
│   ├── multifd-device-state.c
│   ├── multifd-nocomp.c
│   ├── multifd-qatzip.c
│   ├── multifd-qpl.c
│   ├── multifd-uadk.c
│   ├── multifd-zero-page.c
│   ├── multifd-zlib.c
│   ├── multifd-zstd.c
│   ├── multifd.c
│   ├── multifd.h
│   ├── options.c
│   ├── options.h
│   ├── page_cache.c
│   ├── page_cache.h
│   ├── postcopy-ram.c
│   ├── postcopy-ram.h
│   ├── qemu-file.c
│   ├── qemu-file.h
│   ├── ram.c
│   ├── ram.h
│   ├── rdma.c
│   ├── rdma.h
│   ├── savevm.c
│   ├── savevm.h
│   ├── socket.c
│   ├── socket.h
│   ├── target.c
│   ├── threadinfo.c
│   ├── threadinfo.h
│   ├── tls.c
│   ├── tls.h
│   ├── trace-events
│   ├── trace.h
│   ├── vmstate-types.c
│   ├── vmstate.c
│   ├── xbzrle.c
│   ├── xbzrle.h
│   ├── yank_functions.c
│   └── yank_functions.h
├── module-common.c
├── monitor
│   ├── fds.c
│   ├── hmp-cmds-target.c
│   ├── hmp-cmds.c
│   ├── hmp-target.c
│   ├── hmp.c
│   ├── meson.build
│   ├── monitor-internal.h
│   ├── monitor.c
│   ├── qemu-config-qmp.c
│   ├── qmp-cmds-control.c
│   ├── qmp-cmds.c
│   ├── qmp.c
│   ├── trace-events
│   └── trace.h
├── nbd
│   ├── client-connection.c
│   ├── client.c
│   ├── common.c
│   ├── meson.build
│   ├── nbd-internal.h
│   ├── server.c
│   ├── trace-events
│   └── trace.h
├── net
│   ├── af-xdp.c
│   ├── announce.c
│   ├── can
│   │   ├── can_core.c
│   │   ├── can_host.c
│   │   ├── can_socketcan.c
│   │   └── meson.build
│   ├── checksum.c
│   ├── clients.h
│   ├── colo-compare.c
│   ├── colo-compare.h
│   ├── colo-stubs.c
│   ├── colo.c
│   ├── colo.h
│   ├── dgram.c
│   ├── dump.c
│   ├── eth.c
│   ├── filter-buffer.c
│   ├── filter-mirror.c
│   ├── filter-replay.c
│   ├── filter-rewriter.c
│   ├── filter.c
│   ├── hub.c
│   ├── hub.h
│   ├── l2tpv3.c
│   ├── meson.build
│   ├── net-hmp-cmds.c
│   ├── net.c
│   ├── netmap.c
│   ├── queue.c
│   ├── slirp.c
│   ├── socket.c
│   ├── stream.c
│   ├── tap_int.h
│   ├── tap-bsd.c
│   ├── tap-linux.c
│   ├── tap-linux.h
│   ├── tap-solaris.c
│   ├── tap-stub.c
│   ├── tap-win32.c
│   ├── tap.c
│   ├── trace-events
│   ├── trace.h
│   ├── util.c
│   ├── util.h
│   ├── vde.c
│   ├── vhost-user-stub.c
│   ├── vhost-user.c
│   ├── vhost-vdpa-stub.c
│   ├── vhost-vdpa.c
│   ├── vmnet_int.h
│   ├── vmnet-bridged.m
│   ├── vmnet-common.m
│   ├── vmnet-host.c
│   └── vmnet-shared.c
├── NOTES.md
├── os-posix.c
├── os-wasm.c
├── os-win32.c
├── page-target.c
├── page-vary-common.c
├── page-vary-target.c
├── pc-bios
│   ├── ast27x0_bootrom.bin
│   ├── bios-256k.bin
│   ├── bios-microvm.bin
│   ├── bios.bin
│   ├── descriptors
│   │   ├── 50-edk2-i386-secure.json
│   │   ├── 50-edk2-x86_64-secure.json
│   │   ├── 60-edk2-aarch64.json
│   │   ├── 60-edk2-arm.json
│   │   ├── 60-edk2-i386.json
│   │   ├── 60-edk2-loongarch64.json
│   │   ├── 60-edk2-riscv64.json
│   │   ├── 60-edk2-x86_64.json
│   │   └── meson.build
│   ├── dtb
│   │   ├── bamboo.dtb
│   │   ├── bamboo.dts
│   │   ├── canyonlands.dtb
│   │   ├── canyonlands.dts
│   │   ├── meson.build
│   │   ├── petalogix-ml605.dtb
│   │   ├── petalogix-ml605.dts
│   │   ├── petalogix-s3adsp1800.dtb
│   │   └── petalogix-s3adsp1800.dts
│   ├── edk2-aarch64-code.fd.bz2
│   ├── edk2-arm-code.fd.bz2
│   ├── edk2-arm-vars.fd.bz2
│   ├── edk2-i386-code.fd.bz2
│   ├── edk2-i386-secure-code.fd.bz2
│   ├── edk2-i386-vars.fd.bz2
│   ├── edk2-licenses.txt
│   ├── edk2-loongarch64-code.fd.bz2
│   ├── edk2-loongarch64-vars.fd.bz2
│   ├── edk2-riscv-code.fd.bz2
│   ├── edk2-riscv-vars.fd.bz2
│   ├── edk2-x86_64-code.fd.bz2
│   ├── edk2-x86_64-microvm.fd.bz2
│   ├── edk2-x86_64-secure-code.fd.bz2
│   ├── efi-e1000.rom
│   ├── efi-e1000e.rom
│   ├── efi-eepro100.rom
│   ├── efi-ne2k_pci.rom
│   ├── efi-pcnet.rom
│   ├── efi-rtl8139.rom
│   ├── efi-virtio.rom
│   ├── efi-vmxnet3.rom
│   ├── hppa-firmware.img
│   ├── hppa-firmware64.img
│   ├── keymaps
│   │   ├── ar
│   │   ├── bepo
│   │   ├── cz
│   │   ├── da
│   │   ├── de
│   │   ├── de-ch
│   │   ├── en-gb
│   │   ├── en-us
│   │   ├── es
│   │   ├── et
│   │   ├── fi
│   │   ├── fo
│   │   ├── fr
│   │   ├── fr-be
│   │   ├── fr-ca
│   │   ├── fr-ch
│   │   ├── hr
│   │   ├── hu
│   │   ├── is
│   │   ├── it
│   │   ├── ja
│   │   ├── lt
│   │   ├── lv
│   │   ├── meson.build
│   │   ├── mk
│   │   ├── nl
│   │   ├── no
│   │   ├── pl
│   │   ├── pt
│   │   ├── pt-br
│   │   ├── ru
│   │   ├── sl
│   │   ├── sv
│   │   ├── th
│   │   └── tr
│   ├── kvmvapic.bin
│   ├── linuxboot_dma.bin
│   ├── linuxboot.bin
│   ├── meson.build
│   ├── multiboot_dma.bin
│   ├── multiboot.bin
│   ├── npcm7xx_bootrom.bin
│   ├── npcm8xx_bootrom.bin
│   ├── openbios-ppc
│   ├── openbios-sparc32
│   ├── openbios-sparc64
│   ├── opensbi-riscv32-generic-fw_dynamic.bin
│   ├── opensbi-riscv64-generic-fw_dynamic.bin
│   ├── optionrom
│   │   ├── flat.lds
│   │   ├── kvmvapic.S
│   │   ├── linuxboot_dma.c
│   │   ├── linuxboot.S
│   │   ├── Makefile
│   │   ├── multiboot_dma.S
│   │   ├── multiboot.S
│   │   ├── optionrom.h
│   │   ├── optrom_fw_cfg.h
│   │   ├── optrom.h
│   │   ├── pvh_main.c
│   │   └── pvh.S
│   ├── palcode-clipper
│   ├── pnv-pnor.bin
│   ├── pvh.bin
│   ├── pxe-e1000.rom
│   ├── pxe-eepro100.rom
│   ├── pxe-ne2k_pci.rom
│   ├── pxe-pcnet.rom
│   ├── pxe-rtl8139.rom
│   ├── pxe-virtio.rom
│   ├── qboot.rom
│   ├── qemu_logo.svg
│   ├── qemu_vga.ndrv
│   ├── qemu-nsis.bmp
│   ├── qemu-nsis.ico
│   ├── QEMU,cgthree.bin
│   ├── QEMU,tcx.bin
│   ├── qemu.rsrc
│   ├── README
│   ├── s390-ccw
│   │   ├── bootmap.c
│   │   ├── bootmap.h
│   │   ├── bswap.h
│   │   ├── cio.c
│   │   ├── cio.h
│   │   ├── dasd-ipl.c
│   │   ├── dasd-ipl.h
│   │   ├── helper.h
│   │   ├── iplb.h
│   │   ├── jump2ipl.c
│   │   ├── main.c
│   │   ├── Makefile
│   │   ├── menu.c
│   │   ├── netmain.c
│   │   ├── s390-arch.h
│   │   ├── s390-ccw.h
│   │   ├── s390-time.h
│   │   ├── sclp.c
│   │   ├── sclp.h
│   │   ├── scsi.h
│   │   ├── start.S
│   │   ├── virtio-blkdev.c
│   │   ├── virtio-net.c
│   │   ├── virtio-scsi.c
│   │   ├── virtio-scsi.h
│   │   ├── virtio.c
│   │   └── virtio.h
│   ├── s390-ccw.img
│   ├── skiboot.lid
│   ├── slof.bin
│   ├── u-boot-sam460-20100605.bin
│   ├── u-boot.e500
│   ├── vgabios-ati.bin
│   ├── vgabios-bochs-display.bin
│   ├── vgabios-cirrus.bin
│   ├── vgabios-qxl.bin
│   ├── vgabios-ramfb.bin
│   ├── vgabios-stdvga.bin
│   ├── vgabios-virtio.bin
│   ├── vgabios-vmware.bin
│   ├── vgabios.bin
│   ├── vof
│   │   ├── bootmem.c
│   │   ├── ci.c
│   │   ├── entry.S
│   │   ├── libc.c
│   │   ├── main.c
│   │   ├── Makefile
│   │   ├── vof.h
│   │   └── vof.lds
│   ├── vof-nvram.bin
│   └── vof.bin
├── plugins
│   ├── api-system.c
│   ├── api-user.c
│   ├── api.c
│   ├── core.c
│   ├── loader.c
│   ├── meson.build
│   ├── plugin.h
│   ├── system.c
│   └── user.c
├── po
│   ├── bg.po
│   ├── de_DE.po
│   ├── fr_FR.po
│   ├── hu.po
│   ├── it.po
│   ├── LINGUAS
│   ├── meson.build
│   ├── POTFILES
│   ├── sv.po
│   ├── tr.po
│   ├── uk.po
│   └── zh_CN.po
├── python
│   ├── avocado.cfg
│   ├── Makefile
│   ├── MANIFEST.in
│   ├── PACKAGE.rst
│   ├── qemu
│   │   ├── machine
│   │   │   ├── __init__.py
│   │   │   ├── console_socket.py
│   │   │   ├── machine.py
│   │   │   ├── py.typed
│   │   │   ├── qtest.py
│   │   │   └── README.rst
│   │   ├── qmp
│   │   │   ├── __init__.py
│   │   │   ├── error.py
│   │   │   ├── events.py
│   │   │   ├── legacy.py
│   │   │   ├── message.py
│   │   │   ├── models.py
│   │   │   ├── protocol.py
│   │   │   ├── py.typed
│   │   │   ├── qmp_client.py
│   │   │   ├── qmp_shell.py
│   │   │   ├── qmp_tui.py
│   │   │   └── util.py
│   │   ├── README.rst
│   │   └── utils
│   │       ├── __init__.py
│   │       ├── accel.py
│   │       ├── py.typed
│   │       ├── qemu_ga_client.py
│   │       ├── qom_common.py
│   │       ├── qom_fuse.py
│   │       ├── qom.py
│   │       └── README.rst
│   ├── README.rst
│   ├── scripts
│   │   ├── mkvenv.py
│   │   └── vendor.py
│   ├── setup.cfg
│   ├── setup.py
│   ├── tests
│   │   ├── flake8.sh
│   │   ├── iotests-mypy.sh
│   │   ├── iotests-pylint.sh
│   │   ├── isort.sh
│   │   ├── minreqs.txt
│   │   ├── mypy.sh
│   │   ├── protocol.py
│   │   ├── pylint.sh
│   │   ├── qapi-flake8.sh
│   │   ├── qapi-isort.sh
│   │   ├── qapi-mypy.sh
│   │   └── qapi-pylint.sh
│   ├── VERSION
│   └── wheels
│       ├── meson-1.8.1-py3-none-any.whl
│       └── pycotap-1.3.1-py3-none-any.whl
├── pythondeps.toml
├── qapi
│   ├── acpi.json
│   ├── audio.json
│   ├── authz.json
│   ├── block-core.json
│   ├── block-export.json
│   ├── block.json
│   ├── char.json
│   ├── common.json
│   ├── compat.json
│   ├── control.json
│   ├── crypto.json
│   ├── cryptodev.json
│   ├── cxl.json
│   ├── dump.json
│   ├── ebpf.json
│   ├── error.json
│   ├── introspect.json
│   ├── job.json
│   ├── machine-common.json
│   ├── machine-s390x.json
│   ├── machine.json
│   ├── meson.build
│   ├── migration.json
│   ├── misc-arm.json
│   ├── misc-i386.json
│   ├── misc.json
│   ├── net.json
│   ├── opts-visitor.c
│   ├── pci.json
│   ├── pragma.json
│   ├── qapi-clone-visitor.c
│   ├── qapi-dealloc-visitor.c
│   ├── qapi-forward-visitor.c
│   ├── qapi-schema.json
│   ├── qapi-type-helpers.c
│   ├── qapi-util.c
│   ├── qapi-visit-core.c
│   ├── qdev.json
│   ├── qmp-dispatch.c
│   ├── qmp-event.c
│   ├── qmp-registry.c
│   ├── qobject-input-visitor.c
│   ├── qobject-output-visitor.c
│   ├── qom.json
│   ├── replay.json
│   ├── rocker.json
│   ├── run-state.json
│   ├── sockets.json
│   ├── stats.json
│   ├── string-input-visitor.c
│   ├── string-output-visitor.c
│   ├── tpm.json
│   ├── trace-events
│   ├── trace.h
│   ├── trace.json
│   ├── transaction.json
│   ├── uefi.json
│   ├── ui.json
│   ├── vfio.json
│   ├── virtio.json
│   └── yank.json
├── qemu-bridge-helper.c
├── qemu-edid.c
├── qemu-img-cmds.hx
├── qemu-img.c
├── qemu-io-cmds.c
├── qemu-io.c
├── qemu-keymap.c
├── qemu-nbd.c
├── qemu-options.hx
├── qemu.nsi
├── qemu.sasl
├── qga
│   ├── channel-posix.c
│   ├── channel-win32.c
│   ├── channel.h
│   ├── commands-bsd.c
│   ├── commands-common-ssh.c
│   ├── commands-common-ssh.h
│   ├── commands-common.h
│   ├── commands-linux.c
│   ├── commands-posix-ssh.c
│   ├── commands-posix.c
│   ├── commands-win32.c
│   ├── commands-windows-ssh.c
│   ├── commands-windows-ssh.h
│   ├── commands.c
│   ├── cutils.c
│   ├── cutils.h
│   ├── guest-agent-command-state.c
│   ├── guest-agent-core.h
│   ├── installer
│   │   └── qemu-ga.wxs
│   ├── main.c
│   ├── meson.build
│   ├── messages-win32.mc
│   ├── qapi-schema.json
│   ├── service-win32.c
│   ├── service-win32.h
│   ├── vss-win32
│   │   ├── install.cpp
│   │   ├── install.h
│   │   ├── meson.build
│   │   ├── provider.cpp
│   │   ├── qga-vss.def
│   │   ├── qga-vss.idl
│   │   ├── requester.cpp
│   │   ├── requester.h
│   │   ├── vss-common.h
│   │   ├── vss-debug.cpp
│   │   ├── vss-debug.h
│   │   └── vss-handles.h
│   ├── vss-win32.c
│   └── vss-win32.h
├── qobject
│   ├── block-qdict.c
│   ├── json-lexer.c
│   ├── json-parser-int.h
│   ├── json-parser.c
│   ├── json-streamer.c
│   ├── json-writer.c
│   ├── meson.build
│   ├── qbool.c
│   ├── qdict.c
│   ├── qjson.c
│   ├── qlist.c
│   ├── qlit.c
│   ├── qnull.c
│   ├── qnum.c
│   ├── qobject-internal.h
│   ├── qobject.c
│   └── qstring.c
├── qom
│   ├── container.c
│   ├── meson.build
│   ├── object_interfaces.c
│   ├── object.c
│   ├── qom-hmp-cmds.c
│   ├── qom-qmp-cmds.c
│   ├── qom-qobject.c
│   ├── trace-events
│   └── trace.h
├── README.rst
├── replay
│   ├── meson.build
│   ├── replay-audio.c
│   ├── replay-char.c
│   ├── replay-debugging.c
│   ├── replay-events.c
│   ├── replay-input.c
│   ├── replay-internal.c
│   ├── replay-internal.h
│   ├── replay-net.c
│   ├── replay-random.c
│   ├── replay-snapshot.c
│   ├── replay-time.c
│   ├── replay.c
│   └── stubs-system.c
├── replication.c
├── roms
│   ├── config.seabios-128k
│   ├── config.seabios-256k
│   ├── config.seabios-microvm
│   ├── config.vga-ati
│   ├── config.vga-bochs-display
│   ├── config.vga-cirrus
│   ├── config.vga-isavga
│   ├── config.vga-qxl
│   ├── config.vga-ramfb
│   ├── config.vga-stdvga
│   ├── config.vga-virtio
│   ├── config.vga-vmware
│   ├── configure-seabios.sh
│   ├── edk2
│   ├── edk2-build.config
│   ├── edk2-build.py
│   ├── edk2-version
│   ├── ipxe
│   ├── Makefile
│   ├── openbios
│   ├── opensbi
│   ├── qboot
│   ├── qemu-palcode
│   ├── QemuMacDrivers
│   ├── seabios
│   ├── seabios-hppa
│   ├── skiboot
│   ├── SLOF
│   ├── u-boot
│   ├── u-boot-sam460ex
│   └── vbootrom
├── rust
│   ├── bits
│   │   ├── Cargo.toml
│   │   ├── meson.build
│   │   └── src
│   │       └── lib.rs
│   ├── Cargo.lock
│   ├── Cargo.toml
│   ├── hw
│   │   ├── char
│   │   │   ├── Kconfig
│   │   │   ├── meson.build
│   │   │   └── pl011
│   │   │       ├── Cargo.toml
│   │   │       ├── meson.build
│   │   │       └── src
│   │   │           ├── device_class.rs
│   │   │           ├── device.rs
│   │   │           ├── lib.rs
│   │   │           └── registers.rs
│   │   ├── Kconfig
│   │   ├── meson.build
│   │   └── timer
│   │       ├── hpet
│   │       │   ├── Cargo.toml
│   │       │   ├── meson.build
│   │       │   └── src
│   │       │       ├── device.rs
│   │       │       ├── fw_cfg.rs
│   │       │       └── lib.rs
│   │       ├── Kconfig
│   │       └── meson.build
│   ├── Kconfig
│   ├── meson.build
│   ├── qemu-api
│   │   ├── build.rs
│   │   ├── Cargo.toml
│   │   ├── meson.build
│   │   ├── README.md
│   │   ├── src
│   │   │   ├── assertions.rs
│   │   │   ├── bindings.rs
│   │   │   ├── bitops.rs
│   │   │   ├── callbacks.rs
│   │   │   ├── cell.rs
│   │   │   ├── chardev.rs
│   │   │   ├── errno.rs
│   │   │   ├── error.rs
│   │   │   ├── irq.rs
│   │   │   ├── lib.rs
│   │   │   ├── log.rs
│   │   │   ├── memory.rs
│   │   │   ├── module.rs
│   │   │   ├── prelude.rs
│   │   │   ├── qdev.rs
│   │   │   ├── qom.rs
│   │   │   ├── sysbus.rs
│   │   │   ├── timer.rs
│   │   │   ├── uninit.rs
│   │   │   ├── vmstate.rs
│   │   │   └── zeroable.rs
│   │   ├── tests
│   │   │   ├── tests.rs
│   │   │   └── vmstate_tests.rs
│   │   └── wrapper.h
│   ├── qemu-api-macros
│   │   ├── Cargo.toml
│   │   ├── meson.build
│   │   └── src
│   │       ├── bits.rs
│   │       ├── lib.rs
│   │       └── utils.rs
│   └── rustfmt.toml
├── scripts
│   ├── analyse-9p-simpletrace.py
│   ├── analyse-locks-simpletrace.py
│   ├── analyze-inclusions
│   ├── analyze-migration.py
│   ├── archive-source.sh
│   ├── block-coroutine-wrapper.py
│   ├── check_sparse.py
│   ├── checkpatch.pl
│   ├── ci
│   │   ├── coverage-summary.sh
│   │   ├── gitlab-ci-section
│   │   ├── gitlab-kubernetes-runners
│   │   │   └── values.yaml
│   │   ├── gitlab-pipeline-status
│   │   └── setup
│   │       ├── gitlab-runner.yml
│   │       ├── inventory.template
│   │       ├── ubuntu
│   │       │   ├── build-environment.yml
│   │       │   ├── ubuntu-2204-aarch64.yaml
│   │       │   ├── ubuntu-2204-armhf-cross.yml
│   │       │   └── ubuntu-2204-s390x.yaml
│   │       └── vars.yml.template
│   ├── clean-header-guards.pl
│   ├── clean-includes
│   ├── cleanup-trace-events.pl
│   ├── cocci-macro-file.h
│   ├── coccinelle
│   │   ├── cpu_restore_state.cocci
│   │   ├── cpu-reset.cocci
│   │   ├── device-reset.cocci
│   │   ├── err-bad-newline.cocci
│   │   ├── error_propagate_null.cocci
│   │   ├── error-use-after-free.cocci
│   │   ├── errp-guard.cocci
│   │   ├── exec_rw_const.cocci
│   │   ├── inplace-byteswaps.cocci
│   │   ├── memory-region-housekeeping.cocci
│   │   ├── overflow_muldiv64.cocci
│   │   ├── qobject.cocci
│   │   ├── qom-parent-type.cocci
│   │   ├── remove_local_err.cocci
│   │   ├── remove_muldiv64.cocci
│   │   ├── reset-type.cocci
│   │   ├── return_directly.cocci
│   │   ├── round.cocci
│   │   ├── simplify_muldiv64.cocci
│   │   ├── swap_muldiv64.cocci
│   │   ├── tcg_gen_extract.cocci
│   │   ├── timer-del-timer-free.cocci
│   │   ├── typecast.cocci
│   │   ├── use-error_fatal.cocci
│   │   └── use-g_new-etc.cocci
│   ├── codeconverter
│   │   ├── codeconverter
│   │   │   ├── __init__.py
│   │   │   ├── patching.py
│   │   │   ├── qom_macros.py
│   │   │   ├── qom_type_info.py
│   │   │   ├── regexps.py
│   │   │   ├── test_patching.py
│   │   │   ├── test_regexps.py
│   │   │   └── utils.py
│   │   └── converter.py
│   ├── compare-machine-types.py
│   ├── coverage
│   │   └── compare_gcov_json.py
│   ├── coverity-scan
│   │   ├── COMPONENTS.md
│   │   ├── coverity-scan.docker
│   │   ├── model.c
│   │   └── run-coverity-scan
│   ├── cpu-x86-uarch-abi.py
│   ├── decodetree.py
│   ├── device-crash-test
│   ├── disas-objdump.pl
│   ├── dump-guest-memory.py
│   ├── entitlement.sh
│   ├── extract-vsssdk-headers
│   ├── feature_to_c.py
│   ├── fix-multiline-comments.sh
│   ├── get_maintainer.pl
│   ├── git-submodule.sh
│   ├── git.orderfile
│   ├── hxtool
│   ├── kernel-doc
│   ├── kvm
│   │   ├── kvm_flightrecorder
│   │   └── vmxcap
│   ├── make-config-poison.sh
│   ├── make-release
│   ├── meson-buildoptions.py
│   ├── meson-buildoptions.sh
│   ├── meson.build
│   ├── minikconf.py
│   ├── modinfo-collect.py
│   ├── modinfo-generate.py
│   ├── modules
│   │   └── module_block.py
│   ├── mtest2make.py
│   ├── nsis.py
│   ├── oss-fuzz
│   │   ├── build.sh
│   │   ├── instrumentation-filter-template
│   │   ├── lsan_suppressions.txt
│   │   ├── minimize_qtest_trace.py
│   │   ├── output_reproducer.py
│   │   └── reorder_fuzzer_qtest_trace.py
│   ├── performance
│   │   ├── dissect.py
│   │   ├── topN_callgrind.py
│   │   └── topN_perf.py
│   ├── probe-gdb-support.py
│   ├── python_qmp_updater.py
│   ├── qapi
│   │   ├── __init__.py
│   │   ├── backend.py
│   │   ├── commands.py
│   │   ├── common.py
│   │   ├── error.py
│   │   ├── events.py
│   │   ├── expr.py
│   │   ├── features.py
│   │   ├── gen.py
│   │   ├── introspect.py
│   │   ├── main.py
│   │   ├── parser.py
│   │   ├── pylintrc
│   │   ├── schema.py
│   │   ├── source.py
│   │   ├── types.py
│   │   └── visit.py
│   ├── qapi-gen.py
│   ├── qcow2-to-stdout.py
│   ├── qemu-binfmt-conf.sh
│   ├── qemu-gdb.py
│   ├── qemu-guest-agent
│   │   ├── fsfreeze-hook
│   │   └── fsfreeze-hook.d
│   │       └── mysql-flush.sh.sample
│   ├── qemu-plugin-symbols.py
│   ├── qemu-stamp.py
│   ├── qemu-trace-stap
│   ├── qemu-version.sh
│   ├── qemugdb
│   │   ├── __init__.py
│   │   ├── aio.py
│   │   ├── coroutine.py
│   │   ├── mtree.py
│   │   ├── tcg.py
│   │   └── timers.py
│   ├── qmp
│   │   ├── qemu-ga-client
│   │   ├── qmp
│   │   ├── qmp-shell
│   │   ├── qmp-shell-wrap
│   │   ├── qom-fuse
│   │   ├── qom-get
│   │   ├── qom-list
│   │   ├── qom-set
│   │   └── qom-tree
│   ├── qom-cast-macro-clean-cocci-gen.py
│   ├── rdma-migration-helper.sh
│   ├── refresh-pxe-roms.sh
│   ├── render_block_graph.py
│   ├── replay-dump.py
│   ├── rust
│   │   ├── rust_root_crate.sh
│   │   └── rustc_args.py
│   ├── shaderinclude.py
│   ├── signrom.py
│   ├── simplebench
│   │   ├── bench_block_job.py
│   │   ├── bench_prealloc.py
│   │   ├── bench_write_req.py
│   │   ├── bench-backup.py
│   │   ├── bench-example.py
│   │   ├── img_bench_templater.py
│   │   ├── results_to_text.py
│   │   ├── simplebench.py
│   │   └── table_templater.py
│   ├── simpletrace.py
│   ├── symlink-install-tree.py
│   ├── tracetool
│   │   ├── __init__.py
│   │   ├── backend
│   │   │   ├── __init__.py
│   │   │   ├── dtrace.py
│   │   │   ├── ftrace.py
│   │   │   ├── log.py
│   │   │   ├── simple.py
│   │   │   ├── syslog.py
│   │   │   └── ust.py
│   │   └── format
│   │       ├── __init__.py
│   │       ├── c.py
│   │       ├── d.py
│   │       ├── h.py
│   │       ├── log_stap.py
│   │       ├── simpletrace_stap.py
│   │       ├── stap.py
│   │       ├── ust_events_c.py
│   │       └── ust_events_h.py
│   ├── tracetool.py
│   ├── u2f-setup-gen.py
│   ├── undefsym.py
│   ├── update-linux-headers.sh
│   ├── update-mips-syscall-args.sh
│   ├── update-syscalltbl.sh
│   ├── userfaultfd-wrlat.py
│   ├── vmstate-static-checker.py
│   ├── xen-detect.c
│   ├── xml-preprocess-test.py
│   └── xml-preprocess.py
├── scsi
│   ├── meson.build
│   ├── pr-helper.h
│   ├── pr-manager-helper.c
│   ├── pr-manager-stub.c
│   ├── pr-manager.c
│   ├── qemu-pr-helper.c
│   ├── trace-events
│   ├── trace.h
│   └── utils.c
├── semihosting
│   ├── arm-compat-semi.c
│   ├── config.c
│   ├── console.c
│   ├── guestfd.c
│   ├── Kconfig
│   ├── meson.build
│   ├── stubs-all.c
│   ├── stubs-system.c
│   ├── syscalls.c
│   ├── uaccess.c
│   └── user.c
├── stats
│   ├── meson.build
│   ├── stats-hmp-cmds.c
│   └── stats-qmp-cmds.c
├── storage-daemon
│   ├── meson.build
│   ├── qapi
│   │   ├── meson.build
│   │   └── qapi-schema.json
│   └── qemu-storage-daemon.c
├── stubs
│   ├── bdrv-next-monitor-owned.c
│   ├── blk-commit-all.c
│   ├── blk-exp-close-all.c
│   ├── blockdev-close-all-bdrv-states.c
│   ├── change-state-handler.c
│   ├── cmos.c
│   ├── cpu-get-clock.c
│   ├── cpu-synchronize-state.c
│   ├── cpus-virtual-clock.c
│   ├── dump.c
│   ├── error-printf.c
│   ├── fdset.c
│   ├── fw_cfg.c
│   ├── gdbstub.c
│   ├── get-vm-name.c
│   ├── graph-lock.c
│   ├── hotplug-stubs.c
│   ├── icount.c
│   ├── io_uring.c
│   ├── iothread-lock-block.c
│   ├── iothread-lock.c
│   ├── is-daemonized.c
│   ├── linux-aio.c
│   ├── meson.build
│   ├── migr-blocker.c
│   ├── monitor-arm-gic.c
│   ├── monitor-core.c
│   ├── monitor-cpu-s390x-kvm.c
│   ├── monitor-cpu-s390x.c
│   ├── monitor-cpu.c
│   ├── monitor-i386-rtc.c
│   ├── monitor-i386-sev.c
│   ├── monitor-i386-sgx.c
│   ├── monitor-i386-xen.c
│   ├── monitor-internal.c
│   ├── physmem.c
│   ├── qdev.c
│   ├── qemu-timer-notify-cb.c
│   ├── qmp-command-available.c
│   ├── qmp-quit.c
│   ├── qtest.c
│   ├── ram-block.c
│   ├── replay-mode.c
│   ├── replay-tools.c
│   ├── replay.c
│   ├── runstate-check.c
│   ├── sysbus.c
│   ├── target-get-monitor-def.c
│   ├── target-monitor-defs.c
│   ├── trace-control.c
│   ├── uuid.c
│   ├── vm-stop.c
│   ├── vmstate.c
│   ├── win32-kbd-hook.c
│   └── xen-hw-stub.c
├── subprojects
│   ├── anyhow-1-rs.wrap
│   ├── arbitrary-int-1-rs.wrap
│   ├── berkeley-softfloat-3.wrap
│   ├── berkeley-testfloat-3.wrap
│   ├── bilge-0.2-rs.wrap
│   ├── bilge-impl-0.2-rs.wrap
│   ├── dtc.wrap
│   ├── either-1-rs.wrap
│   ├── foreign-0.3-rs.wrap
│   ├── itertools-0.11-rs.wrap
│   ├── keycodemapdb.wrap
│   ├── libblkio.wrap
│   ├── libc-0.2-rs.wrap
│   ├── libvduse
│   │   ├── include
│   │   │   ├── atomic.h -> ../../../include/qemu/atomic.h
│   │   │   └── compiler.h -> ../../../include/qemu/compiler.h
│   │   ├── libvduse.c
│   │   ├── libvduse.h
│   │   ├── linux-headers
│   │   │   └── linux -> ../../../linux-headers/linux/
│   │   ├── meson.build
│   │   └── standard-headers
│   │       └── linux -> ../../../include/standard-headers/linux/
│   ├── libvfio-user.wrap
│   ├── libvhost-user
│   │   ├── include
│   │   │   ├── atomic.h -> ../../../include/qemu/atomic.h
│   │   │   └── compiler.h -> ../../../include/qemu/compiler.h
│   │   ├── libvhost-user-glib.c
│   │   ├── libvhost-user-glib.h
│   │   ├── libvhost-user.c
│   │   ├── libvhost-user.h
│   │   ├── link-test.c
│   │   ├── meson.build
│   │   └── standard-headers
│   │       └── linux -> ../../../include/standard-headers/linux
│   ├── packagefiles
│   │   ├── anyhow-1-rs
│   │   │   └── meson.build
│   │   ├── arbitrary-int-1-rs
│   │   │   └── meson.build
│   │   ├── berkeley-softfloat-3
│   │   │   ├── meson_options.txt
│   │   │   └── meson.build
│   │   ├── berkeley-testfloat-3
│   │   │   ├── meson_options.txt
│   │   │   └── meson.build
│   │   ├── bilge-0.2-rs
│   │   │   └── meson.build
│   │   ├── bilge-impl-0.2-rs
│   │   │   └── meson.build
│   │   ├── either-1-rs
│   │   │   └── meson.build
│   │   ├── foreign-0.3-rs
│   │   │   └── meson.build
│   │   ├── itertools-0.11-rs
│   │   │   └── meson.build
│   │   ├── libc-0.2-rs
│   │   │   └── meson.build
│   │   ├── proc-macro-error-1-rs
│   │   │   └── meson.build
│   │   ├── proc-macro-error-attr-1-rs
│   │   │   └── meson.build
│   │   ├── proc-macro2-1-rs
│   │   │   └── meson.build
│   │   ├── quote-1-rs
│   │   │   └── meson.build
│   │   ├── syn-2-rs
│   │   │   └── meson.build
│   │   └── unicode-ident-1-rs
│   │       └── meson.build
│   ├── proc-macro-error-1-rs.wrap
│   ├── proc-macro-error-attr-1-rs.wrap
│   ├── proc-macro2-1-rs.wrap
│   ├── quote-1-rs.wrap
│   ├── slirp.wrap
│   ├── syn-2-rs.wrap
│   └── unicode-ident-1-rs.wrap
├── system
│   ├── arch_init.c
│   ├── async-teardown.c
│   ├── balloon.c
│   ├── bootdevice.c
│   ├── cpu-timers.c
│   ├── cpus.c
│   ├── datadir.c
│   ├── device_tree-stub.c
│   ├── device_tree.c
│   ├── dirtylimit.c
│   ├── dma-helpers.c
│   ├── globals-target.c
│   ├── globals.c
│   ├── ioport.c
│   ├── main.c
│   ├── memory_ldst.c.inc
│   ├── memory_mapping.c
│   ├── memory-internal.h
│   ├── memory.c
│   ├── meson.build
│   ├── physmem.c
│   ├── qdev-monitor.c
│   ├── qemu-seccomp.c
│   ├── qtest.c
│   ├── ram-block-attributes.c
│   ├── rtc.c
│   ├── runstate-action.c
│   ├── runstate-hmp-cmds.c
│   ├── runstate.c
│   ├── tpm-hmp-cmds.c
│   ├── tpm.c
│   ├── trace-events
│   ├── trace.h
│   ├── vl.c
│   └── watchpoint.c
├── target
│   ├── alpha
│   │   ├── clk_helper.c
│   │   ├── cpu-param.h
│   │   ├── cpu-qom.h
│   │   ├── cpu.c
│   │   ├── cpu.h
│   │   ├── fpu_helper.c
│   │   ├── gdbstub.c
│   │   ├── helper.c
│   │   ├── helper.h
│   │   ├── int_helper.c
│   │   ├── Kconfig
│   │   ├── machine.c
│   │   ├── mem_helper.c
│   │   ├── meson.build
│   │   ├── sys_helper.c
│   │   ├── translate.c
│   │   └── vax_helper.c
│   ├── arm
│   │   ├── arch_dump.c
│   │   ├── arm-powerctl.c
│   │   ├── arm-powerctl.h
│   │   ├── arm-qmp-cmds.c
│   │   ├── common-semi-target.h
│   │   ├── cortex-regs.c
│   │   ├── cpregs.h
│   │   ├── cpu-features.h
│   │   ├── cpu-param.h
│   │   ├── cpu-qom.h
│   │   ├── cpu.c
│   │   ├── cpu.h
│   │   ├── cpu32-stubs.c
│   │   ├── cpu64.c
│   │   ├── debug_helper.c
│   │   ├── gdbstub.c
│   │   ├── gdbstub64.c
│   │   ├── gtimer.h
│   │   ├── helper.c
│   │   ├── helper.h
│   │   ├── hvf
│   │   │   ├── hvf.c
│   │   │   ├── meson.build
│   │   │   ├── trace-events
│   │   │   └── trace.h
│   │   ├── hvf_arm.h
│   │   ├── hvf-stub.c
│   │   ├── hyp_gdbstub.c
│   │   ├── idau.h
│   │   ├── internals.h
│   │   ├── Kconfig
│   │   ├── kvm_arm.h
│   │   ├── kvm-consts.h
│   │   ├── kvm-stub.c
│   │   ├── kvm.c
│   │   ├── machine.c
│   │   ├── meson.build
│   │   ├── multiprocessing.h
│   │   ├── ptw.c
│   │   ├── syndrome.h
│   │   ├── tcg
│   │   │   ├── a32-uncond.decode
│   │   │   ├── a32.decode
│   │   │   ├── a64.decode
│   │   │   ├── arith_helper.c
│   │   │   ├── arm_ldst.h
│   │   │   ├── cpu-v7m.c
│   │   │   ├── cpu32.c
│   │   │   ├── cpu64.c
│   │   │   ├── crypto_helper.c
│   │   │   ├── gengvec.c
│   │   │   ├── gengvec64.c
│   │   │   ├── helper-a64.c
│   │   │   ├── helper-a64.h
│   │   │   ├── helper-mve.h
│   │   │   ├── helper-sme.h
│   │   │   ├── helper-sve.h
│   │   │   ├── helper.h
│   │   │   ├── hflags.c
│   │   │   ├── iwmmxt_helper.c
│   │   │   ├── m_helper.c
│   │   │   ├── m-nocp.decode
│   │   │   ├── meson.build
│   │   │   ├── mte_helper.c
│   │   │   ├── mte_helper.h
│   │   │   ├── mve_helper.c
│   │   │   ├── mve.decode
│   │   │   ├── neon_helper.c
│   │   │   ├── neon-dp.decode
│   │   │   ├── neon-ls.decode
│   │   │   ├── neon-shared.decode
│   │   │   ├── op_addsub.c.inc
│   │   │   ├── op_helper.c
│   │   │   ├── pauth_helper.c
│   │   │   ├── psci.c
│   │   │   ├── sme_helper.c
│   │   │   ├── sme-fa64.decode
│   │   │   ├── sme.decode
│   │   │   ├── sve_helper.c
│   │   │   ├── sve_ldst_internal.h
│   │   │   ├── sve.decode
│   │   │   ├── t16.decode
│   │   │   ├── t32.decode
│   │   │   ├── tlb_helper.c
│   │   │   ├── tlb-insns.c
│   │   │   ├── translate-a32.h
│   │   │   ├── translate-a64.c
│   │   │   ├── translate-a64.h
│   │   │   ├── translate-m-nocp.c
│   │   │   ├── translate-mve.c
│   │   │   ├── translate-neon.c
│   │   │   ├── translate-sme.c
│   │   │   ├── translate-sve.c
│   │   │   ├── translate-vfp.c
│   │   │   ├── translate.c
│   │   │   ├── translate.h
│   │   │   ├── vec_helper.c
│   │   │   ├── vec_internal.h
│   │   │   ├── vfp_helper.c
│   │   │   ├── vfp-uncond.decode
│   │   │   └── vfp.decode
│   │   ├── tcg-stubs.c
│   │   ├── trace-events
│   │   ├── trace.h
│   │   └── vfp_fpscr.c
│   ├── avr
│   │   ├── cpu-param.h
│   │   ├── cpu-qom.h
│   │   ├── cpu.c
│   │   ├── cpu.h
│   │   ├── disas.c
│   │   ├── gdbstub.c
│   │   ├── helper.c
│   │   ├── helper.h
│   │   ├── insn.decode
│   │   ├── Kconfig
│   │   ├── machine.c
│   │   ├── meson.build
│   │   └── translate.c
│   ├── hexagon
│   │   ├── arch.c
│   │   ├── arch.h
│   │   ├── attribs_def.h.inc
│   │   ├── attribs.h
│   │   ├── cpu_bits.h
│   │   ├── cpu-param.h
│   │   ├── cpu-qom.h
│   │   ├── cpu.c
│   │   ├── cpu.h
│   │   ├── decode.c
│   │   ├── decode.h
│   │   ├── fma_emu.c
│   │   ├── fma_emu.h
│   │   ├── gdbstub.c
│   │   ├── gen_analyze_funcs.py
│   │   ├── gen_decodetree.py
│   │   ├── gen_dectree_import.c
│   │   ├── gen_helper_funcs.py
│   │   ├── gen_helper_protos.py
│   │   ├── gen_idef_parser_funcs.py
│   │   ├── gen_op_attribs.py
│   │   ├── gen_opcodes_def.py
│   │   ├── gen_printinsn.py
│   │   ├── gen_semantics.c
│   │   ├── gen_tcg_func_table.py
│   │   ├── gen_tcg_funcs.py
│   │   ├── gen_tcg_hvx.h
│   │   ├── gen_tcg.h
│   │   ├── gen_trans_funcs.py
│   │   ├── genptr.c
│   │   ├── genptr.h
│   │   ├── helper.h
│   │   ├── hex_arch_types.h
│   │   ├── hex_common.py
│   │   ├── hex_regs.h
│   │   ├── iclass.c
│   │   ├── iclass.h
│   │   ├── idef-parser
│   │   │   ├── idef-parser.h
│   │   │   ├── idef-parser.lex
│   │   │   ├── idef-parser.y
│   │   │   ├── macros.h.inc
│   │   │   ├── parser-helpers.c
│   │   │   ├── parser-helpers.h
│   │   │   ├── prepare
│   │   │   └── README.rst
│   │   ├── imported
│   │   │   ├── allext_macros.def
│   │   │   ├── allext.idef
│   │   │   ├── allextenc.def
│   │   │   ├── allidefs.def
│   │   │   ├── alu.idef
│   │   │   ├── branch.idef
│   │   │   ├── compare.idef
│   │   │   ├── encode_pp.def
│   │   │   ├── encode_subinsn.def
│   │   │   ├── encode.def
│   │   │   ├── float.idef
│   │   │   ├── iclass.def
│   │   │   ├── ldst.idef
│   │   │   ├── macros.def
│   │   │   ├── mmvec
│   │   │   │   ├── encode_ext.def
│   │   │   │   ├── ext.idef
│   │   │   │   └── macros.def
│   │   │   ├── mpy.idef
│   │   │   ├── shift.idef
│   │   │   ├── subinsns.idef
│   │   │   └── system.idef
│   │   ├── insn.h
│   │   ├── internal.h
│   │   ├── macros.h
│   │   ├── meson.build
│   │   ├── mmvec
│   │   │   ├── decode_ext_mmvec.c
│   │   │   ├── decode_ext_mmvec.h
│   │   │   ├── macros.h
│   │   │   ├── mmvec.h
│   │   │   ├── system_ext_mmvec.c
│   │   │   └── system_ext_mmvec.h
│   │   ├── op_helper.c
│   │   ├── op_helper.h
│   │   ├── opcodes.c
│   │   ├── opcodes.h
│   │   ├── printinsn.c
│   │   ├── printinsn.h
│   │   ├── README
│   │   ├── reg_fields_def.h.inc
│   │   ├── reg_fields.c
│   │   ├── reg_fields.h
│   │   ├── translate.c
│   │   └── translate.h
│   ├── hppa
│   │   ├── cpu-param.h
│   │   ├── cpu-qom.h
│   │   ├── cpu.c
│   │   ├── cpu.h
│   │   ├── fpu_helper.c
│   │   ├── gdbstub.c
│   │   ├── helper.c
│   │   ├── helper.h
│   │   ├── insns.decode
│   │   ├── int_helper.c
│   │   ├── Kconfig
│   │   ├── machine.c
│   │   ├── mem_helper.c
│   │   ├── meson.build
│   │   ├── op_helper.c
│   │   ├── sys_helper.c
│   │   ├── trace-events
│   │   ├── trace.h
│   │   └── translate.c
│   ├── i386
│   │   ├── arch_dump.c
│   │   ├── arch_memory_mapping.c
│   │   ├── confidential-guest.c
│   │   ├── confidential-guest.h
│   │   ├── cpu-apic.c
│   │   ├── cpu-dump.c
│   │   ├── cpu-internal.h
│   │   ├── cpu-param.h
│   │   ├── cpu-qom.h
│   │   ├── cpu-system.c
│   │   ├── cpu.c
│   │   ├── cpu.h
│   │   ├── emulate
│   │   │   ├── meson.build
│   │   │   ├── panic.h
│   │   │   ├── x86_decode.c
│   │   │   ├── x86_decode.h
│   │   │   ├── x86_emu.c
│   │   │   ├── x86_emu.h
│   │   │   ├── x86_flags.c
│   │   │   ├── x86_flags.h
│   │   │   └── x86.h
│   │   ├── gdbstub.c
│   │   ├── helper.c
│   │   ├── helper.h
│   │   ├── host-cpu.c
│   │   ├── host-cpu.h
│   │   ├── hvf
│   │   │   ├── hvf-cpu.c
│   │   │   ├── hvf-i386.h
│   │   │   ├── hvf.c
│   │   │   ├── meson.build
│   │   │   ├── panic.h
│   │   │   ├── README.md
│   │   │   ├── vmcs.h
│   │   │   ├── vmx.h
│   │   │   ├── x86_cpuid.c
│   │   │   ├── x86_descr.c
│   │   │   ├── x86_descr.h
│   │   │   ├── x86_mmu.c
│   │   │   ├── x86_mmu.h
│   │   │   ├── x86_task.c
│   │   │   ├── x86_task.h
│   │   │   ├── x86.c
│   │   │   ├── x86hvf.c
│   │   │   └── x86hvf.h
│   │   ├── Kconfig
│   │   ├── kvm
│   │   │   ├── hyperv-proto.h
│   │   │   ├── hyperv-stub.c
│   │   │   ├── hyperv.c
│   │   │   ├── hyperv.h
│   │   │   ├── kvm_i386.h
│   │   │   ├── kvm-cpu.c
│   │   │   ├── kvm.c
│   │   │   ├── meson.build
│   │   │   ├── tdx-quote-generator.c
│   │   │   ├── tdx-quote-generator.h
│   │   │   ├── tdx-stub.c
│   │   │   ├── tdx.c
│   │   │   ├── tdx.h
│   │   │   ├── trace-events
│   │   │   ├── trace.h
│   │   │   ├── vmsr_energy.c
│   │   │   ├── vmsr_energy.h
│   │   │   ├── xen-compat.h
│   │   │   ├── xen-emu.c
│   │   │   └── xen-emu.h
│   │   ├── machine.c
│   │   ├── meson.build
│   │   ├── monitor.c
│   │   ├── nvmm
│   │   │   ├── meson.build
│   │   │   ├── nvmm-accel-ops.c
│   │   │   ├── nvmm-accel-ops.h
│   │   │   └── nvmm-all.c
│   │   ├── ops_sse.h
│   │   ├── sev-system-stub.c
│   │   ├── sev.c
│   │   ├── sev.h
│   │   ├── svm.h
│   │   ├── tcg
│   │   │   ├── access.c
│   │   │   ├── access.h
│   │   │   ├── bpt_helper.c
│   │   │   ├── cc_helper_template.h.inc
│   │   │   ├── cc_helper.c
│   │   │   ├── decode-new.c.inc
│   │   │   ├── decode-new.h
│   │   │   ├── emit.c.inc
│   │   │   ├── excp_helper.c
│   │   │   ├── fpu_helper.c
│   │   │   ├── helper-tcg.h
│   │   │   ├── int_helper.c
│   │   │   ├── mem_helper.c
│   │   │   ├── meson.build
│   │   │   ├── misc_helper.c
│   │   │   ├── mpx_helper.c
│   │   │   ├── ops_sse_header.h.inc
│   │   │   ├── seg_helper.c
│   │   │   ├── seg_helper.h
│   │   │   ├── system
│   │   │   │   ├── bpt_helper.c
│   │   │   │   ├── excp_helper.c
│   │   │   │   ├── fpu_helper.c
│   │   │   │   ├── meson.build
│   │   │   │   ├── misc_helper.c
│   │   │   │   ├── seg_helper.c
│   │   │   │   ├── smm_helper.c
│   │   │   │   ├── svm_helper.c
│   │   │   │   └── tcg-cpu.c
│   │   │   ├── tcg-cpu.c
│   │   │   ├── tcg-cpu.h
│   │   │   ├── tcg-stub.c
│   │   │   ├── translate.c
│   │   │   └── user
│   │   │       ├── excp_helper.c
│   │   │       ├── meson.build
│   │   │       └── seg_helper.c
│   │   ├── trace-events
│   │   ├── trace.h
│   │   ├── whpx
│   │   │   ├── meson.build
│   │   │   ├── whpx-accel-ops.c
│   │   │   ├── whpx-accel-ops.h
│   │   │   ├── whpx-all.c
│   │   │   ├── whpx-apic.c
│   │   │   └── whpx-internal.h
│   │   └── xsave_helper.c
│   ├── Kconfig
│   ├── loongarch
│   │   ├── arch_dump.c
│   │   ├── cpu_helper.c
│   │   ├── cpu-csr.h
│   │   ├── cpu-param.h
│   │   ├── cpu-qom.h
│   │   ├── cpu.c
│   │   ├── cpu.h
│   │   ├── csr.c
│   │   ├── csr.h
│   │   ├── disas.c
│   │   ├── gdbstub.c
│   │   ├── helper.h
│   │   ├── insns.decode
│   │   ├── internals.h
│   │   ├── Kconfig
│   │   ├── kvm
│   │   │   ├── kvm_loongarch.h
│   │   │   ├── kvm.c
│   │   │   └── meson.build
│   │   ├── loongarch-qmp-cmds.c
│   │   ├── machine.c
│   │   ├── meson.build
│   │   ├── README
│   │   ├── tcg
│   │   │   ├── constant_timer.c
│   │   │   ├── csr_helper.c
│   │   │   ├── fpu_helper.c
│   │   │   ├── helper.h
│   │   │   ├── insn_trans
│   │   │   │   ├── trans_arith.c.inc
│   │   │   │   ├── trans_atomic.c.inc
│   │   │   │   ├── trans_bit.c.inc
│   │   │   │   ├── trans_branch.c.inc
│   │   │   │   ├── trans_extra.c.inc
│   │   │   │   ├── trans_farith.c.inc
│   │   │   │   ├── trans_fcmp.c.inc
│   │   │   │   ├── trans_fcnv.c.inc
│   │   │   │   ├── trans_fmemory.c.inc
│   │   │   │   ├── trans_fmov.c.inc
│   │   │   │   ├── trans_memory.c.inc
│   │   │   │   ├── trans_privileged.c.inc
│   │   │   │   ├── trans_shift.c.inc
│   │   │   │   └── trans_vec.c.inc
│   │   │   ├── iocsr_helper.c
│   │   │   ├── meson.build
│   │   │   ├── op_helper.c
│   │   │   ├── tcg_loongarch.h
│   │   │   ├── tlb_helper.c
│   │   │   ├── translate.c
│   │   │   └── vec_helper.c
│   │   ├── trace-events
│   │   ├── trace.h
│   │   ├── translate.h
│   │   └── vec.h
│   ├── m68k
│   │   ├── cpu-param.h
│   │   ├── cpu-qom.h
│   │   ├── cpu.c
│   │   ├── cpu.h
│   │   ├── fpu_helper.c
│   │   ├── gdbstub.c
│   │   ├── helper.c
│   │   ├── helper.h
│   │   ├── Kconfig
│   │   ├── m68k-semi.c
│   │   ├── meson.build
│   │   ├── monitor.c
│   │   ├── op_helper.c
│   │   ├── qregs.h.inc
│   │   ├── semihosting-stub.c
│   │   ├── softfloat_fpsp_tables.h
│   │   ├── softfloat.c
│   │   ├── softfloat.h
│   │   └── translate.c
│   ├── meson.build
│   ├── microblaze
│   │   ├── cpu-param.h
│   │   ├── cpu-qom.h
│   │   ├── cpu.c
│   │   ├── cpu.h
│   │   ├── gdbstub.c
│   │   ├── helper.c
│   │   ├── helper.h
│   │   ├── insns.decode
│   │   ├── Kconfig
│   │   ├── machine.c
│   │   ├── meson.build
│   │   ├── mmu.c
│   │   ├── mmu.h
│   │   ├── op_helper.c
│   │   └── translate.c
│   ├── mips
│   │   ├── cpu-defs.c.inc
│   │   ├── cpu-param.h
│   │   ├── cpu-qom.h
│   │   ├── cpu.c
│   │   ├── cpu.h
│   │   ├── fpu_helper.h
│   │   ├── fpu.c
│   │   ├── gdbstub.c
│   │   ├── helper.h
│   │   ├── internal.h
│   │   ├── Kconfig
│   │   ├── kvm_mips.h
│   │   ├── kvm.c
│   │   ├── meson.build
│   │   ├── mips-defs.h
│   │   ├── msa.c
│   │   ├── system
│   │   │   ├── addr.c
│   │   │   ├── cp0_timer.c
│   │   │   ├── cp0.c
│   │   │   ├── machine.c
│   │   │   ├── meson.build
│   │   │   ├── mips-qmp-cmds.c
│   │   │   └── physaddr.c
│   │   └── tcg
│   │       ├── dsp_helper.c
│   │       ├── exception.c
│   │       ├── fpu_helper.c
│   │       ├── godson2.decode
│   │       ├── lcsr_translate.c
│   │       ├── lcsr.decode
│   │       ├── ldst_helper.c
│   │       ├── lmmi_helper.c
│   │       ├── loong_translate.c
│   │       ├── loong-ext.decode
│   │       ├── meson.build
│   │       ├── micromips_translate.c.inc
│   │       ├── mips16e_translate.c.inc
│   │       ├── msa_helper.c
│   │       ├── msa_helper.h.inc
│   │       ├── msa_translate.c
│   │       ├── msa.decode
│   │       ├── mxu_translate.c
│   │       ├── nanomips_translate.c.inc
│   │       ├── octeon_translate.c
│   │       ├── octeon.decode
│   │       ├── op_helper.c
│   │       ├── rel6_translate.c
│   │       ├── rel6.decode
│   │       ├── system
│   │       │   ├── cp0_helper.c
│   │       │   ├── lcsr_helper.c
│   │       │   ├── meson.build
│   │       │   ├── mips-semi.c
│   │       │   ├── semihosting-stub.c
│   │       │   ├── special_helper.c
│   │       │   └── tlb_helper.c
│   │       ├── system_helper.h.inc
│   │       ├── tcg-internal.h
│   │       ├── trace-events
│   │       ├── trace.h
│   │       ├── translate_addr_const.c
│   │       ├── translate.c
│   │       ├── translate.h
│   │       ├── tx79_translate.c
│   │       ├── tx79.decode
│   │       ├── txx9_translate.c
│   │       ├── vr54xx_helper.c
│   │       ├── vr54xx_helper.h.inc
│   │       ├── vr54xx_translate.c
│   │       └── vr54xx.decode
│   ├── openrisc
│   │   ├── cpu-param.h
│   │   ├── cpu-qom.h
│   │   ├── cpu.c
│   │   ├── cpu.h
│   │   ├── disas.c
│   │   ├── exception_helper.c
│   │   ├── exception.c
│   │   ├── exception.h
│   │   ├── fpu_helper.c
│   │   ├── gdbstub.c
│   │   ├── helper.h
│   │   ├── insns.decode
│   │   ├── interrupt_helper.c
│   │   ├── interrupt.c
│   │   ├── Kconfig
│   │   ├── machine.c
│   │   ├── meson.build
│   │   ├── mmu.c
│   │   ├── sys_helper.c
│   │   └── translate.c
│   ├── ppc
│   │   ├── arch_dump.c
│   │   ├── compat.c
│   │   ├── cpu_init.c
│   │   ├── cpu_init.h
│   │   ├── cpu-models.c
│   │   ├── cpu-models.h
│   │   ├── cpu-param.h
│   │   ├── cpu-qom.h
│   │   ├── cpu.c
│   │   ├── cpu.h
│   │   ├── dfp_helper.c
│   │   ├── excp_helper.c
│   │   ├── fpu_helper.c
│   │   ├── gdbstub.c
│   │   ├── helper_regs.c
│   │   ├── helper_regs.h
│   │   ├── helper.h
│   │   ├── insn32.decode
│   │   ├── insn64.decode
│   │   ├── int_helper.c
│   │   ├── internal.h
│   │   ├── Kconfig
│   │   ├── kvm_ppc.h
│   │   ├── kvm.c
│   │   ├── machine.c
│   │   ├── mem_helper.c
│   │   ├── meson.build
│   │   ├── misc_helper.c
│   │   ├── mmu_common.c
│   │   ├── mmu_helper.c
│   │   ├── mmu-book3s-v3.c
│   │   ├── mmu-book3s-v3.h
│   │   ├── mmu-booke.c
│   │   ├── mmu-booke.h
│   │   ├── mmu-books.h
│   │   ├── mmu-hash32.c
│   │   ├── mmu-hash32.h
│   │   ├── mmu-hash64.c
│   │   ├── mmu-hash64.h
│   │   ├── mmu-radix64.c
│   │   ├── mmu-radix64.h
│   │   ├── power8-pmu-regs.c.inc
│   │   ├── power8-pmu.c
│   │   ├── power8-pmu.h
│   │   ├── ppc-qmp-cmds.c
│   │   ├── spr_common.h
│   │   ├── tcg-excp_helper.c
│   │   ├── tcg-stub.c
│   │   ├── timebase_helper.c
│   │   ├── trace-events
│   │   ├── trace.h
│   │   ├── translate
│   │   │   ├── bhrb-impl.c.inc
│   │   │   ├── branch-impl.c.inc
│   │   │   ├── dfp-impl.c.inc
│   │   │   ├── fixedpoint-impl.c.inc
│   │   │   ├── fp-impl.c.inc
│   │   │   ├── fp-ops.c.inc
│   │   │   ├── misc-impl.c.inc
│   │   │   ├── processor-ctrl-impl.c.inc
│   │   │   ├── spe-impl.c.inc
│   │   │   ├── spe-ops.c.inc
│   │   │   ├── storage-ctrl-impl.c.inc
│   │   │   ├── vmx-impl.c.inc
│   │   │   ├── vmx-ops.c.inc
│   │   │   ├── vsx-impl.c.inc
│   │   │   └── vsx-ops.c.inc
│   │   ├── translate.c
│   │   └── user_only_helper.c
│   ├── riscv
│   │   ├── arch_dump.c
│   │   ├── bitmanip_helper.c
│   │   ├── common-semi-target.h
│   │   ├── cpu_bits.h
│   │   ├── cpu_cfg_fields.h.inc
│   │   ├── cpu_cfg.h
│   │   ├── cpu_helper.c
│   │   ├── cpu_user.h
│   │   ├── cpu_vendorid.h
│   │   ├── cpu-param.h
│   │   ├── cpu-qom.h
│   │   ├── cpu.c
│   │   ├── cpu.h
│   │   ├── crypto_helper.c
│   │   ├── csr.c
│   │   ├── debug.c
│   │   ├── debug.h
│   │   ├── fpu_helper.c
│   │   ├── gdbstub.c
│   │   ├── helper.h
│   │   ├── insn_trans
│   │   │   ├── trans_privileged.c.inc
│   │   │   ├── trans_rva.c.inc
│   │   │   ├── trans_rvb.c.inc
│   │   │   ├── trans_rvbf16.c.inc
│   │   │   ├── trans_rvd.c.inc
│   │   │   ├── trans_rvf.c.inc
│   │   │   ├── trans_rvh.c.inc
│   │   │   ├── trans_rvi.c.inc
│   │   │   ├── trans_rvk.c.inc
│   │   │   ├── trans_rvm.c.inc
│   │   │   ├── trans_rvv.c.inc
│   │   │   ├── trans_rvvk.c.inc
│   │   │   ├── trans_rvzabha.c.inc
│   │   │   ├── trans_rvzacas.c.inc
│   │   │   ├── trans_rvzawrs.c.inc
│   │   │   ├── trans_rvzce.c.inc
│   │   │   ├── trans_rvzcmop.c.inc
│   │   │   ├── trans_rvzfa.c.inc
│   │   │   ├── trans_rvzfh.c.inc
│   │   │   ├── trans_rvzicbo.c.inc
│   │   │   ├── trans_rvzicfiss.c.inc
│   │   │   ├── trans_rvzicond.c.inc
│   │   │   ├── trans_rvzimop.c.inc
│   │   │   ├── trans_svinval.c.inc
│   │   │   ├── trans_xthead.c.inc
│   │   │   └── trans_xventanacondops.c.inc
│   │   ├── insn16.decode
│   │   ├── insn32.decode
│   │   ├── instmap.h
│   │   ├── internals.h
│   │   ├── Kconfig
│   │   ├── kvm
│   │   │   ├── kvm_riscv.h
│   │   │   ├── kvm-cpu.c
│   │   │   └── meson.build
│   │   ├── m128_helper.c
│   │   ├── machine.c
│   │   ├── meson.build
│   │   ├── monitor.c
│   │   ├── op_helper.c
│   │   ├── pmp.c
│   │   ├── pmp.h
│   │   ├── pmu.c
│   │   ├── pmu.h
│   │   ├── riscv-qmp-cmds.c
│   │   ├── sbi_ecall_interface.h
│   │   ├── tcg
│   │   │   ├── meson.build
│   │   │   ├── tcg-cpu.c
│   │   │   └── tcg-cpu.h
│   │   ├── th_csr.c
│   │   ├── time_helper.c
│   │   ├── time_helper.h
│   │   ├── trace-events
│   │   ├── trace.h
│   │   ├── translate.c
│   │   ├── vcrypto_helper.c
│   │   ├── vector_helper.c
│   │   ├── vector_internals.c
│   │   ├── vector_internals.h
│   │   ├── xthead.decode
│   │   ├── XVentanaCondOps.decode
│   │   └── zce_helper.c
│   ├── rx
│   │   ├── cpu-param.h
│   │   ├── cpu-qom.h
│   │   ├── cpu.c
│   │   ├── cpu.h
│   │   ├── disas.c
│   │   ├── gdbstub.c
│   │   ├── helper.c
│   │   ├── helper.h
│   │   ├── insns.decode
│   │   ├── Kconfig
│   │   ├── meson.build
│   │   ├── op_helper.c
│   │   └── translate.c
│   ├── s390x
│   │   ├── arch_dump.c
│   │   ├── cpu_features_def.h
│   │   ├── cpu_features_def.h.inc
│   │   ├── cpu_features.c
│   │   ├── cpu_features.h
│   │   ├── cpu_models_system.c
│   │   ├── cpu_models_user.c
│   │   ├── cpu_models.c
│   │   ├── cpu_models.h
│   │   ├── cpu-dump.c
│   │   ├── cpu-param.h
│   │   ├── cpu-qom.h
│   │   ├── cpu-system.c
│   │   ├── cpu.c
│   │   ├── cpu.h
│   │   ├── diag.c
│   │   ├── gdbstub.c
│   │   ├── gen-features.c
│   │   ├── helper.c
│   │   ├── helper.h
│   │   ├── interrupt.c
│   │   ├── ioinst.c
│   │   ├── Kconfig
│   │   ├── kvm
│   │   │   ├── kvm_s390x.h
│   │   │   ├── kvm.c
│   │   │   ├── meson.build
│   │   │   ├── pv.c
│   │   │   ├── pv.h
│   │   │   ├── stsi-topology.c
│   │   │   ├── stubs.c
│   │   │   ├── trace-events
│   │   │   └── trace.h
│   │   ├── machine.c
│   │   ├── meson.build
│   │   ├── mmu_helper.c
│   │   ├── s390x-internal.h
│   │   ├── sigp.c
│   │   ├── tcg
│   │   │   ├── cc_helper.c
│   │   │   ├── crypto_helper.c
│   │   │   ├── excp_helper.c
│   │   │   ├── fpu_helper.c
│   │   │   ├── insn-data.h.inc
│   │   │   ├── insn-format.h.inc
│   │   │   ├── int_helper.c
│   │   │   ├── mem_helper.c
│   │   │   ├── meson.build
│   │   │   ├── misc_helper.c
│   │   │   ├── s390-tod.h
│   │   │   ├── tcg_s390x.h
│   │   │   ├── translate_vx.c.inc
│   │   │   ├── translate.c
│   │   │   ├── vec_fpu_helper.c
│   │   │   ├── vec_helper.c
│   │   │   ├── vec_int_helper.c
│   │   │   ├── vec_string_helper.c
│   │   │   └── vec.h
│   │   ├── trace-events
│   │   └── trace.h
│   ├── sh4
│   │   ├── cpu-param.h
│   │   ├── cpu-qom.h
│   │   ├── cpu.c
│   │   ├── cpu.h
│   │   ├── gdbstub.c
│   │   ├── helper.c
│   │   ├── helper.h
│   │   ├── Kconfig
│   │   ├── meson.build
│   │   ├── monitor.c
│   │   ├── op_helper.c
│   │   └── translate.c
│   ├── sparc
│   │   ├── asi.h
│   │   ├── cpu-feature.h.inc
│   │   ├── cpu-param.h
│   │   ├── cpu-qom.h
│   │   ├── cpu.c
│   │   ├── cpu.h
│   │   ├── fop_helper.c
│   │   ├── gdbstub.c
│   │   ├── helper.c
│   │   ├── helper.h
│   │   ├── insns.decode
│   │   ├── int32_helper.c
│   │   ├── int64_helper.c
│   │   ├── Kconfig
│   │   ├── ldst_helper.c
│   │   ├── machine.c
│   │   ├── meson.build
│   │   ├── mmu_helper.c
│   │   ├── monitor.c
│   │   ├── trace-events
│   │   ├── trace.h
│   │   ├── translate.c
│   │   ├── translate.h
│   │   ├── vis_helper.c
│   │   └── win_helper.c
│   ├── tricore
│   │   ├── cpu-param.h
│   │   ├── cpu-qom.h
│   │   ├── cpu.c
│   │   ├── cpu.h
│   │   ├── csfr.h.inc
│   │   ├── fpu_helper.c
│   │   ├── gdbstub.c
│   │   ├── helper.c
│   │   ├── helper.h
│   │   ├── Kconfig
│   │   ├── meson.build
│   │   ├── op_helper.c
│   │   ├── translate.c
│   │   ├── tricore-defs.h
│   │   └── tricore-opcodes.h
│   └── xtensa
│       ├── core-dc232b
│       │   ├── core-isa.h
│       │   ├── gdb-config.c.inc
│       │   └── xtensa-modules.c.inc
│       ├── core-dc232b.c
│       ├── core-dc233c
│       │   ├── core-isa.h
│       │   ├── gdb-config.c.inc
│       │   └── xtensa-modules.c.inc
│       ├── core-dc233c.c
│       ├── core-de212
│       │   ├── core-isa.h
│       │   ├── gdb-config.c.inc
│       │   └── xtensa-modules.c.inc
│       ├── core-de212.c
│       ├── core-de233_fpu
│       │   ├── core-isa.h
│       │   ├── core-matmap.h
│       │   ├── gdb-config.c.inc
│       │   └── xtensa-modules.c.inc
│       ├── core-de233_fpu.c
│       ├── core-dsp3400
│       │   ├── core-isa.h
│       │   ├── core-matmap.h
│       │   ├── gdb-config.c.inc
│       │   └── xtensa-modules.c.inc
│       ├── core-dsp3400.c
│       ├── core-fsf
│       │   ├── core-isa.h
│       │   └── xtensa-modules.c.inc
│       ├── core-fsf.c
│       ├── core-lx106
│       │   ├── core-isa.h
│       │   ├── gdb-config.c.inc
│       │   └── xtensa-modules.c.inc
│       ├── core-lx106.c
│       ├── core-sample_controller
│       │   ├── core-isa.h
│       │   ├── gdb-config.c.inc
│       │   └── xtensa-modules.c.inc
│       ├── core-sample_controller.c
│       ├── core-test_kc705_be
│       │   ├── core-isa.h
│       │   ├── gdb-config.c.inc
│       │   └── xtensa-modules.c.inc
│       ├── core-test_kc705_be.c
│       ├── core-test_mmuhifi_c3
│       │   ├── core-isa.h
│       │   ├── gdb-config.c.inc
│       │   └── xtensa-modules.c.inc
│       ├── core-test_mmuhifi_c3.c
│       ├── cores.list
│       ├── cpu-param.h
│       ├── cpu-qom.h
│       ├── cpu.c
│       ├── cpu.h
│       ├── dbg_helper.c
│       ├── exc_helper.c
│       ├── fpu_helper.c
│       ├── gdbstub.c
│       ├── helper.c
│       ├── helper.h
│       ├── import_core.sh
│       ├── Kconfig
│       ├── meson.build
│       ├── mmu_helper.c
│       ├── monitor.c
│       ├── op_helper.c
│       ├── overlay_tool.h
│       ├── translate.c
│       ├── win_helper.c
│       ├── xtensa-isa-internal.h
│       ├── xtensa-isa.c
│       ├── xtensa-isa.h
│       └── xtensa-semi.c
├── target-info-stub.c
├── target-info.c
├── tcg
│   ├── aarch64
│   │   ├── tcg-target-con-set.h
│   │   ├── tcg-target-con-str.h
│   │   ├── tcg-target-has.h
│   │   ├── tcg-target-mo.h
│   │   ├── tcg-target-opc.h.inc
│   │   ├── tcg-target-reg-bits.h
│   │   ├── tcg-target.c.inc
│   │   └── tcg-target.h
│   ├── arm
│   │   ├── tcg-target-con-set.h
│   │   ├── tcg-target-con-str.h
│   │   ├── tcg-target-has.h
│   │   ├── tcg-target-mo.h
│   │   ├── tcg-target-opc.h.inc
│   │   ├── tcg-target-reg-bits.h
│   │   ├── tcg-target.c.inc
│   │   └── tcg-target.h
│   ├── debuginfo.c
│   ├── i386
│   │   ├── tcg-target-con-set.h
│   │   ├── tcg-target-con-str.h
│   │   ├── tcg-target-has.h
│   │   ├── tcg-target-mo.h
│   │   ├── tcg-target-opc.h.inc
│   │   ├── tcg-target-reg-bits.h
│   │   ├── tcg-target.c.inc
│   │   └── tcg-target.h
│   ├── loongarch64
│   │   ├── tcg-insn-defs.c.inc
│   │   ├── tcg-target-con-set.h
│   │   ├── tcg-target-con-str.h
│   │   ├── tcg-target-has.h
│   │   ├── tcg-target-mo.h
│   │   ├── tcg-target-opc.h.inc
│   │   ├── tcg-target-reg-bits.h
│   │   ├── tcg-target.c.inc
│   │   └── tcg-target.h
│   ├── meson.build
│   ├── mips
│   │   ├── tcg-target-con-set.h
│   │   ├── tcg-target-con-str.h
│   │   ├── tcg-target-has.h
│   │   ├── tcg-target-mo.h
│   │   ├── tcg-target-opc.h.inc
│   │   ├── tcg-target-reg-bits.h
│   │   ├── tcg-target.c.inc
│   │   └── tcg-target.h
│   ├── optimize.c
│   ├── perf.c
│   ├── ppc
│   │   ├── tcg-target-con-set.h
│   │   ├── tcg-target-con-str.h
│   │   ├── tcg-target-has.h
│   │   ├── tcg-target-mo.h
│   │   ├── tcg-target-opc.h.inc
│   │   ├── tcg-target-reg-bits.h
│   │   ├── tcg-target.c.inc
│   │   └── tcg-target.h
│   ├── region.c
│   ├── riscv
│   │   ├── tcg-target-con-set.h
│   │   ├── tcg-target-con-str.h
│   │   ├── tcg-target-has.h
│   │   ├── tcg-target-mo.h
│   │   ├── tcg-target-opc.h.inc
│   │   ├── tcg-target-reg-bits.h
│   │   ├── tcg-target.c.inc
│   │   └── tcg-target.h
│   ├── s390x
│   │   ├── tcg-target-con-set.h
│   │   ├── tcg-target-con-str.h
│   │   ├── tcg-target-has.h
│   │   ├── tcg-target-mo.h
│   │   ├── tcg-target-opc.h.inc
│   │   ├── tcg-target-reg-bits.h
│   │   ├── tcg-target.c.inc
│   │   └── tcg-target.h
│   ├── sparc64
│   │   ├── tcg-target-con-set.h
│   │   ├── tcg-target-con-str.h
│   │   ├── tcg-target-has.h
│   │   ├── tcg-target-mo.h
│   │   ├── tcg-target-opc.h.inc
│   │   ├── tcg-target-reg-bits.h
│   │   ├── tcg-target.c.inc
│   │   └── tcg-target.h
│   ├── tcg-common.c
│   ├── tcg-has.h
│   ├── tcg-internal.h
│   ├── tcg-op-gvec.c
│   ├── tcg-op-ldst.c
│   ├── tcg-op-vec.c
│   ├── tcg-op.c
│   ├── tcg.c
│   ├── tci
│   │   ├── README
│   │   ├── tcg-target-con-set.h
│   │   ├── tcg-target-con-str.h
│   │   ├── tcg-target-has.h
│   │   ├── tcg-target-mo.h
│   │   ├── tcg-target-opc.h.inc
│   │   ├── tcg-target-reg-bits.h
│   │   ├── tcg-target.c.inc
│   │   └── tcg-target.h
│   └── tci.c
├── tests
│   ├── bench
│   │   ├── atomic_add-bench.c
│   │   ├── atomic64-bench.c
│   │   ├── benchmark-crypto-akcipher.c
│   │   ├── benchmark-crypto-cipher.c
│   │   ├── benchmark-crypto-hash.c
│   │   ├── benchmark-crypto-hmac.c
│   │   ├── bufferiszero-bench.c
│   │   ├── meson.build
│   │   ├── qht-bench.c
│   │   ├── qtree-bench.c
│   │   └── test_akcipher_keys.c.inc
│   ├── data
│   │   ├── acpi
│   │   │   ├── aarch64
│   │   │   │   └── virt
│   │   │   │       ├── APIC
│   │   │   │       ├── APIC.acpihmatvirt
│   │   │   │       ├── APIC.topology
│   │   │   │       ├── DBG2
│   │   │   │       ├── DSDT
│   │   │   │       ├── DSDT.acpihmatvirt
│   │   │   │       ├── DSDT.memhp
│   │   │   │       ├── DSDT.pxb
│   │   │   │       ├── DSDT.topology
│   │   │   │       ├── FACP
│   │   │   │       ├── GTDT
│   │   │   │       ├── HMAT.acpihmatvirt
│   │   │   │       ├── IORT
│   │   │   │       ├── MCFG
│   │   │   │       ├── NFIT.memhp
│   │   │   │       ├── PPTT
│   │   │   │       ├── PPTT.acpihmatvirt
│   │   │   │       ├── PPTT.topology
│   │   │   │       ├── SLIT.memhp
│   │   │   │       ├── SPCR
│   │   │   │       ├── SRAT.acpihmatvirt
│   │   │   │       ├── SRAT.memhp
│   │   │   │       ├── SRAT.numamem
│   │   │   │       ├── SSDT.memhp
│   │   │   │       └── VIOT
│   │   │   ├── disassemle-aml.sh
│   │   │   ├── rebuild-expected-aml.sh
│   │   │   ├── riscv64
│   │   │   │   └── virt
│   │   │   │       ├── APIC
│   │   │   │       ├── DSDT
│   │   │   │       ├── FACP
│   │   │   │       ├── MCFG
│   │   │   │       ├── RHCT
│   │   │   │       ├── SPCR
│   │   │   │       └── SRAT.numamem
│   │   │   └── x86
│   │   │       ├── microvm
│   │   │       │   ├── APIC
│   │   │       │   ├── APIC.ioapic2
│   │   │       │   ├── APIC.pcie
│   │   │       │   ├── DSDT
│   │   │       │   ├── DSDT.ioapic2
│   │   │       │   ├── DSDT.pcie
│   │   │       │   ├── DSDT.rtc
│   │   │       │   ├── DSDT.usb
│   │   │       │   ├── ERST.pcie
│   │   │       │   └── FACP
│   │   │       ├── pc
│   │   │       │   ├── APIC
│   │   │       │   ├── APIC.acpihmat
│   │   │       │   ├── APIC.cphp
│   │   │       │   ├── APIC.dimmpxm
│   │   │       │   ├── DSDT
│   │   │       │   ├── DSDT.acpierst
│   │   │       │   ├── DSDT.acpihmat
│   │   │       │   ├── DSDT.bridge
│   │   │       │   ├── DSDT.cphp
│   │   │       │   ├── DSDT.dimmpxm
│   │   │       │   ├── DSDT.hpbridge
│   │   │       │   ├── DSDT.hpbrroot
│   │   │       │   ├── DSDT.ipmikcs
│   │   │       │   ├── DSDT.memhp
│   │   │       │   ├── DSDT.nohpet
│   │   │       │   ├── DSDT.numamem
│   │   │       │   ├── DSDT.roothp
│   │   │       │   ├── ERST.acpierst
│   │   │       │   ├── FACP
│   │   │       │   ├── FACP.nosmm
│   │   │       │   ├── FACS
│   │   │       │   ├── HMAT.acpihmat
│   │   │       │   ├── HPET
│   │   │       │   ├── NFIT.dimmpxm
│   │   │       │   ├── SLIT.cphp
│   │   │       │   ├── SLIT.memhp
│   │   │       │   ├── SRAT.acpihmat
│   │   │       │   ├── SRAT.cphp
│   │   │       │   ├── SRAT.dimmpxm
│   │   │       │   ├── SRAT.memhp
│   │   │       │   ├── SRAT.numamem
│   │   │       │   ├── SSDT.dimmpxm
│   │   │       │   └── WAET
│   │   │       └── q35
│   │   │           ├── APIC
│   │   │           ├── APIC.acpihmat
│   │   │           ├── APIC.acpihmat-generic-x
│   │   │           ├── APIC.acpihmat-noinitiator
│   │   │           ├── APIC.core-count
│   │   │           ├── APIC.core-count2
│   │   │           ├── APIC.cphp
│   │   │           ├── APIC.dimmpxm
│   │   │           ├── APIC.thread-count
│   │   │           ├── APIC.thread-count2
│   │   │           ├── APIC.type4-count
│   │   │           ├── APIC.xapic
│   │   │           ├── CEDT.acpihmat-generic-x
│   │   │           ├── CEDT.cxl
│   │   │           ├── DMAR.dmar
│   │   │           ├── DSDT
│   │   │           ├── DSDT.acpierst
│   │   │           ├── DSDT.acpihmat
│   │   │           ├── DSDT.acpihmat-generic-x
│   │   │           ├── DSDT.acpihmat-noinitiator
│   │   │           ├── DSDT.applesmc
│   │   │           ├── DSDT.bridge
│   │   │           ├── DSDT.core-count
│   │   │           ├── DSDT.core-count2
│   │   │           ├── DSDT.cphp
│   │   │           ├── DSDT.cxl
│   │   │           ├── DSDT.dimmpxm
│   │   │           ├── DSDT.ipmibt
│   │   │           ├── DSDT.ipmismbus
│   │   │           ├── DSDT.ivrs
│   │   │           ├── DSDT.memhp
│   │   │           ├── DSDT.mmio64
│   │   │           ├── DSDT.multi-bridge
│   │   │           ├── DSDT.noacpihp
│   │   │           ├── DSDT.nohpet
│   │   │           ├── DSDT.numamem
│   │   │           ├── DSDT.pvpanic-isa
│   │   │           ├── DSDT.thread-count
│   │   │           ├── DSDT.thread-count2
│   │   │           ├── DSDT.tis.tpm12
│   │   │           ├── DSDT.tis.tpm2
│   │   │           ├── DSDT.type4-count
│   │   │           ├── DSDT.viot
│   │   │           ├── DSDT.xapic
│   │   │           ├── ERST.acpierst
│   │   │           ├── FACP
│   │   │           ├── FACP.core-count
│   │   │           ├── FACP.core-count2
│   │   │           ├── FACP.nosmm
│   │   │           ├── FACP.slic
│   │   │           ├── FACP.thread-count
│   │   │           ├── FACP.thread-count2
│   │   │           ├── FACP.type4-count
│   │   │           ├── FACP.xapic
│   │   │           ├── FACS
│   │   │           ├── HMAT.acpihmat
│   │   │           ├── HMAT.acpihmat-generic-x
│   │   │           ├── HMAT.acpihmat-noinitiator
│   │   │           ├── HPET
│   │   │           ├── IVRS.ivrs
│   │   │           ├── MCFG
│   │   │           ├── NFIT.dimmpxm
│   │   │           ├── SLIC.slic
│   │   │           ├── SLIT.cphp
│   │   │           ├── SLIT.memhp
│   │   │           ├── SRAT.acpihmat
│   │   │           ├── SRAT.acpihmat-generic-x
│   │   │           ├── SRAT.acpihmat-noinitiator
│   │   │           ├── SRAT.cphp
│   │   │           ├── SRAT.dimmpxm
│   │   │           ├── SRAT.memhp
│   │   │           ├── SRAT.mmio64
│   │   │           ├── SRAT.numamem
│   │   │           ├── SRAT.xapic
│   │   │           ├── SSDT.dimmpxm
│   │   │           ├── TCPA.tis.tpm12
│   │   │           ├── TPM2.tis.tpm2
│   │   │           ├── VIOT.viot
│   │   │           └── WAET
│   │   ├── hex-loader
│   │   │   └── test.hex
│   │   ├── qobject
│   │   │   └── qdict.txt
│   │   ├── smbios
│   │   │   ├── type11_blob
│   │   │   └── type11_blob.legacy
│   │   ├── test-qga-config
│   │   ├── test-qga-os-release
│   │   └── uefi-boot-images
│   │       ├── bios-tables-test.aarch64.iso.qcow2
│   │       ├── bios-tables-test.arm.iso.qcow2
│   │       ├── bios-tables-test.i386.iso.qcow2
│   │       ├── bios-tables-test.loongarch64.iso.qcow2
│   │       ├── bios-tables-test.riscv64.iso.qcow2
│   │       └── bios-tables-test.x86_64.iso.qcow2
│   ├── dbus-vmstate-daemon.sh
│   ├── decode
│   │   ├── err_argset1.decode
│   │   ├── err_argset2.decode
│   │   ├── err_field1.decode
│   │   ├── err_field10.decode
│   │   ├── err_field2.decode
│   │   ├── err_field3.decode
│   │   ├── err_field4.decode
│   │   ├── err_field5.decode
│   │   ├── err_field6.decode
│   │   ├── err_field7.decode
│   │   ├── err_field8.decode
│   │   ├── err_field9.decode
│   │   ├── err_init1.decode
│   │   ├── err_init2.decode
│   │   ├── err_init3.decode
│   │   ├── err_init4.decode
│   │   ├── err_overlap1.decode
│   │   ├── err_overlap2.decode
│   │   ├── err_overlap3.decode
│   │   ├── err_overlap4.decode
│   │   ├── err_overlap5.decode
│   │   ├── err_overlap6.decode
│   │   ├── err_overlap7.decode
│   │   ├── err_overlap8.decode
│   │   ├── err_overlap9.decode
│   │   ├── err_pattern_group_empty.decode
│   │   ├── err_pattern_group_ident1.decode
│   │   ├── err_pattern_group_ident2.decode
│   │   ├── err_pattern_group_nest1.decode
│   │   ├── err_pattern_group_nest2.decode
│   │   ├── err_pattern_group_nest3.decode
│   │   ├── err_pattern_group_overlap1.decode
│   │   ├── err_width1.decode
│   │   ├── err_width2.decode
│   │   ├── err_width3.decode
│   │   ├── err_width4.decode
│   │   ├── meson.build
│   │   ├── succ_argset_type1.decode
│   │   ├── succ_function.decode
│   │   ├── succ_ident1.decode
│   │   ├── succ_named_field.decode
│   │   ├── succ_pattern_group_nest1.decode
│   │   ├── succ_pattern_group_nest2.decode
│   │   ├── succ_pattern_group_nest3.decode
│   │   └── succ_pattern_group_nest4.decode
│   ├── docker
│   │   ├── common.rc
│   │   ├── docker.py
│   │   ├── dockerfiles
│   │   │   ├── alpine.docker
│   │   │   ├── centos9.docker
│   │   │   ├── debian-all-test-cross.docker
│   │   │   ├── debian-amd64-cross.docker
│   │   │   ├── debian-arm64-cross.docker
│   │   │   ├── debian-armhf-cross.docker
│   │   │   ├── debian-bootstrap.docker
│   │   │   ├── debian-bootstrap.pre
│   │   │   ├── debian-hexagon-cross.docker
│   │   │   ├── debian-i686-cross.docker
│   │   │   ├── debian-legacy-test-cross.docker
│   │   │   ├── debian-loongarch-cross.docker
│   │   │   ├── debian-microblaze-cross.d
│   │   │   │   └── build-toolchain.sh
│   │   │   ├── debian-mips64el-cross.docker
│   │   │   ├── debian-mipsel-cross.docker
│   │   │   ├── debian-ppc64el-cross.docker
│   │   │   ├── debian-riscv64-cross.docker
│   │   │   ├── debian-s390x-cross.docker
│   │   │   ├── debian-toolchain.docker
│   │   │   ├── debian-tricore-cross.docker
│   │   │   ├── debian-xtensa-cross.docker
│   │   │   ├── debian.docker
│   │   │   ├── emsdk-wasm32-cross.docker
│   │   │   ├── fedora-rust-nightly.docker
│   │   │   ├── fedora-win64-cross.docker
│   │   │   ├── fedora.docker
│   │   │   ├── opensuse-leap.docker
│   │   │   ├── python.docker
│   │   │   └── ubuntu2204.docker
│   │   ├── Makefile.include
│   │   ├── run
│   │   ├── test-block
│   │   ├── test-build
│   │   ├── test-clang
│   │   ├── test-debug
│   │   ├── test-full
│   │   ├── test-fuzz
│   │   ├── test-mingw
│   │   ├── test-misc
│   │   ├── test-quick
│   │   ├── test-rust
│   │   ├── test-static
│   │   ├── test-tcg
│   │   ├── test-tsan
│   │   └── test-unit
│   ├── fp
│   │   ├── fp-bench.c
│   │   ├── fp-test-log2.c
│   │   ├── fp-test.c
│   │   ├── meson.build
│   │   ├── platform.h
│   │   └── wrap.c.inc
│   ├── functional
│   │   ├── acpi-bits
│   │   │   ├── bits-config
│   │   │   │   └── bits-cfg.txt
│   │   │   └── bits-tests
│   │   │       ├── smbios.py2
│   │   │       ├── smilatency.py2
│   │   │       ├── testacpi.py2
│   │   │       └── testcpuid.py2
│   │   ├── aspeed.py
│   │   ├── meson.build
│   │   ├── qemu_test
│   │   │   ├── __init__.py
│   │   │   ├── archive.py
│   │   │   ├── asset.py
│   │   │   ├── cmd.py
│   │   │   ├── config.py
│   │   │   ├── decorators.py
│   │   │   ├── linuxkernel.py
│   │   │   ├── ports.py
│   │   │   ├── tesseract.py
│   │   │   ├── testcase.py
│   │   │   ├── tuxruntest.py
│   │   │   ├── uncompress.py
│   │   │   └── utils.py
│   │   ├── replay_kernel.py
│   │   ├── reverse_debugging.py
│   │   ├── test_aarch64_aspeed_ast2700.py
│   │   ├── test_aarch64_aspeed_ast2700fc.py
│   │   ├── test_aarch64_imx8mp_evk.py
│   │   ├── test_aarch64_raspi3.py
│   │   ├── test_aarch64_raspi4.py
│   │   ├── test_aarch64_replay.py
│   │   ├── test_aarch64_reverse_debug.py
│   │   ├── test_aarch64_rme_sbsaref.py
│   │   ├── test_aarch64_rme_virt.py
│   │   ├── test_aarch64_sbsaref_alpine.py
│   │   ├── test_aarch64_sbsaref_freebsd.py
│   │   ├── test_aarch64_sbsaref.py
│   │   ├── test_aarch64_smmu.py
│   │   ├── test_aarch64_tcg_plugins.py
│   │   ├── test_aarch64_tuxrun.py
│   │   ├── test_aarch64_virt_gpu.py
│   │   ├── test_aarch64_virt.py
│   │   ├── test_aarch64_xen.py
│   │   ├── test_aarch64_xlnx_versal.py
│   │   ├── test_acpi_bits.py
│   │   ├── test_alpha_clipper.py
│   │   ├── test_alpha_replay.py
│   │   ├── test_arm_aspeed_ast1030.py
│   │   ├── test_arm_aspeed_ast2500.py
│   │   ├── test_arm_aspeed_ast2600.py
│   │   ├── test_arm_aspeed_bletchley.py
│   │   ├── test_arm_aspeed_palmetto.py
│   │   ├── test_arm_aspeed_rainier.py
│   │   ├── test_arm_aspeed_romulus.py
│   │   ├── test_arm_aspeed_witherspoon.py
│   │   ├── test_arm_bflt.py
│   │   ├── test_arm_bpim2u.py
│   │   ├── test_arm_canona1100.py
│   │   ├── test_arm_collie.py
│   │   ├── test_arm_cubieboard.py
│   │   ├── test_arm_emcraft_sf2.py
│   │   ├── test_arm_integratorcp.py
│   │   ├── test_arm_microbit.py
│   │   ├── test_arm_orangepi.py
│   │   ├── test_arm_quanta_gsj.py
│   │   ├── test_arm_raspi2.py
│   │   ├── test_arm_realview.py
│   │   ├── test_arm_replay.py
│   │   ├── test_arm_smdkc210.py
│   │   ├── test_arm_stellaris.py
│   │   ├── test_arm_sx1.py
│   │   ├── test_arm_tuxrun.py
│   │   ├── test_arm_vexpress.py
│   │   ├── test_arm_virt.py
│   │   ├── test_avr_mega2560.py
│   │   ├── test_avr_uno.py
│   │   ├── test_cpu_queries.py
│   │   ├── test_empty_cpu_model.py
│   │   ├── test_hppa_seabios.py
│   │   ├── test_i386_replay.py
│   │   ├── test_i386_tuxrun.py
│   │   ├── test_info_usernet.py
│   │   ├── test_intel_iommu.py
│   │   ├── test_linux_initrd.py
│   │   ├── test_loongarch64_virt.py
│   │   ├── test_m68k_mcf5208evb.py
│   │   ├── test_m68k_nextcube.py
│   │   ├── test_m68k_q800.py
│   │   ├── test_m68k_replay.py
│   │   ├── test_m68k_tuxrun.py
│   │   ├── test_mem_addr_space.py
│   │   ├── test_memlock.py
│   │   ├── test_microblaze_replay.py
│   │   ├── test_microblaze_s3adsp1800.py
│   │   ├── test_microblazeel_s3adsp1800.py
│   │   ├── test_migration.py
│   │   ├── test_mips_malta.py
│   │   ├── test_mips_replay.py
│   │   ├── test_mips_tuxrun.py
│   │   ├── test_mips64_malta.py
│   │   ├── test_mips64_tuxrun.py
│   │   ├── test_mips64el_fuloong2e.py
│   │   ├── test_mips64el_loongson3v.py
│   │   ├── test_mips64el_malta.py
│   │   ├── test_mips64el_replay.py
│   │   ├── test_mips64el_tuxrun.py
│   │   ├── test_mipsel_malta.py
│   │   ├── test_mipsel_replay.py
│   │   ├── test_mipsel_tuxrun.py
│   │   ├── test_multiprocess.py
│   │   ├── test_netdev_ethtool.py
│   │   ├── test_or1k_replay.py
│   │   ├── test_or1k_sim.py
│   │   ├── test_pc_cpu_hotplug_props.py
│   │   ├── test_ppc_40p.py
│   │   ├── test_ppc_74xx.py
│   │   ├── test_ppc_amiga.py
│   │   ├── test_ppc_bamboo.py
│   │   ├── test_ppc_mac.py
│   │   ├── test_ppc_mpc8544ds.py
│   │   ├── test_ppc_replay.py
│   │   ├── test_ppc_sam460ex.py
│   │   ├── test_ppc_tuxrun.py
│   │   ├── test_ppc_virtex_ml507.py
│   │   ├── test_ppc64_e500.py
│   │   ├── test_ppc64_hv.py
│   │   ├── test_ppc64_mac99.py
│   │   ├── test_ppc64_powernv.py
│   │   ├── test_ppc64_pseries.py
│   │   ├── test_ppc64_replay.py
│   │   ├── test_ppc64_reverse_debug.py
│   │   ├── test_ppc64_tuxrun.py
│   │   ├── test_riscv_opensbi.py
│   │   ├── test_riscv32_tuxrun.py
│   │   ├── test_riscv64_tuxrun.py
│   │   ├── test_rx_gdbsim.py
│   │   ├── test_s390x_ccw_virtio.py
│   │   ├── test_s390x_replay.py
│   │   ├── test_s390x_topology.py
│   │   ├── test_s390x_tuxrun.py
│   │   ├── test_sh4_r2d.py
│   │   ├── test_sh4_tuxrun.py
│   │   ├── test_sh4eb_r2d.py
│   │   ├── test_sparc_replay.py
│   │   ├── test_sparc_sun4m.py
│   │   ├── test_sparc64_sun4u.py
│   │   ├── test_sparc64_tuxrun.py
│   │   ├── test_version.py
│   │   ├── test_virtio_balloon.py
│   │   ├── test_virtio_gpu.py
│   │   ├── test_virtio_version.py
│   │   ├── test_vnc.py
│   │   ├── test_x86_64_hotplug_blk.py
│   │   ├── test_x86_64_hotplug_cpu.py
│   │   ├── test_x86_64_kvm_xen.py
│   │   ├── test_x86_64_replay.py
│   │   ├── test_x86_64_reverse_debug.py
│   │   ├── test_x86_64_tuxrun.py
│   │   ├── test_x86_cpu_model_versions.py
│   │   ├── test_xtensa_lx60.py
│   │   └── test_xtensa_replay.py
│   ├── guest-debug
│   │   ├── run-test.py
│   │   └── test_gdbstub.py
│   ├── image-fuzzer
│   │   ├── qcow2
│   │   │   ├── __init__.py
│   │   │   ├── fuzz.py
│   │   │   └── layout.py
│   │   └── runner.py
│   ├── include
│   │   └── meson.build
│   ├── keys
│   │   ├── id_rsa
│   │   ├── id_rsa.pub
│   │   ├── README
│   │   ├── vagrant
│   │   └── vagrant.pub
│   ├── lcitool
│   │   ├── libvirt-ci
│   │   ├── Makefile.include
│   │   ├── mappings.yml
│   │   ├── projects
│   │   │   ├── qemu-minimal.yml
│   │   │   ├── qemu-win-installer.yml
│   │   │   └── qemu.yml
│   │   ├── refresh
│   │   └── targets
│   │       └── opensuse-leap-15.yml
│   ├── Makefile.include
│   ├── meson.build
│   ├── migration-stress
│   │   ├── guestperf
│   │   │   ├── __init__.py
│   │   │   ├── comparison.py
│   │   │   ├── engine.py
│   │   │   ├── hardware.py
│   │   │   ├── plot.py
│   │   │   ├── progress.py
│   │   │   ├── report.py
│   │   │   ├── scenario.py
│   │   │   ├── shell.py
│   │   │   └── timings.py
│   │   ├── guestperf-batch.py
│   │   ├── guestperf-plot.py
│   │   ├── guestperf.py
│   │   ├── initrd-stress.sh
│   │   ├── meson.build
│   │   └── stress.c
│   ├── multiboot
│   │   ├── aout_kludge.out
│   │   ├── aout_kludge.S
│   │   ├── libc.c
│   │   ├── libc.h
│   │   ├── link.ld
│   │   ├── Makefile
│   │   ├── mmap.c
│   │   ├── mmap.out
│   │   ├── module.txt
│   │   ├── modules.c
│   │   ├── modules.out
│   │   ├── multiboot.h
│   │   ├── run_test.sh
│   │   └── start.S
│   ├── perf
│   │   └── block
│   │       └── qcow2
│   │           └── convert-blockstatus
│   ├── qapi-schema
│   │   ├── allow-preconfig-test.err
│   │   ├── allow-preconfig-test.json
│   │   ├── allow-preconfig-test.out
│   │   ├── alternate-any.err
│   │   ├── alternate-any.json
│   │   ├── alternate-any.out
│   │   ├── alternate-array.err
│   │   ├── alternate-array.json
│   │   ├── alternate-array.out
│   │   ├── alternate-base.err
│   │   ├── alternate-base.json
│   │   ├── alternate-base.out
│   │   ├── alternate-branch-if-invalid.err
│   │   ├── alternate-branch-if-invalid.json
│   │   ├── alternate-branch-if-invalid.out
│   │   ├── alternate-clash.err
│   │   ├── alternate-clash.json
│   │   ├── alternate-clash.out
│   │   ├── alternate-conflict-bool-string.err
│   │   ├── alternate-conflict-bool-string.json
│   │   ├── alternate-conflict-bool-string.out
│   │   ├── alternate-conflict-dict.err
│   │   ├── alternate-conflict-dict.json
│   │   ├── alternate-conflict-dict.out
│   │   ├── alternate-conflict-enum-bool.err
│   │   ├── alternate-conflict-enum-bool.json
│   │   ├── alternate-conflict-enum-bool.out
│   │   ├── alternate-conflict-enum-int.err
│   │   ├── alternate-conflict-enum-int.json
│   │   ├── alternate-conflict-enum-int.out
│   │   ├── alternate-conflict-lists.err
│   │   ├── alternate-conflict-lists.json
│   │   ├── alternate-conflict-lists.out
│   │   ├── alternate-conflict-num-string.err
│   │   ├── alternate-conflict-num-string.json
│   │   ├── alternate-conflict-num-string.out
│   │   ├── alternate-conflict-string.err
│   │   ├── alternate-conflict-string.json
│   │   ├── alternate-conflict-string.out
│   │   ├── alternate-data-invalid.err
│   │   ├── alternate-data-invalid.json
│   │   ├── alternate-data-invalid.out
│   │   ├── alternate-empty.err
│   │   ├── alternate-empty.json
│   │   ├── alternate-empty.out
│   │   ├── alternate-invalid-dict.err
│   │   ├── alternate-invalid-dict.json
│   │   ├── alternate-invalid-dict.out
│   │   ├── alternate-nested.err
│   │   ├── alternate-nested.json
│   │   ├── alternate-nested.out
│   │   ├── alternate-unknown.err
│   │   ├── alternate-unknown.json
│   │   ├── alternate-unknown.out
│   │   ├── args-alternate.err
│   │   ├── args-alternate.json
│   │   ├── args-alternate.out
│   │   ├── args-any.err
│   │   ├── args-any.json
│   │   ├── args-any.out
│   │   ├── args-array-empty.err
│   │   ├── args-array-empty.json
│   │   ├── args-array-empty.out
│   │   ├── args-array-unknown.err
│   │   ├── args-array-unknown.json
│   │   ├── args-array-unknown.out
│   │   ├── args-bad-boxed.err
│   │   ├── args-bad-boxed.json
│   │   ├── args-bad-boxed.out
│   │   ├── args-boxed-anon.err
│   │   ├── args-boxed-anon.json
│   │   ├── args-boxed-anon.out
│   │   ├── args-boxed-string.err
│   │   ├── args-boxed-string.json
│   │   ├── args-boxed-string.out
│   │   ├── args-if-implicit.err
│   │   ├── args-if-implicit.json
│   │   ├── args-if-implicit.out
│   │   ├── args-if-unboxed.err
│   │   ├── args-if-unboxed.json
│   │   ├── args-if-unboxed.out
│   │   ├── args-int.err
│   │   ├── args-int.json
│   │   ├── args-int.out
│   │   ├── args-invalid.err
│   │   ├── args-invalid.json
│   │   ├── args-invalid.out
│   │   ├── args-member-array-bad.err
│   │   ├── args-member-array-bad.json
│   │   ├── args-member-array-bad.out
│   │   ├── args-member-case.err
│   │   ├── args-member-case.json
│   │   ├── args-member-case.out
│   │   ├── args-member-unknown.err
│   │   ├── args-member-unknown.json
│   │   ├── args-member-unknown.out
│   │   ├── args-union.err
│   │   ├── args-union.json
│   │   ├── args-union.out
│   │   ├── args-unknown.err
│   │   ├── args-unknown.json
│   │   ├── args-unknown.out
│   │   ├── bad-base.err
│   │   ├── bad-base.json
│   │   ├── bad-base.out
│   │   ├── bad-data.err
│   │   ├── bad-data.json
│   │   ├── bad-data.out
│   │   ├── bad-ident.err
│   │   ├── bad-ident.json
│   │   ├── bad-ident.out
│   │   ├── bad-if-all.err
│   │   ├── bad-if-all.json
│   │   ├── bad-if-all.out
│   │   ├── bad-if-empty-list.err
│   │   ├── bad-if-empty-list.json
│   │   ├── bad-if-empty-list.out
│   │   ├── bad-if-empty.err
│   │   ├── bad-if-empty.json
│   │   ├── bad-if-empty.out
│   │   ├── bad-if-key.err
│   │   ├── bad-if-key.json
│   │   ├── bad-if-key.out
│   │   ├── bad-if-keys.err
│   │   ├── bad-if-keys.json
│   │   ├── bad-if-keys.out
│   │   ├── bad-if-list.err
│   │   ├── bad-if-list.json
│   │   ├── bad-if-list.out
│   │   ├── bad-if-not.err
│   │   ├── bad-if-not.json
│   │   ├── bad-if-not.out
│   │   ├── bad-if.err
│   │   ├── bad-if.json
│   │   ├── bad-if.out
│   │   ├── bad-type-bool.err
│   │   ├── bad-type-bool.json
│   │   ├── bad-type-bool.out
│   │   ├── bad-type-dict.err
│   │   ├── bad-type-dict.json
│   │   ├── bad-type-dict.out
│   │   ├── bad-type-int.err
│   │   ├── bad-type-int.json
│   │   ├── bad-type-int.out
│   │   ├── base-cycle-direct.err
│   │   ├── base-cycle-direct.json
│   │   ├── base-cycle-direct.out
│   │   ├── base-cycle-indirect.err
│   │   ├── base-cycle-indirect.json
│   │   ├── base-cycle-indirect.out
│   │   ├── command-int.err
│   │   ├── command-int.json
│   │   ├── command-int.out
│   │   ├── comments.err
│   │   ├── comments.json
│   │   ├── comments.out
│   │   ├── doc-bad-alternate-member.err
│   │   ├── doc-bad-alternate-member.json
│   │   ├── doc-bad-alternate-member.out
│   │   ├── doc-bad-boxed-command-arg.err
│   │   ├── doc-bad-boxed-command-arg.json
│   │   ├── doc-bad-boxed-command-arg.out
│   │   ├── doc-bad-command-arg.err
│   │   ├── doc-bad-command-arg.json
│   │   ├── doc-bad-command-arg.out
│   │   ├── doc-bad-enum-member.err
│   │   ├── doc-bad-enum-member.json
│   │   ├── doc-bad-enum-member.out
│   │   ├── doc-bad-event-arg.err
│   │   ├── doc-bad-event-arg.json
│   │   ├── doc-bad-event-arg.out
│   │   ├── doc-bad-feature.err
│   │   ├── doc-bad-feature.json
│   │   ├── doc-bad-feature.out
│   │   ├── doc-bad-indent.err
│   │   ├── doc-bad-indent.json
│   │   ├── doc-bad-indent.out
│   │   ├── doc-bad-section.err
│   │   ├── doc-bad-section.json
│   │   ├── doc-bad-section.out
│   │   ├── doc-bad-symbol.err
│   │   ├── doc-bad-symbol.json
│   │   ├── doc-bad-symbol.out
│   │   ├── doc-bad-union-member.err
│   │   ├── doc-bad-union-member.json
│   │   ├── doc-bad-union-member.out
│   │   ├── doc-before-include.err
│   │   ├── doc-before-include.json
│   │   ├── doc-before-include.out
│   │   ├── doc-before-pragma.err
│   │   ├── doc-before-pragma.json
│   │   ├── doc-before-pragma.out
│   │   ├── doc-duplicate-features.err
│   │   ├── doc-duplicate-features.json
│   │   ├── doc-duplicate-features.out
│   │   ├── doc-duplicated-arg.err
│   │   ├── doc-duplicated-arg.json
│   │   ├── doc-duplicated-arg.out
│   │   ├── doc-duplicated-return.err
│   │   ├── doc-duplicated-return.json
│   │   ├── doc-duplicated-return.out
│   │   ├── doc-duplicated-since.err
│   │   ├── doc-duplicated-since.json
│   │   ├── doc-duplicated-since.out
│   │   ├── doc-empty-arg.err
│   │   ├── doc-empty-arg.json
│   │   ├── doc-empty-arg.out
│   │   ├── doc-empty-features.err
│   │   ├── doc-empty-features.json
│   │   ├── doc-empty-features.out
│   │   ├── doc-empty-section.err
│   │   ├── doc-empty-section.json
│   │   ├── doc-empty-section.out
│   │   ├── doc-empty-symbol.err
│   │   ├── doc-empty-symbol.json
│   │   ├── doc-empty-symbol.out
│   │   ├── doc-good.err
│   │   ├── doc-good.json
│   │   ├── doc-good.out
│   │   ├── doc-good.rst
│   │   ├── doc-good.txt
│   │   ├── doc-interleaved-section.err
│   │   ├── doc-interleaved-section.json
│   │   ├── doc-interleaved-section.out
│   │   ├── doc-invalid-end.err
│   │   ├── doc-invalid-end.json
│   │   ├── doc-invalid-end.out
│   │   ├── doc-invalid-end2.err
│   │   ├── doc-invalid-end2.json
│   │   ├── doc-invalid-end2.out
│   │   ├── doc-invalid-return.err
│   │   ├── doc-invalid-return.json
│   │   ├── doc-invalid-return.out
│   │   ├── doc-invalid-return2.err
│   │   ├── doc-invalid-return2.json
│   │   ├── doc-invalid-return2.out
│   │   ├── doc-invalid-section.err
│   │   ├── doc-invalid-section.json
│   │   ├── doc-invalid-section.out
│   │   ├── doc-invalid-start.err
│   │   ├── doc-invalid-start.json
│   │   ├── doc-invalid-start.out
│   │   ├── doc-missing-colon.err
│   │   ├── doc-missing-colon.json
│   │   ├── doc-missing-colon.out
│   │   ├── doc-missing-expr.err
│   │   ├── doc-missing-expr.json
│   │   ├── doc-missing-expr.out
│   │   ├── doc-missing-space.err
│   │   ├── doc-missing-space.json
│   │   ├── doc-missing-space.out
│   │   ├── doc-missing.err
│   │   ├── doc-missing.json
│   │   ├── doc-missing.out
│   │   ├── doc-no-symbol.err
│   │   ├── doc-no-symbol.json
│   │   ├── doc-no-symbol.out
│   │   ├── doc-non-first-section.err
│   │   ├── doc-non-first-section.json
│   │   ├── doc-non-first-section.out
│   │   ├── doc-undoc-feature.err
│   │   ├── doc-undoc-feature.json
│   │   ├── doc-undoc-feature.out
│   │   ├── double-type.err
│   │   ├── double-type.json
│   │   ├── double-type.out
│   │   ├── duplicate-key.err
│   │   ├── duplicate-key.json
│   │   ├── duplicate-key.out
│   │   ├── empty.err
│   │   ├── empty.json
│   │   ├── empty.out
│   │   ├── enum-bad-member.err
│   │   ├── enum-bad-member.json
│   │   ├── enum-bad-member.out
│   │   ├── enum-bad-name.err
│   │   ├── enum-bad-name.json
│   │   ├── enum-bad-name.out
│   │   ├── enum-bad-prefix.err
│   │   ├── enum-bad-prefix.json
│   │   ├── enum-bad-prefix.out
│   │   ├── enum-clash-member.err
│   │   ├── enum-clash-member.json
│   │   ├── enum-clash-member.out
│   │   ├── enum-dict-member-unknown.err
│   │   ├── enum-dict-member-unknown.json
│   │   ├── enum-dict-member-unknown.out
│   │   ├── enum-dict-no-name.err
│   │   ├── enum-dict-no-name.json
│   │   ├── enum-dict-no-name.out
│   │   ├── enum-if-invalid.err
│   │   ├── enum-if-invalid.json
│   │   ├── enum-if-invalid.out
│   │   ├── enum-int-member.err
│   │   ├── enum-int-member.json
│   │   ├── enum-int-member.out
│   │   ├── enum-member-case.err
│   │   ├── enum-member-case.json
│   │   ├── enum-member-case.out
│   │   ├── enum-missing-data.err
│   │   ├── enum-missing-data.json
│   │   ├── enum-missing-data.out
│   │   ├── enum-wrong-data.err
│   │   ├── enum-wrong-data.json
│   │   ├── enum-wrong-data.out
│   │   ├── escape-outside-string.err
│   │   ├── event-args-if-unboxed.err
│   │   ├── event-args-if-unboxed.json
│   │   ├── event-args-if-unboxed.out
│   │   ├── event-boxed-empty.err
│   │   ├── event-boxed-empty.json
│   │   ├── event-boxed-empty.out
│   │   ├── event-case.err
│   │   ├── event-case.json
│   │   ├── event-case.out
│   │   ├── event-member-invalid-dict.err
│   │   ├── event-member-invalid-dict.json
│   │   ├── event-member-invalid-dict.out
│   │   ├── event-nest-struct.err
│   │   ├── event-nest-struct.json
│   │   ├── event-nest-struct.out
│   │   ├── features-bad-type.err
│   │   ├── features-bad-type.json
│   │   ├── features-bad-type.out
│   │   ├── features-deprecated-type.err
│   │   ├── features-deprecated-type.json
│   │   ├── features-deprecated-type.out
│   │   ├── features-duplicate-name.err
│   │   ├── features-duplicate-name.json
│   │   ├── features-duplicate-name.out
│   │   ├── features-if-invalid.err
│   │   ├── features-if-invalid.json
│   │   ├── features-if-invalid.out
│   │   ├── features-missing-name.err
│   │   ├── features-missing-name.json
│   │   ├── features-missing-name.out
│   │   ├── features-name-bad-type.err
│   │   ├── features-name-bad-type.json
│   │   ├── features-name-bad-type.out
│   │   ├── features-no-list.err
│   │   ├── features-no-list.json
│   │   ├── features-no-list.out
│   │   ├── features-too-many.err
│   │   ├── features-too-many.json
│   │   ├── features-too-many.out
│   │   ├── features-unknown-key.err
│   │   ├── features-unknown-key.json
│   │   ├── features-unknown-key.out
│   │   ├── funny-char.err
│   │   ├── funny-char.json
│   │   ├── funny-char.out
│   │   ├── funny-word.err
│   │   ├── funny-word.json
│   │   ├── funny-word.out
│   │   ├── ident-with-escape.err
│   │   ├── ident-with-escape.json
│   │   ├── ident-with-escape.out
│   │   ├── include
│   │   │   └── sub-module.json
│   │   ├── include-before-err.err
│   │   ├── include-before-err.json
│   │   ├── include-before-err.out
│   │   ├── include-cycle-b.json
│   │   ├── include-cycle-c.json
│   │   ├── include-cycle.err
│   │   ├── include-cycle.json
│   │   ├── include-cycle.out
│   │   ├── include-extra-junk.err
│   │   ├── include-extra-junk.json
│   │   ├── include-extra-junk.out
│   │   ├── include-nested-err.err
│   │   ├── include-nested-err.json
│   │   ├── include-nested-err.out
│   │   ├── include-no-file.err
│   │   ├── include-no-file.json
│   │   ├── include-no-file.out
│   │   ├── include-non-file.err
│   │   ├── include-non-file.json
│   │   ├── include-non-file.out
│   │   ├── include-repetition-sub.json
│   │   ├── include-repetition.err
│   │   ├── include-repetition.json
│   │   ├── include-repetition.out
│   │   ├── include-self-cycle.err
│   │   ├── include-self-cycle.json
│   │   ├── include-self-cycle.out
│   │   ├── include-simple-sub.json
│   │   ├── include-simple.err
│   │   ├── include-simple.json
│   │   ├── include-simple.out
│   │   ├── indented-expr.err
│   │   ├── indented-expr.json
│   │   ├── indented-expr.out
│   │   ├── leading-comma-list.err
│   │   ├── leading-comma-list.json
│   │   ├── leading-comma-list.out
│   │   ├── leading-comma-object.err
│   │   ├── leading-comma-object.json
│   │   ├── leading-comma-object.out
│   │   ├── meson.build
│   │   ├── missing-array-rsqb.err
│   │   ├── missing-array-rsqb.json
│   │   ├── missing-array-rsqb.out
│   │   ├── missing-colon.err
│   │   ├── missing-colon.json
│   │   ├── missing-colon.out
│   │   ├── missing-comma-list.err
│   │   ├── missing-comma-list.json
│   │   ├── missing-comma-list.out
│   │   ├── missing-comma-object.err
│   │   ├── missing-comma-object.json
│   │   ├── missing-comma-object.out
│   │   ├── missing-object-member-element.err
│   │   ├── missing-object-member-element.json
│   │   ├── missing-object-member-element.out
│   │   ├── missing-schema.err
│   │   ├── missing-schema.out
│   │   ├── missing-type.err
│   │   ├── missing-type.json
│   │   ├── missing-type.out
│   │   ├── nested-struct-data-invalid-dict.err
│   │   ├── nested-struct-data-invalid-dict.json
│   │   ├── nested-struct-data-invalid-dict.out
│   │   ├── nested-struct-data.err
│   │   ├── nested-struct-data.json
│   │   ├── nested-struct-data.out
│   │   ├── non-objects.err
│   │   ├── non-objects.json
│   │   ├── non-objects.out
│   │   ├── oob-coroutine.err
│   │   ├── oob-coroutine.json
│   │   ├── oob-coroutine.out
│   │   ├── oob-test.err
│   │   ├── oob-test.json
│   │   ├── oob-test.out
│   │   ├── pragma-extra-junk.err
│   │   ├── pragma-extra-junk.json
│   │   ├── pragma-extra-junk.out
│   │   ├── pragma-non-dict.err
│   │   ├── pragma-non-dict.json
│   │   ├── pragma-non-dict.out
│   │   ├── pragma-unknown.err
│   │   ├── pragma-unknown.json
│   │   ├── pragma-unknown.out
│   │   ├── pragma-value-not-bool.err
│   │   ├── pragma-value-not-bool.json
│   │   ├── pragma-value-not-bool.out
│   │   ├── pragma-value-not-list-of-str.err
│   │   ├── pragma-value-not-list-of-str.json
│   │   ├── pragma-value-not-list-of-str.out
│   │   ├── pragma-value-not-list.err
│   │   ├── pragma-value-not-list.json
│   │   ├── pragma-value-not-list.out
│   │   ├── qapi-schema-test.err
│   │   ├── qapi-schema-test.json
│   │   ├── qapi-schema-test.out
│   │   ├── quoted-structural-chars.err
│   │   ├── quoted-structural-chars.json
│   │   ├── quoted-structural-chars.out
│   │   ├── redefined-command.err
│   │   ├── redefined-command.json
│   │   ├── redefined-command.out
│   │   ├── redefined-event.err
│   │   ├── redefined-event.json
│   │   ├── redefined-event.out
│   │   ├── redefined-predefined.err
│   │   ├── redefined-predefined.json
│   │   ├── redefined-predefined.out
│   │   ├── redefined-type.err
│   │   ├── redefined-type.json
│   │   ├── redefined-type.out
│   │   ├── reserved-command-q.err
│   │   ├── reserved-command-q.json
│   │   ├── reserved-command-q.out
│   │   ├── reserved-enum-q.err
│   │   ├── reserved-enum-q.json
│   │   ├── reserved-enum-q.out
│   │   ├── reserved-member-has.err
│   │   ├── reserved-member-has.json
│   │   ├── reserved-member-has.out
│   │   ├── reserved-member-q.err
│   │   ├── reserved-member-q.json
│   │   ├── reserved-member-q.out
│   │   ├── reserved-member-u.err
│   │   ├── reserved-member-u.json
│   │   ├── reserved-member-u.out
│   │   ├── reserved-member-underscore.err
│   │   ├── reserved-member-underscore.json
│   │   ├── reserved-member-underscore.out
│   │   ├── reserved-type-list.err
│   │   ├── reserved-type-list.json
│   │   ├── reserved-type-list.out
│   │   ├── returns-alternate.err
│   │   ├── returns-alternate.json
│   │   ├── returns-alternate.out
│   │   ├── returns-array-bad.err
│   │   ├── returns-array-bad.json
│   │   ├── returns-array-bad.out
│   │   ├── returns-bad-type.err
│   │   ├── returns-bad-type.json
│   │   ├── returns-bad-type.out
│   │   ├── returns-dict.err
│   │   ├── returns-dict.json
│   │   ├── returns-dict.out
│   │   ├── returns-unknown.err
│   │   ├── returns-unknown.json
│   │   ├── returns-unknown.out
│   │   ├── string-code-point-127.err
│   │   ├── string-code-point-127.json
│   │   ├── string-code-point-127.out
│   │   ├── string-code-point-31.err
│   │   ├── string-code-point-31.json
│   │   ├── string-code-point-31.out
│   │   ├── struct-base-clash-deep.err
│   │   ├── struct-base-clash-deep.json
│   │   ├── struct-base-clash-deep.out
│   │   ├── struct-base-clash.err
│   │   ├── struct-base-clash.json
│   │   ├── struct-base-clash.out
│   │   ├── struct-data-invalid.err
│   │   ├── struct-data-invalid.json
│   │   ├── struct-data-invalid.out
│   │   ├── struct-data-typename.err
│   │   ├── struct-data-typename.json
│   │   ├── struct-data-typename.out
│   │   ├── struct-member-if-invalid.err
│   │   ├── struct-member-if-invalid.json
│   │   ├── struct-member-if-invalid.out
│   │   ├── struct-member-invalid-dict.err
│   │   ├── struct-member-invalid-dict.json
│   │   ├── struct-member-invalid-dict.out
│   │   ├── struct-member-invalid.err
│   │   ├── struct-member-invalid.json
│   │   ├── struct-member-invalid.out
│   │   ├── struct-member-name-clash.err
│   │   ├── struct-member-name-clash.json
│   │   ├── struct-member-name-clash.out
│   │   ├── sub-sub-module.json
│   │   ├── test-qapi.py
│   │   ├── trailing-comma-list.err
│   │   ├── trailing-comma-list.json
│   │   ├── trailing-comma-list.out
│   │   ├── trailing-comma-object.err
│   │   ├── trailing-comma-object.json
│   │   ├── trailing-comma-object.out
│   │   ├── type-bypass-bad-gen.err
│   │   ├── type-bypass-bad-gen.json
│   │   ├── type-bypass-bad-gen.out
│   │   ├── type-case.err
│   │   ├── type-case.json
│   │   ├── type-case.out
│   │   ├── unclosed-list.err
│   │   ├── unclosed-list.json
│   │   ├── unclosed-list.out
│   │   ├── unclosed-object.err
│   │   ├── unclosed-object.json
│   │   ├── unclosed-object.out
│   │   ├── unclosed-string.err
│   │   ├── unclosed-string.json
│   │   ├── unclosed-string.out
│   │   ├── union-array-branch.err
│   │   ├── union-array-branch.json
│   │   ├── union-array-branch.out
│   │   ├── union-bad-base.err
│   │   ├── union-bad-base.json
│   │   ├── union-bad-base.out
│   │   ├── union-bad-discriminator.err
│   │   ├── union-bad-discriminator.json
│   │   ├── union-bad-discriminator.out
│   │   ├── union-base-any.err
│   │   ├── union-base-any.json
│   │   ├── union-base-any.out
│   │   ├── union-base-empty.err
│   │   ├── union-base-empty.json
│   │   ├── union-base-empty.out
│   │   ├── union-base-no-discriminator.err
│   │   ├── union-base-no-discriminator.json
│   │   ├── union-base-no-discriminator.out
│   │   ├── union-base-union.err
│   │   ├── union-base-union.json
│   │   ├── union-base-union.out
│   │   ├── union-branch-if-invalid.err
│   │   ├── union-branch-if-invalid.json
│   │   ├── union-branch-if-invalid.out
│   │   ├── union-branch-invalid-dict.err
│   │   ├── union-branch-invalid-dict.json
│   │   ├── union-branch-invalid-dict.out
│   │   ├── union-clash-member.err
│   │   ├── union-clash-member.json
│   │   ├── union-clash-member.out
│   │   ├── union-discriminator-bad-name.err
│   │   ├── union-discriminator-bad-name.json
│   │   ├── union-discriminator-bad-name.out
│   │   ├── union-empty.err
│   │   ├── union-empty.json
│   │   ├── union-empty.out
│   │   ├── union-inline-invalid-dict.err
│   │   ├── union-inline-invalid-dict.json
│   │   ├── union-inline-invalid-dict.out
│   │   ├── union-int-branch.err
│   │   ├── union-int-branch.json
│   │   ├── union-int-branch.out
│   │   ├── union-invalid-base.err
│   │   ├── union-invalid-base.json
│   │   ├── union-invalid-base.out
│   │   ├── union-invalid-branch-key.err
│   │   ├── union-invalid-branch-key.json
│   │   ├── union-invalid-branch-key.out
│   │   ├── union-invalid-data.err
│   │   ├── union-invalid-data.json
│   │   ├── union-invalid-data.out
│   │   ├── union-invalid-discriminator.err
│   │   ├── union-invalid-discriminator.json
│   │   ├── union-invalid-discriminator.out
│   │   ├── union-invalid-if-discriminator.err
│   │   ├── union-invalid-if-discriminator.json
│   │   ├── union-invalid-if-discriminator.out
│   │   ├── union-invalid-union-subfield.err
│   │   ├── union-invalid-union-subfield.json
│   │   ├── union-invalid-union-subfield.out
│   │   ├── union-invalid-union-subtype.err
│   │   ├── union-invalid-union-subtype.json
│   │   ├── union-invalid-union-subtype.out
│   │   ├── union-no-base.err
│   │   ├── union-no-base.json
│   │   ├── union-no-base.out
│   │   ├── union-optional-discriminator.err
│   │   ├── union-optional-discriminator.json
│   │   ├── union-optional-discriminator.out
│   │   ├── union-string-discriminator.err
│   │   ├── union-string-discriminator.json
│   │   ├── union-string-discriminator.out
│   │   ├── union-unknown.err
│   │   ├── union-unknown.json
│   │   ├── union-unknown.out
│   │   ├── unknown-escape.err
│   │   ├── unknown-escape.json
│   │   ├── unknown-escape.out
│   │   ├── unknown-expr-key.err
│   │   ├── unknown-expr-key.json
│   │   └── unknown-expr-key.out
│   ├── qemu-iotests
│   │   ├── 001
│   │   ├── 001.out
│   │   ├── 002
│   │   ├── 002.out
│   │   ├── 003
│   │   ├── 003.out
│   │   ├── 004
│   │   ├── 004.out
│   │   ├── 005
│   │   ├── 005.out
│   │   ├── 007
│   │   ├── 007.out
│   │   ├── 008
│   │   ├── 008.out
│   │   ├── 009
│   │   ├── 009.out
│   │   ├── 010
│   │   ├── 010.out
│   │   ├── 011
│   │   ├── 011.out
│   │   ├── 012
│   │   ├── 012.out
│   │   ├── 013
│   │   ├── 013.out
│   │   ├── 014
│   │   ├── 014.out
│   │   ├── 015
│   │   ├── 015.out
│   │   ├── 017
│   │   ├── 017.out
│   │   ├── 018
│   │   ├── 018.out
│   │   ├── 019
│   │   ├── 019.out
│   │   ├── 020
│   │   ├── 020.out
│   │   ├── 021
│   │   ├── 021.out
│   │   ├── 022
│   │   ├── 022.out
│   │   ├── 023
│   │   ├── 023.out
│   │   ├── 024
│   │   ├── 024.out
│   │   ├── 025
│   │   ├── 025.out
│   │   ├── 026
│   │   ├── 026.out
│   │   ├── 026.out.nocache
│   │   ├── 027
│   │   ├── 027.out
│   │   ├── 028
│   │   ├── 028.out
│   │   ├── 029
│   │   ├── 029.out
│   │   ├── 030
│   │   ├── 030.out
│   │   ├── 031
│   │   ├── 031.out
│   │   ├── 032
│   │   ├── 032.out
│   │   ├── 033
│   │   ├── 033.out
│   │   ├── 034
│   │   ├── 034.out
│   │   ├── 035
│   │   ├── 035.out
│   │   ├── 036
│   │   ├── 036.out
│   │   ├── 037
│   │   ├── 037.out
│   │   ├── 038
│   │   ├── 038.out
│   │   ├── 039
│   │   ├── 039.out
│   │   ├── 040
│   │   ├── 040.out
│   │   ├── 041
│   │   ├── 041.out
│   │   ├── 042
│   │   ├── 042.out
│   │   ├── 043
│   │   ├── 043.out
│   │   ├── 044
│   │   ├── 044.out
│   │   ├── 045
│   │   ├── 045.out
│   │   ├── 046
│   │   ├── 046.out
│   │   ├── 047
│   │   ├── 047.out
│   │   ├── 048
│   │   ├── 048.out
│   │   ├── 049
│   │   ├── 049.out
│   │   ├── 050
│   │   ├── 050.out
│   │   ├── 051
│   │   ├── 051.out
│   │   ├── 051.pc.out
│   │   ├── 052
│   │   ├── 052.out
│   │   ├── 053
│   │   ├── 053.out
│   │   ├── 054
│   │   ├── 054.out
│   │   ├── 055
│   │   ├── 055.out
│   │   ├── 056
│   │   ├── 056.out
│   │   ├── 057
│   │   ├── 057.out
│   │   ├── 058
│   │   ├── 058.out
│   │   ├── 059
│   │   ├── 059.out
│   │   ├── 060
│   │   ├── 060.out
│   │   ├── 061
│   │   ├── 061.out
│   │   ├── 062
│   │   ├── 062.out
│   │   ├── 063
│   │   ├── 063.out
│   │   ├── 064
│   │   ├── 064.out
│   │   ├── 065
│   │   ├── 065.out
│   │   ├── 066
│   │   ├── 066.out
│   │   ├── 068
│   │   ├── 068.out
│   │   ├── 069
│   │   ├── 069.out
│   │   ├── 070
│   │   ├── 070.out
│   │   ├── 071
│   │   ├── 071.out
│   │   ├── 072
│   │   ├── 072.out
│   │   ├── 073
│   │   ├── 073.out
│   │   ├── 074
│   │   ├── 074.out
│   │   ├── 075
│   │   ├── 075.out
│   │   ├── 076
│   │   ├── 076.out
│   │   ├── 077
│   │   ├── 077.out
│   │   ├── 078
│   │   ├── 078.out
│   │   ├── 079
│   │   ├── 079.out
│   │   ├── 080
│   │   ├── 080.out
│   │   ├── 081
│   │   ├── 081.out
│   │   ├── 082
│   │   ├── 082.out
│   │   ├── 083
│   │   ├── 083.out
│   │   ├── 084
│   │   ├── 084.out
│   │   ├── 085
│   │   ├── 085.out
│   │   ├── 086
│   │   ├── 086.out
│   │   ├── 087
│   │   ├── 087.out
│   │   ├── 088
│   │   ├── 088.out
│   │   ├── 089
│   │   ├── 089.out
│   │   ├── 090
│   │   ├── 090.out
│   │   ├── 091
│   │   ├── 091.out
│   │   ├── 092
│   │   ├── 092.out
│   │   ├── 093
│   │   ├── 093.out
│   │   ├── 094
│   │   ├── 094.out
│   │   ├── 095
│   │   ├── 095.out
│   │   ├── 096
│   │   ├── 096.out
│   │   ├── 097
│   │   ├── 097.out
│   │   ├── 098
│   │   ├── 098.out
│   │   ├── 099
│   │   ├── 099.out
│   │   ├── 101
│   │   ├── 101.out
│   │   ├── 102
│   │   ├── 102.out
│   │   ├── 103
│   │   ├── 103.out
│   │   ├── 104
│   │   ├── 104.out
│   │   ├── 105
│   │   ├── 105.out
│   │   ├── 106
│   │   ├── 106.out
│   │   ├── 107
│   │   ├── 107.out
│   │   ├── 108
│   │   ├── 108.out
│   │   ├── 109
│   │   ├── 109.out
│   │   ├── 110
│   │   ├── 110.out
│   │   ├── 111
│   │   ├── 111.out
│   │   ├── 112
│   │   ├── 112.out
│   │   ├── 113
│   │   ├── 113.out
│   │   ├── 114
│   │   ├── 114.out
│   │   ├── 115
│   │   ├── 115.out
│   │   ├── 116
│   │   ├── 116.out
│   │   ├── 117
│   │   ├── 117.out
│   │   ├── 118
│   │   ├── 118.out
│   │   ├── 119
│   │   ├── 119.out
│   │   ├── 120
│   │   ├── 120.out
│   │   ├── 121
│   │   ├── 121.out
│   │   ├── 122
│   │   ├── 122.out
│   │   ├── 123
│   │   ├── 123.out
│   │   ├── 124
│   │   ├── 124.out
│   │   ├── 125
│   │   ├── 125.out
│   │   ├── 126
│   │   ├── 126.out
│   │   ├── 127
│   │   ├── 127.out
│   │   ├── 128
│   │   ├── 128.out
│   │   ├── 129
│   │   ├── 129.out
│   │   ├── 130
│   │   ├── 130.out
│   │   ├── 131
│   │   ├── 131.out
│   │   ├── 132
│   │   ├── 132.out
│   │   ├── 133
│   │   ├── 133.out
│   │   ├── 134
│   │   ├── 134.out
│   │   ├── 135
│   │   ├── 135.out
│   │   ├── 136
│   │   ├── 136.out
│   │   ├── 137
│   │   ├── 137.out
│   │   ├── 138
│   │   ├── 138.out
│   │   ├── 139
│   │   ├── 139.out
│   │   ├── 140
│   │   ├── 140.out
│   │   ├── 141
│   │   ├── 141.out
│   │   ├── 142
│   │   ├── 142.out
│   │   ├── 143
│   │   ├── 143.out
│   │   ├── 144
│   │   ├── 144.out
│   │   ├── 145
│   │   ├── 145.out
│   │   ├── 146
│   │   ├── 146.out
│   │   ├── 147
│   │   ├── 147.out
│   │   ├── 148
│   │   ├── 148.out
│   │   ├── 149
│   │   ├── 149.out
│   │   ├── 150
│   │   ├── 150.out.qcow2
│   │   ├── 150.out.raw
│   │   ├── 151
│   │   ├── 151.out
│   │   ├── 152
│   │   ├── 152.out
│   │   ├── 153
│   │   ├── 153.out
│   │   ├── 154
│   │   ├── 154.out
│   │   ├── 155
│   │   ├── 155.out
│   │   ├── 156
│   │   ├── 156.out
│   │   ├── 157
│   │   ├── 157.out
│   │   ├── 158
│   │   ├── 158.out
│   │   ├── 159
│   │   ├── 159.out
│   │   ├── 160
│   │   ├── 160.out
│   │   ├── 161
│   │   ├── 161.out
│   │   ├── 162
│   │   ├── 162.out
│   │   ├── 163
│   │   ├── 163.out
│   │   ├── 165
│   │   ├── 165.out
│   │   ├── 170
│   │   ├── 170.out
│   │   ├── 171
│   │   ├── 171.out
│   │   ├── 172
│   │   ├── 172.out
│   │   ├── 173
│   │   ├── 173.out
│   │   ├── 174
│   │   ├── 174.out
│   │   ├── 175
│   │   ├── 175.out
│   │   ├── 176
│   │   ├── 176.out
│   │   ├── 177
│   │   ├── 177.out
│   │   ├── 178
│   │   ├── 178.out.qcow2
│   │   ├── 178.out.raw
│   │   ├── 179
│   │   ├── 179.out
│   │   ├── 181
│   │   ├── 181.out
│   │   ├── 182
│   │   ├── 182.out
│   │   ├── 184
│   │   ├── 184.out
│   │   ├── 185
│   │   ├── 185.out
│   │   ├── 186
│   │   ├── 186.out
│   │   ├── 187
│   │   ├── 187.out
│   │   ├── 188
│   │   ├── 188.out
│   │   ├── 189
│   │   ├── 189.out
│   │   ├── 190
│   │   ├── 190.out
│   │   ├── 191
│   │   ├── 191.out
│   │   ├── 192
│   │   ├── 192.out
│   │   ├── 194
│   │   ├── 194.out
│   │   ├── 195
│   │   ├── 195.out
│   │   ├── 196
│   │   ├── 196.out
│   │   ├── 197
│   │   ├── 197.out
│   │   ├── 198
│   │   ├── 198.out
│   │   ├── 200
│   │   ├── 200.out
│   │   ├── 201
│   │   ├── 201.out
│   │   ├── 202
│   │   ├── 202.out
│   │   ├── 203
│   │   ├── 203.out
│   │   ├── 204
│   │   ├── 204.out
│   │   ├── 205
│   │   ├── 205.out
│   │   ├── 206
│   │   ├── 206.out
│   │   ├── 207
│   │   ├── 207.out
│   │   ├── 208
│   │   ├── 208.out
│   │   ├── 209
│   │   ├── 209.out
│   │   ├── 210
│   │   ├── 210.out
│   │   ├── 211
│   │   ├── 211.out
│   │   ├── 212
│   │   ├── 212.out
│   │   ├── 213
│   │   ├── 213.out
│   │   ├── 214
│   │   ├── 214.out
│   │   ├── 215
│   │   ├── 215.out
│   │   ├── 216
│   │   ├── 216.out
│   │   ├── 217
│   │   ├── 217.out
│   │   ├── 218
│   │   ├── 218.out
│   │   ├── 219
│   │   ├── 219.out
│   │   ├── 220
│   │   ├── 220.out
│   │   ├── 221
│   │   ├── 221.out
│   │   ├── 223
│   │   ├── 223.out
│   │   ├── 224
│   │   ├── 224.out
│   │   ├── 225
│   │   ├── 225.out
│   │   ├── 226
│   │   ├── 226.out
│   │   ├── 227
│   │   ├── 227.out
│   │   ├── 228
│   │   ├── 228.out
│   │   ├── 229
│   │   ├── 229.out
│   │   ├── 231
│   │   ├── 231.out
│   │   ├── 232
│   │   ├── 232.out
│   │   ├── 233
│   │   ├── 233.out
│   │   ├── 234
│   │   ├── 234.out
│   │   ├── 235
│   │   ├── 235.out
│   │   ├── 236
│   │   ├── 236.out
│   │   ├── 237
│   │   ├── 237.out
│   │   ├── 238
│   │   ├── 238.out
│   │   ├── 239
│   │   ├── 239.out
│   │   ├── 240
│   │   ├── 240.out
│   │   ├── 241
│   │   ├── 241.out
│   │   ├── 242
│   │   ├── 242.out
│   │   ├── 243
│   │   ├── 243.out
│   │   ├── 244
│   │   ├── 244.out
│   │   ├── 245
│   │   ├── 245.out
│   │   ├── 246
│   │   ├── 246.out
│   │   ├── 247
│   │   ├── 247.out
│   │   ├── 248
│   │   ├── 248.out
│   │   ├── 249
│   │   ├── 249.out
│   │   ├── 250
│   │   ├── 250.out
│   │   ├── 251
│   │   ├── 251.out
│   │   ├── 252
│   │   ├── 252.out
│   │   ├── 253
│   │   ├── 253.out
│   │   ├── 254
│   │   ├── 254.out
│   │   ├── 255
│   │   ├── 255.out
│   │   ├── 256
│   │   ├── 256.out
│   │   ├── 257
│   │   ├── 257.out
│   │   ├── 258
│   │   ├── 258.out
│   │   ├── 259
│   │   ├── 259.out
│   │   ├── 260
│   │   ├── 260.out
│   │   ├── 261
│   │   ├── 261.out
│   │   ├── 262
│   │   ├── 262.out
│   │   ├── 263
│   │   ├── 263.out
│   │   ├── 264
│   │   ├── 264.out
│   │   ├── 265
│   │   ├── 265.out
│   │   ├── 266
│   │   ├── 266.out
│   │   ├── 267
│   │   ├── 267.out
│   │   ├── 268
│   │   ├── 268.out
│   │   ├── 270
│   │   ├── 270.out
│   │   ├── 271
│   │   ├── 271.out
│   │   ├── 272
│   │   ├── 272.out
│   │   ├── 273
│   │   ├── 273.out
│   │   ├── 274
│   │   ├── 274.out
│   │   ├── 277
│   │   ├── 277.out
│   │   ├── 279
│   │   ├── 279.out
│   │   ├── 280
│   │   ├── 280.out
│   │   ├── 281
│   │   ├── 281.out
│   │   ├── 282
│   │   ├── 282.out
│   │   ├── 283
│   │   ├── 283.out
│   │   ├── 284
│   │   ├── 284.out
│   │   ├── 286
│   │   ├── 286.out
│   │   ├── 287
│   │   ├── 287.out
│   │   ├── 288
│   │   ├── 288.out
│   │   ├── 289
│   │   ├── 289.out
│   │   ├── 290
│   │   ├── 290.out
│   │   ├── 292
│   │   ├── 292.out
│   │   ├── 293
│   │   ├── 293.out
│   │   ├── 294
│   │   ├── 294.out
│   │   ├── 295
│   │   ├── 295.out
│   │   ├── 296
│   │   ├── 296.out
│   │   ├── 297
│   │   ├── 297.out
│   │   ├── 298
│   │   ├── 298.out
│   │   ├── 299
│   │   ├── 299.out
│   │   ├── 300
│   │   ├── 300.out
│   │   ├── 301
│   │   ├── 301.out
│   │   ├── 302
│   │   ├── 302.out
│   │   ├── 303
│   │   ├── 303.out
│   │   ├── 304
│   │   ├── 304.out
│   │   ├── 305
│   │   ├── 305.out
│   │   ├── 307
│   │   ├── 307.out
│   │   ├── 308
│   │   ├── 308.out
│   │   ├── 310
│   │   ├── 310.out
│   │   ├── 312
│   │   ├── 312.out
│   │   ├── 313
│   │   ├── 313.out
│   │   ├── 314
│   │   ├── 314.out
│   │   ├── check
│   │   ├── common.filter
│   │   ├── common.nbd
│   │   ├── common.pattern
│   │   ├── common.qemu
│   │   ├── common.rc
│   │   ├── common.tls
│   │   ├── fat16.py
│   │   ├── findtests.py
│   │   ├── iotests.py
│   │   ├── linters.py
│   │   ├── Makefile
│   │   ├── meson.build
│   │   ├── mypy.ini
│   │   ├── nbd-fault-injector.py
│   │   ├── pylintrc
│   │   ├── qcow2_format.py
│   │   ├── qcow2.py
│   │   ├── qed.py
│   │   ├── README
│   │   ├── sample_images
│   │   │   ├── afl5.img.bz2
│   │   │   ├── afl9.vmdk.bz2
│   │   │   ├── d2v-zerofilled.vhd.bz2
│   │   │   ├── empty.bochs.bz2
│   │   │   ├── grub_mbr.raw.bz2
│   │   │   ├── hyperv2012r2-dynamic.vhd.bz2
│   │   │   ├── iotest-dirtylog-10G-4M.vhdx.bz2
│   │   │   ├── iotest-dynamic-1G.vhdx.bz2
│   │   │   ├── iotest-version3.vmdk.bz2
│   │   │   ├── parallels-v1.bz2
│   │   │   ├── parallels-v2.bz2
│   │   │   ├── parallels-with-bitmap.bz2
│   │   │   ├── parallels-with-bitmap.sh
│   │   │   ├── README
│   │   │   ├── simple-dmg.dmg.bz2
│   │   │   ├── simple-pattern.cloop.bz2
│   │   │   ├── test-disk2vhd.vhdx.bz2
│   │   │   └── virtualpc-dynamic.vhd.bz2
│   │   ├── testenv.py
│   │   ├── testrunner.py
│   │   └── tests
│   │       ├── backing-file-invalidation
│   │       ├── backing-file-invalidation.out
│   │       ├── backup-discard-source
│   │       ├── backup-discard-source.out
│   │       ├── block-status-cache
│   │       ├── block-status-cache.out
│   │       ├── commit-zero-blocks
│   │       ├── commit-zero-blocks.out
│   │       ├── copy-before-write
│   │       ├── copy-before-write.out
│   │       ├── detect-zeroes-registered-buf
│   │       ├── detect-zeroes-registered-buf.out
│   │       ├── export-incoming-iothread
│   │       ├── export-incoming-iothread.out
│   │       ├── file-io-error
│   │       ├── file-io-error.out
│   │       ├── fuse-allow-other
│   │       ├── fuse-allow-other.out
│   │       ├── graph-changes-while-io
│   │       ├── graph-changes-while-io.out
│   │       ├── image-fleecing
│   │       ├── image-fleecing.out
│   │       ├── inactive-node-nbd
│   │       ├── inactive-node-nbd.out
│   │       ├── iothreads-commit-active
│   │       ├── iothreads-commit-active.out
│   │       ├── iothreads-create
│   │       ├── iothreads-create.out
│   │       ├── iothreads-nbd-export
│   │       ├── iothreads-nbd-export.out
│   │       ├── iothreads-resize
│   │       ├── iothreads-resize.out
│   │       ├── iothreads-stream
│   │       ├── iothreads-stream.out
│   │       ├── iov-padding
│   │       ├── iov-padding.out
│   │       ├── luks-detached-header
│   │       ├── luks-detached-header.out
│   │       ├── migrate-bitmaps-postcopy-test
│   │       ├── migrate-bitmaps-postcopy-test.out
│   │       ├── migrate-bitmaps-test
│   │       ├── migrate-bitmaps-test.out
│   │       ├── migrate-during-backup
│   │       ├── migrate-during-backup.out
│   │       ├── migration-permissions
│   │       ├── migration-permissions.out
│   │       ├── mirror-change-copy-mode
│   │       ├── mirror-change-copy-mode.out
│   │       ├── mirror-ready-cancel-error
│   │       ├── mirror-ready-cancel-error.out
│   │       ├── mirror-sparse
│   │       ├── mirror-sparse.out
│   │       ├── mirror-top-perms
│   │       ├── mirror-top-perms.out
│   │       ├── nbd-multiconn
│   │       ├── nbd-multiconn.out
│   │       ├── nbd-qemu-allocation
│   │       ├── nbd-qemu-allocation.out
│   │       ├── nbd-reconnect-on-open
│   │       ├── nbd-reconnect-on-open.out
│   │       ├── nbd-tls-iothread
│   │       ├── nbd-tls-iothread.out
│   │       ├── parallels-checks
│   │       ├── parallels-checks.out
│   │       ├── parallels-read-bitmap
│   │       ├── parallels-read-bitmap.out
│   │       ├── qcow2-encryption
│   │       ├── qcow2-encryption.out
│   │       ├── qcow2-internal-snapshots
│   │       ├── qcow2-internal-snapshots.out
│   │       ├── qemu-img-bitmaps
│   │       ├── qemu-img-bitmaps.out
│   │       ├── qemu-img-close-errors
│   │       ├── qemu-img-close-errors.out
│   │       ├── qsd-jobs
│   │       ├── qsd-jobs.out
│   │       ├── qsd-migrate
│   │       ├── qsd-migrate.out
│   │       ├── regression-vhdx-log
│   │       ├── regression-vhdx-log.out
│   │       ├── remove-bitmap-from-backing
│   │       ├── remove-bitmap-from-backing.out
│   │       ├── reopen-file
│   │       ├── reopen-file.out
│   │       ├── stream-error-on-reset
│   │       ├── stream-error-on-reset.out
│   │       ├── stream-unaligned-prefetch
│   │       ├── stream-unaligned-prefetch.out
│   │       ├── stream-under-throttle
│   │       ├── stream-under-throttle.out
│   │       ├── vvfat
│   │       ├── vvfat.out
│   │       ├── write-zeroes-unmap
│   │       ├── write-zeroes-unmap.out
│   │       ├── zoned
│   │       └── zoned.out
│   ├── qtest
│   │   ├── ac97-test.c
│   │   ├── acpi-utils.c
│   │   ├── acpi-utils.h
│   │   ├── adm1266-test.c
│   │   ├── adm1272-test.c
│   │   ├── ahci-test.c
│   │   ├── am53c974-test.c
│   │   ├── arm-cpu-features.c
│   │   ├── aspeed_fsi-test.c
│   │   ├── aspeed_gpio-test.c
│   │   ├── aspeed_hace-test.c
│   │   ├── aspeed_smc-test.c
│   │   ├── aspeed-hace-utils.c
│   │   ├── aspeed-hace-utils.h
│   │   ├── aspeed-smc-utils.c
│   │   ├── aspeed-smc-utils.h
│   │   ├── ast2700-gpio-test.c
│   │   ├── ast2700-hace-test.c
│   │   ├── ast2700-smc-test.c
│   │   ├── bcm2835-dma-test.c
│   │   ├── bcm2835-i2c-test.c
│   │   ├── bios-tables-test-allowed-diff.h
│   │   ├── bios-tables-test.c
│   │   ├── boot-order-test.c
│   │   ├── boot-sector.c
│   │   ├── boot-sector.h
│   │   ├── boot-serial-test.c
│   │   ├── cdrom-test.c
│   │   ├── cmsdk-apb-dualtimer-test.c
│   │   ├── cmsdk-apb-timer-test.c
│   │   ├── cmsdk-apb-watchdog-test.c
│   │   ├── cpu-plug-test.c
│   │   ├── cxl-test.c
│   │   ├── dbus-display-test.c
│   │   ├── dbus-vmstate-test.c
│   │   ├── device-introspect-test.c
│   │   ├── device-plug-test.c
│   │   ├── display-vga-test.c
│   │   ├── dm163-test.c
│   │   ├── drive_del-test.c
│   │   ├── ds1338-test.c
│   │   ├── e1000-test.c
│   │   ├── e1000e-test.c
│   │   ├── eepro100-test.c
│   │   ├── emc141x-test.c
│   │   ├── endianness-test.c
│   │   ├── erst-test.c
│   │   ├── es1370-test.c
│   │   ├── fdc-test.c
│   │   ├── fuzz
│   │   │   ├── fuzz.c
│   │   │   ├── fuzz.h
│   │   │   ├── generic_fuzz_configs.h
│   │   │   ├── generic_fuzz.c
│   │   │   ├── i440fx_fuzz.c
│   │   │   ├── meson.build
│   │   │   ├── qos_fuzz.c
│   │   │   ├── qos_fuzz.h
│   │   │   ├── qtest_wrappers.c
│   │   │   ├── virtio_blk_fuzz.c
│   │   │   ├── virtio_net_fuzz.c
│   │   │   └── virtio_scsi_fuzz.c
│   │   ├── fuzz-e1000e-test.c
│   │   ├── fuzz-lsi53c895a-test.c
│   │   ├── fuzz-megasas-test.c
│   │   ├── fuzz-sb16-test.c
│   │   ├── fuzz-sdcard-test.c
│   │   ├── fuzz-virtio-scsi-test.c
│   │   ├── fuzz-xlnx-dp-test.c
│   │   ├── fw_cfg-test.c
│   │   ├── hd-geo-test.c
│   │   ├── hexloader-test.c
│   │   ├── i440fx-test.c
│   │   ├── i82801b11-test.c
│   │   ├── ide-test.c
│   │   ├── igb-test.c
│   │   ├── intel-hda-test.c
│   │   ├── intel-iommu-test.c
│   │   ├── ioh3420-test.c
│   │   ├── ipmi-bt-test.c
│   │   ├── ipmi-kcs-test.c
│   │   ├── ipoctal232-test.c
│   │   ├── isl_pmbus_vr-test.c
│   │   ├── ivshmem-test.c
│   │   ├── libqmp.c
│   │   ├── libqmp.h
│   │   ├── libqos
│   │   │   ├── aarch64-xlnx-zcu102-machine.c
│   │   │   ├── ahci.c
│   │   │   ├── ahci.h
│   │   │   ├── arm-imx25-pdk-machine.c
│   │   │   ├── arm-raspi2-machine.c
│   │   │   ├── arm-sabrelite-machine.c
│   │   │   ├── arm-smdkc210-machine.c
│   │   │   ├── arm-virt-machine.c
│   │   │   ├── arm-xilinx-zynq-a9-machine.c
│   │   │   ├── e1000e.c
│   │   │   ├── e1000e.h
│   │   │   ├── fw_cfg.c
│   │   │   ├── fw_cfg.h
│   │   │   ├── generic-pcihost.c
│   │   │   ├── generic-pcihost.h
│   │   │   ├── i2c-imx.c
│   │   │   ├── i2c-omap.c
│   │   │   ├── i2c.c
│   │   │   ├── i2c.h
│   │   │   ├── igb.c
│   │   │   ├── libqos-malloc.c
│   │   │   ├── libqos-malloc.h
│   │   │   ├── libqos-pc.c
│   │   │   ├── libqos-pc.h
│   │   │   ├── libqos-spapr.c
│   │   │   ├── libqos-spapr.h
│   │   │   ├── libqos.c
│   │   │   ├── libqos.h
│   │   │   ├── loongarch-virt-machine.c
│   │   │   ├── malloc-pc.c
│   │   │   ├── malloc-pc.h
│   │   │   ├── malloc-spapr.c
│   │   │   ├── malloc-spapr.h
│   │   │   ├── meson.build
│   │   │   ├── pci-pc.c
│   │   │   ├── pci-pc.h
│   │   │   ├── pci-spapr.c
│   │   │   ├── pci-spapr.h
│   │   │   ├── pci.c
│   │   │   ├── pci.h
│   │   │   ├── ppc64_pseries-machine.c
│   │   │   ├── qgraph_internal.h
│   │   │   ├── qgraph.c
│   │   │   ├── qgraph.h
│   │   │   ├── qos_external.c
│   │   │   ├── qos_external.h
│   │   │   ├── riscv-iommu.c
│   │   │   ├── riscv-iommu.h
│   │   │   ├── riscv-virt-machine.c
│   │   │   ├── rtas.c
│   │   │   ├── rtas.h
│   │   │   ├── sdhci-cmd.c
│   │   │   ├── sdhci-cmd.h
│   │   │   ├── sdhci.c
│   │   │   ├── sdhci.h
│   │   │   ├── tpci200.c
│   │   │   ├── usb.c
│   │   │   ├── usb.h
│   │   │   ├── vhost-user-blk.c
│   │   │   ├── vhost-user-blk.h
│   │   │   ├── virtio-9p-client.c
│   │   │   ├── virtio-9p-client.h
│   │   │   ├── virtio-9p.c
│   │   │   ├── virtio-9p.h
│   │   │   ├── virtio-balloon.c
│   │   │   ├── virtio-balloon.h
│   │   │   ├── virtio-blk.c
│   │   │   ├── virtio-blk.h
│   │   │   ├── virtio-gpio.c
│   │   │   ├── virtio-gpio.h
│   │   │   ├── virtio-iommu.c
│   │   │   ├── virtio-iommu.h
│   │   │   ├── virtio-mmio.c
│   │   │   ├── virtio-mmio.h
│   │   │   ├── virtio-net.c
│   │   │   ├── virtio-net.h
│   │   │   ├── virtio-pci-modern.c
│   │   │   ├── virtio-pci-modern.h
│   │   │   ├── virtio-pci.c
│   │   │   ├── virtio-pci.h
│   │   │   ├── virtio-rng.c
│   │   │   ├── virtio-rng.h
│   │   │   ├── virtio-scmi.c
│   │   │   ├── virtio-scmi.h
│   │   │   ├── virtio-scsi.c
│   │   │   ├── virtio-scsi.h
│   │   │   ├── virtio-serial.c
│   │   │   ├── virtio-serial.h
│   │   │   ├── virtio.c
│   │   │   ├── virtio.h
│   │   │   └── x86_64_pc-machine.c
│   │   ├── libqtest-single.h
│   │   ├── libqtest.c
│   │   ├── libqtest.h
│   │   ├── lpc-ich9-test.c
│   │   ├── lsm303dlhc-mag-test.c
│   │   ├── m48t59-test.c
│   │   ├── machine-none-test.c
│   │   ├── max34451-test.c
│   │   ├── megasas-test.c
│   │   ├── meson.build
│   │   ├── microbit-test.c
│   │   ├── migration
│   │   │   ├── aarch64
│   │   │   │   ├── a-b-kernel.h
│   │   │   │   ├── a-b-kernel.S
│   │   │   │   └── Makefile
│   │   │   ├── bootfile.c
│   │   │   ├── bootfile.h
│   │   │   ├── compression-tests.c
│   │   │   ├── cpr-tests.c
│   │   │   ├── file-tests.c
│   │   │   ├── framework.c
│   │   │   ├── framework.h
│   │   │   ├── i386
│   │   │   │   ├── a-b-bootblock.h
│   │   │   │   ├── a-b-bootblock.S
│   │   │   │   └── Makefile
│   │   │   ├── Makefile
│   │   │   ├── migration-qmp.c
│   │   │   ├── migration-qmp.h
│   │   │   ├── migration-util.c
│   │   │   ├── migration-util.h
│   │   │   ├── misc-tests.c
│   │   │   ├── postcopy-tests.c
│   │   │   ├── ppc64
│   │   │   │   ├── a-b-kernel.h
│   │   │   │   ├── a-b-kernel.S
│   │   │   │   └── Makefile
│   │   │   ├── precopy-tests.c
│   │   │   ├── s390x
│   │   │   │   ├── a-b-bios.c
│   │   │   │   ├── a-b-bios.h
│   │   │   │   └── Makefile
│   │   │   └── tls-tests.c
│   │   ├── migration-test.c
│   │   ├── modules-test.c
│   │   ├── ne2000-test.c
│   │   ├── netdev-socket.c
│   │   ├── npcm_gmac-test.c
│   │   ├── npcm7xx_adc-test.c
│   │   ├── npcm7xx_emc-test.c
│   │   ├── npcm7xx_gpio-test.c
│   │   ├── npcm7xx_pwm-test.c
│   │   ├── npcm7xx_rng-test.c
│   │   ├── npcm7xx_sdhci-test.c
│   │   ├── npcm7xx_smbus-test.c
│   │   ├── npcm7xx_timer-test.c
│   │   ├── npcm7xx_watchdog_timer-test.c
│   │   ├── numa-test.c
│   │   ├── nvme-test.c
│   │   ├── pca9552-test.c
│   │   ├── pci-test.c
│   │   ├── pcnet-test.c
│   │   ├── pflash-cfi02-test.c
│   │   ├── pnv-host-i2c-test.c
│   │   ├── pnv-spi-seeprom-test.c
│   │   ├── pnv-xive2-common.c
│   │   ├── pnv-xive2-common.h
│   │   ├── pnv-xive2-flush-sync.c
│   │   ├── pnv-xive2-nvpg_bar.c
│   │   ├── pnv-xive2-test.c
│   │   ├── pnv-xscom-test.c
│   │   ├── pnv-xscom.h
│   │   ├── ppc-util.h
│   │   ├── prom-env-test.c
│   │   ├── pvpanic-pci-test.c
│   │   ├── pvpanic-test.c
│   │   ├── pxe-test.c
│   │   ├── q35-test.c
│   │   ├── qmp-cmd-test.c
│   │   ├── qmp-test.c
│   │   ├── qom-test.c
│   │   ├── qos-test.c
│   │   ├── qtest_aspeed.c
│   │   ├── qtest_aspeed.h
│   │   ├── readconfig-test.c
│   │   ├── riscv-csr-test.c
│   │   ├── riscv-iommu-test.c
│   │   ├── rs5c372-test.c
│   │   ├── rtas-test.c
│   │   ├── rtc-test.c
│   │   ├── rtl8139-test.c
│   │   ├── sdhci-test.c
│   │   ├── sifive-e-aon-watchdog-test.c
│   │   ├── spapr-phb-test.c
│   │   ├── sse-timer-test.c
│   │   ├── stm32l4x5_exti-test.c
│   │   ├── stm32l4x5_gpio-test.c
│   │   ├── stm32l4x5_rcc-test.c
│   │   ├── stm32l4x5_syscfg-test.c
│   │   ├── stm32l4x5_usart-test.c
│   │   ├── stm32l4x5.h
│   │   ├── tco-test.c
│   │   ├── test-arm-mptimer.c
│   │   ├── test-filter-mirror.c
│   │   ├── test-filter-redirector.c
│   │   ├── test-hmp.c
│   │   ├── test-netfilter.c
│   │   ├── test-x86-cpuid-compat.c
│   │   ├── tmp105-test.c
│   │   ├── tpm-crb-swtpm-test.c
│   │   ├── tpm-crb-test.c
│   │   ├── tpm-emu.c
│   │   ├── tpm-emu.h
│   │   ├── tpm-tests.c
│   │   ├── tpm-tests.h
│   │   ├── tpm-tis-device-swtpm-test.c
│   │   ├── tpm-tis-device-test.c
│   │   ├── tpm-tis-i2c-test.c
│   │   ├── tpm-tis-swtpm-test.c
│   │   ├── tpm-tis-test.c
│   │   ├── tpm-tis-util.c
│   │   ├── tpm-tis-util.h
│   │   ├── tpm-util.c
│   │   ├── tpm-util.h
│   │   ├── tulip-test.c
│   │   ├── ufs-test.c
│   │   ├── usb-hcd-ehci-test.c
│   │   ├── usb-hcd-ohci-test.c
│   │   ├── usb-hcd-uhci-test.c
│   │   ├── usb-hcd-xhci-test.c
│   │   ├── vhost-user-blk-test.c
│   │   ├── vhost-user-test.c
│   │   ├── virtio-9p-test.c
│   │   ├── virtio-balloon-test.c
│   │   ├── virtio-blk-test.c
│   │   ├── virtio-ccw-test.c
│   │   ├── virtio-iommu-test.c
│   │   ├── virtio-net-failover.c
│   │   ├── virtio-net-test.c
│   │   ├── virtio-rng-test.c
│   │   ├── virtio-scsi-test.c
│   │   ├── virtio-serial-test.c
│   │   ├── virtio-test.c
│   │   ├── vmcoreinfo-test.c
│   │   ├── vmgenid-test.c
│   │   ├── vmxnet3-test.c
│   │   ├── vnc-display-test.c
│   │   ├── wdt_ib700-test.c
│   │   ├── xlnx-can-test.c
│   │   ├── xlnx-canfd-test.c
│   │   └── xlnx-versal-trng-test.c
│   ├── rocker
│   │   ├── all
│   │   ├── bridge
│   │   ├── bridge-stp
│   │   ├── bridge-vlan
│   │   ├── bridge-vlan-stp
│   │   ├── port
│   │   ├── README
│   │   └── tut.dot
│   ├── tcg
│   │   ├── aarch64
│   │   │   ├── bti-1.c
│   │   │   ├── bti-2.c
│   │   │   ├── bti-3.c
│   │   │   ├── bti-crt.c.inc
│   │   │   ├── dcpodp.c
│   │   │   ├── dcpop.c
│   │   │   ├── fcvt.ref
│   │   │   ├── float_convd.ref
│   │   │   ├── float_convs.ref
│   │   │   ├── float_madds.ref
│   │   │   ├── gdbstub
│   │   │   │   ├── test-mte.py
│   │   │   │   ├── test-sve-ioctl.py
│   │   │   │   └── test-sve.py
│   │   │   ├── lse2-fault.c
│   │   │   ├── Makefile.softmmu-target
│   │   │   ├── Makefile.target
│   │   │   ├── mte-1.c
│   │   │   ├── mte-2.c
│   │   │   ├── mte-3.c
│   │   │   ├── mte-4.c
│   │   │   ├── mte-5.c
│   │   │   ├── mte-6.c
│   │   │   ├── mte-7.c
│   │   │   ├── mte-8.c
│   │   │   ├── mte.h
│   │   │   ├── pauth-1.c
│   │   │   ├── pauth-2.c
│   │   │   ├── pauth-4.c
│   │   │   ├── pauth-5.c
│   │   │   ├── pauth.h
│   │   │   ├── pcalign-a64.c
│   │   │   ├── semicall.h
│   │   │   ├── sme-fmopa-1.c
│   │   │   ├── sme-fmopa-2.c
│   │   │   ├── sme-fmopa-3.c
│   │   │   ├── sme-outprod1.c
│   │   │   ├── sme-smopa-1.c
│   │   │   ├── sme-smopa-2.c
│   │   │   ├── sve-ioctls.c
│   │   │   ├── sve-str.c
│   │   │   ├── sysregs.c
│   │   │   ├── system
│   │   │   │   ├── boot.S
│   │   │   │   ├── feat-xs.c
│   │   │   │   ├── kernel.ld
│   │   │   │   ├── mte.S
│   │   │   │   ├── pauth-3.c
│   │   │   │   ├── semiconsole.c
│   │   │   │   ├── semiheap.c
│   │   │   │   └── vtimer.c
│   │   │   ├── test-2150.c
│   │   │   ├── test-2248.c
│   │   │   ├── test-2375.c
│   │   │   ├── test-826.c
│   │   │   └── test-aes.c
│   │   ├── aarch64_be
│   │   │   ├── hello.c
│   │   │   └── Makefile.target
│   │   ├── alpha
│   │   │   ├── hello-alpha.c
│   │   │   ├── Makefile.softmmu-target
│   │   │   ├── Makefile.target
│   │   │   ├── system
│   │   │   │   ├── boot.S
│   │   │   │   └── kernel.ld
│   │   │   ├── test-cond.c
│   │   │   ├── test-cvttq.c
│   │   │   └── test-ovf.c
│   │   ├── arm
│   │   │   ├── commpage.c
│   │   │   ├── fcvt.c
│   │   │   ├── fcvt.ref
│   │   │   ├── float_convd.ref
│   │   │   ├── float_convs.ref
│   │   │   ├── float_madds.ref
│   │   │   ├── hello-arm.c
│   │   │   ├── Makefile.softmmu-target
│   │   │   ├── Makefile.target
│   │   │   ├── pcalign-a32.c
│   │   │   ├── README
│   │   │   ├── semicall.h
│   │   │   └── system
│   │   │       ├── boot.S
│   │   │       ├── kernel.ld
│   │   │       ├── semiconsole.c
│   │   │       ├── test-armv6m-undef.ld
│   │   │       └── test-armv6m-undef.S
│   │   ├── hexagon
│   │   │   ├── atomics.c
│   │   │   ├── brev.c
│   │   │   ├── circ.c
│   │   │   ├── crt.S
│   │   │   ├── dual_stores.c
│   │   │   ├── first.S
│   │   │   ├── float_convd.ref
│   │   │   ├── float_convs.ref
│   │   │   ├── float_madds.ref
│   │   │   ├── fpstuff.c
│   │   │   ├── hex_sigsegv.c
│   │   │   ├── hex_test.h
│   │   │   ├── hvx_histogram_input.h
│   │   │   ├── hvx_histogram_row.h
│   │   │   ├── hvx_histogram_row.S
│   │   │   ├── hvx_histogram.c
│   │   │   ├── hvx_misc.c
│   │   │   ├── hvx_misc.h
│   │   │   ├── invalid-slots.c
│   │   │   ├── load_align.c
│   │   │   ├── load_unpack.c
│   │   │   ├── Makefile.target
│   │   │   ├── mem_noshuf_exception.c
│   │   │   ├── mem_noshuf.c
│   │   │   ├── misc.c
│   │   │   ├── multi_result.c
│   │   │   ├── overflow.c
│   │   │   ├── preg_alias.c
│   │   │   ├── read_write_overlap.c
│   │   │   ├── reg_mut.c
│   │   │   ├── scatter_gather.c
│   │   │   ├── signal_context.c
│   │   │   ├── test_abs.S
│   │   │   ├── test_bitcnt.S
│   │   │   ├── test_bitsplit.S
│   │   │   ├── test_call.S
│   │   │   ├── test_clobber.S
│   │   │   ├── test_cmp.S
│   │   │   ├── test_dotnew.S
│   │   │   ├── test_ext.S
│   │   │   ├── test_fibonacci.S
│   │   │   ├── test_hl.S
│   │   │   ├── test_hwloops.S
│   │   │   ├── test_jmp.S
│   │   │   ├── test_lsr.S
│   │   │   ├── test_mpyi.S
│   │   │   ├── test_packet.S
│   │   │   ├── test_reorder.S
│   │   │   ├── test_round.S
│   │   │   ├── test_vavgw.S
│   │   │   ├── test_vcmpb.S
│   │   │   ├── test_vcmpw.S
│   │   │   ├── test_vlsrw.S
│   │   │   ├── test_vmaxh.S
│   │   │   ├── test_vminh.S
│   │   │   ├── test_vpmpyh.S
│   │   │   ├── test_vspliceb.S
│   │   │   ├── unaligned_pc.c
│   │   │   ├── usr.c
│   │   │   ├── v68_hvx.c
│   │   │   ├── v68_scalar.c
│   │   │   ├── v69_hvx.c
│   │   │   ├── v6mpy_ref.c.inc
│   │   │   ├── v73_scalar.c
│   │   │   └── vector_add_int.c
│   │   ├── hppa
│   │   │   ├── Makefile.target
│   │   │   └── stby.c
│   │   ├── i386
│   │   │   ├── float_convd.conf
│   │   │   ├── float_convs.ref
│   │   │   ├── hello-i386.c
│   │   │   ├── Makefile.softmmu-target
│   │   │   ├── Makefile.target
│   │   │   ├── README
│   │   │   ├── system
│   │   │   │   ├── boot.S
│   │   │   │   └── kernel.ld
│   │   │   ├── test-3dnow.c
│   │   │   ├── test-aes.c
│   │   │   ├── test-avx.c
│   │   │   ├── test-avx.py
│   │   │   ├── test-flags.c
│   │   │   ├── test-i386-adcox.c
│   │   │   ├── test-i386-bmi2.c
│   │   │   ├── test-i386-code16.S
│   │   │   ├── test-i386-f2xm1.c
│   │   │   ├── test-i386-fbstp.c
│   │   │   ├── test-i386-fisttp.c
│   │   │   ├── test-i386-fldcst.c
│   │   │   ├── test-i386-fp-exceptions.c
│   │   │   ├── test-i386-fpatan.c
│   │   │   ├── test-i386-fprem.c
│   │   │   ├── test-i386-fscale.c
│   │   │   ├── test-i386-fxam.c
│   │   │   ├── test-i386-fxtract.c
│   │   │   ├── test-i386-fyl2x.c
│   │   │   ├── test-i386-fyl2xp1.c
│   │   │   ├── test-i386-muldiv.h
│   │   │   ├── test-i386-pcmpistri.c
│   │   │   ├── test-i386-pseudo-denormal.c
│   │   │   ├── test-i386-shift.h
│   │   │   ├── test-i386-snan-convert.c
│   │   │   ├── test-i386-sse-exceptions.c
│   │   │   ├── test-i386-ssse3.c
│   │   │   ├── test-i386-vm86.S
│   │   │   ├── test-i386.c
│   │   │   ├── test-i386.h
│   │   │   ├── test-mmx.c
│   │   │   ├── test-mmx.py
│   │   │   └── x86.csv
│   │   ├── loongarch64
│   │   │   ├── float_convd.ref
│   │   │   ├── float_convs.ref
│   │   │   ├── float_madds.ref
│   │   │   ├── Makefile.softmmu-target
│   │   │   ├── Makefile.target
│   │   │   ├── system
│   │   │   │   ├── boot.S
│   │   │   │   ├── kernel.ld
│   │   │   │   └── regdef.h
│   │   │   ├── test_bit.c
│   │   │   ├── test_div.c
│   │   │   ├── test_fclass.c
│   │   │   ├── test_fcsr.c
│   │   │   ├── test_fpcom.c
│   │   │   └── test_pcadd.c
│   │   ├── m68k
│   │   │   ├── denormal.c
│   │   │   ├── Makefile.target
│   │   │   └── trap.c
│   │   ├── Makefile.target
│   │   ├── minilib
│   │   │   ├── Makefile.target
│   │   │   ├── minilib.h
│   │   │   └── printf.c
│   │   ├── mips
│   │   │   ├── hello-mips.c
│   │   │   ├── include
│   │   │   │   ├── test_inputs_128.h
│   │   │   │   ├── test_inputs_32.h
│   │   │   │   ├── test_inputs_64.h
│   │   │   │   ├── test_utils_128.h
│   │   │   │   ├── test_utils_32.h
│   │   │   │   ├── test_utils_64.h
│   │   │   │   ├── wrappers_mips64r6.h
│   │   │   │   └── wrappers_msa.h
│   │   │   ├── Makefile.target
│   │   │   ├── README
│   │   │   └── user
│   │   │       ├── ase
│   │   │       │   ├── dsp
│   │   │       │   │   ├── Makefile
│   │   │       │   │   ├── test_dsp_r1_absq_s_ph.c
│   │   │       │   │   ├── test_dsp_r1_absq_s_w.c
│   │   │       │   │   ├── test_dsp_r1_addq_ph.c
│   │   │       │   │   ├── test_dsp_r1_addq_s_ph.c
│   │   │       │   │   ├── test_dsp_r1_addq_s_w.c
│   │   │       │   │   ├── test_dsp_r1_addsc.c
│   │   │       │   │   ├── test_dsp_r1_addu_qb.c
│   │   │       │   │   ├── test_dsp_r1_addu_s_qb.c
│   │   │       │   │   ├── test_dsp_r1_addwc.c
│   │   │       │   │   ├── test_dsp_r1_bitrev.c
│   │   │       │   │   ├── test_dsp_r1_bposge32.c
│   │   │       │   │   ├── test_dsp_r1_cmp_eq_ph.c
│   │   │       │   │   ├── test_dsp_r1_cmp_le_ph.c
│   │   │       │   │   ├── test_dsp_r1_cmp_lt_ph.c
│   │   │       │   │   ├── test_dsp_r1_cmpgu_eq_qb.c
│   │   │       │   │   ├── test_dsp_r1_cmpgu_le_qb.c
│   │   │       │   │   ├── test_dsp_r1_cmpgu_lt_qb.c
│   │   │       │   │   ├── test_dsp_r1_cmpu_eq_qb.c
│   │   │       │   │   ├── test_dsp_r1_cmpu_le_qb.c
│   │   │       │   │   ├── test_dsp_r1_cmpu_lt_qb.c
│   │   │       │   │   ├── test_dsp_r1_dpaq_s_w_ph.c
│   │   │       │   │   ├── test_dsp_r1_dpaq_sa_l_w.c
│   │   │       │   │   ├── test_dsp_r1_dpau_h_qbl.c
│   │   │       │   │   ├── test_dsp_r1_dpau_h_qbr.c
│   │   │       │   │   ├── test_dsp_r1_dpsq_s_w_ph.c
│   │   │       │   │   ├── test_dsp_r1_dpsq_sa_l_w.c
│   │   │       │   │   ├── test_dsp_r1_dpsu_h_qbl.c
│   │   │       │   │   ├── test_dsp_r1_dpsu_h_qbr.c
│   │   │       │   │   ├── test_dsp_r1_extp.c
│   │   │       │   │   ├── test_dsp_r1_extpdp.c
│   │   │       │   │   ├── test_dsp_r1_extpdpv.c
│   │   │       │   │   ├── test_dsp_r1_extpv.c
│   │   │       │   │   ├── test_dsp_r1_extr_r_w.c
│   │   │       │   │   ├── test_dsp_r1_extr_rs_w.c
│   │   │       │   │   ├── test_dsp_r1_extr_s_h.c
│   │   │       │   │   ├── test_dsp_r1_extr_w.c
│   │   │       │   │   ├── test_dsp_r1_extrv_r_w.c
│   │   │       │   │   ├── test_dsp_r1_extrv_rs_w.c
│   │   │       │   │   ├── test_dsp_r1_extrv_s_h.c
│   │   │       │   │   ├── test_dsp_r1_extrv_w.c
│   │   │       │   │   ├── test_dsp_r1_insv.c
│   │   │       │   │   ├── test_dsp_r1_lbux.c
│   │   │       │   │   ├── test_dsp_r1_lhx.c
│   │   │       │   │   ├── test_dsp_r1_lwx.c
│   │   │       │   │   ├── test_dsp_r1_madd.c
│   │   │       │   │   ├── test_dsp_r1_maddu.c
│   │   │       │   │   ├── test_dsp_r1_main.c
│   │   │       │   │   ├── test_dsp_r1_maq_s_w_phl.c
│   │   │       │   │   ├── test_dsp_r1_maq_s_w_phr.c
│   │   │       │   │   ├── test_dsp_r1_maq_sa_w_phl.c
│   │   │       │   │   ├── test_dsp_r1_maq_sa_w_phr.c
│   │   │       │   │   ├── test_dsp_r1_mfhi.c
│   │   │       │   │   ├── test_dsp_r1_mflo.c
│   │   │       │   │   ├── test_dsp_r1_modsub.c
│   │   │       │   │   ├── test_dsp_r1_msub.c
│   │   │       │   │   ├── test_dsp_r1_msubu.c
│   │   │       │   │   ├── test_dsp_r1_mthi.c
│   │   │       │   │   ├── test_dsp_r1_mthlip.c
│   │   │       │   │   ├── test_dsp_r1_mtlo.c
│   │   │       │   │   ├── test_dsp_r1_muleq_s_w_phl.c
│   │   │       │   │   ├── test_dsp_r1_muleq_s_w_phr.c
│   │   │       │   │   ├── test_dsp_r1_muleu_s_ph_qbl.c
│   │   │       │   │   ├── test_dsp_r1_muleu_s_ph_qbr.c
│   │   │       │   │   ├── test_dsp_r1_mulq_rs_ph.c
│   │   │       │   │   ├── test_dsp_r1_mult.c
│   │   │       │   │   ├── test_dsp_r1_multu.c
│   │   │       │   │   ├── test_dsp_r1_packrl_ph.c
│   │   │       │   │   ├── test_dsp_r1_pick_ph.c
│   │   │       │   │   ├── test_dsp_r1_pick_qb.c
│   │   │       │   │   ├── test_dsp_r1_preceq_w_phl.c
│   │   │       │   │   ├── test_dsp_r1_preceq_w_phr.c
│   │   │       │   │   ├── test_dsp_r1_precequ_ph_qbl.c
│   │   │       │   │   ├── test_dsp_r1_precequ_ph_qbla.c
│   │   │       │   │   ├── test_dsp_r1_precequ_ph_qbr.c
│   │   │       │   │   ├── test_dsp_r1_precequ_ph_qbra.c
│   │   │       │   │   ├── test_dsp_r1_preceu_ph_qbl.c
│   │   │       │   │   ├── test_dsp_r1_preceu_ph_qbla.c
│   │   │       │   │   ├── test_dsp_r1_preceu_ph_qbr.c
│   │   │       │   │   ├── test_dsp_r1_preceu_ph_qbra.c
│   │   │       │   │   ├── test_dsp_r1_precrq_ph_w.c
│   │   │       │   │   ├── test_dsp_r1_precrq_qb_ph.c
│   │   │       │   │   ├── test_dsp_r1_precrq_rs_ph_w.c
│   │   │       │   │   ├── test_dsp_r1_precrqu_s_qb_ph.c
│   │   │       │   │   ├── test_dsp_r1_raddu_w_qb.c
│   │   │       │   │   ├── test_dsp_r1_rddsp.c
│   │   │       │   │   ├── test_dsp_r1_repl_ph.c
│   │   │       │   │   ├── test_dsp_r1_repl_qb.c
│   │   │       │   │   ├── test_dsp_r1_replv_ph.c
│   │   │       │   │   ├── test_dsp_r1_replv_qb.c
│   │   │       │   │   ├── test_dsp_r1_shilo.c
│   │   │       │   │   ├── test_dsp_r1_shilov.c
│   │   │       │   │   ├── test_dsp_r1_shll_ph.c
│   │   │       │   │   ├── test_dsp_r1_shll_qb.c
│   │   │       │   │   ├── test_dsp_r1_shll_s_ph.c
│   │   │       │   │   ├── test_dsp_r1_shll_s_w.c
│   │   │       │   │   ├── test_dsp_r1_shllv_ph.c
│   │   │       │   │   ├── test_dsp_r1_shllv_qb.c
│   │   │       │   │   ├── test_dsp_r1_shllv_s_ph.c
│   │   │       │   │   ├── test_dsp_r1_shllv_s_w.c
│   │   │       │   │   ├── test_dsp_r1_shra_ph.c
│   │   │       │   │   ├── test_dsp_r1_shra_r_ph.c
│   │   │       │   │   ├── test_dsp_r1_shra_r_w.c
│   │   │       │   │   ├── test_dsp_r1_shrav_ph.c
│   │   │       │   │   ├── test_dsp_r1_shrav_r_ph.c
│   │   │       │   │   ├── test_dsp_r1_shrav_r_w.c
│   │   │       │   │   ├── test_dsp_r1_shrl_qb.c
│   │   │       │   │   ├── test_dsp_r1_shrlv_qb.c
│   │   │       │   │   ├── test_dsp_r1_subq_ph.c
│   │   │       │   │   ├── test_dsp_r1_subq_s_ph.c
│   │   │       │   │   ├── test_dsp_r1_subq_s_w.c
│   │   │       │   │   ├── test_dsp_r1_subu_qb.c
│   │   │       │   │   ├── test_dsp_r1_subu_s_qb.c
│   │   │       │   │   ├── test_dsp_r1_wrdsp.c
│   │   │       │   │   ├── test_dsp_r2_absq_s_qb.c
│   │   │       │   │   ├── test_dsp_r2_addqh_ph.c
│   │   │       │   │   ├── test_dsp_r2_addqh_r_ph.c
│   │   │       │   │   ├── test_dsp_r2_addqh_r_w.c
│   │   │       │   │   ├── test_dsp_r2_addqh_w.c
│   │   │       │   │   ├── test_dsp_r2_addu_ph.c
│   │   │       │   │   ├── test_dsp_r2_addu_s_ph.c
│   │   │       │   │   ├── test_dsp_r2_adduh_qb.c
│   │   │       │   │   ├── test_dsp_r2_adduh_r_qb.c
│   │   │       │   │   ├── test_dsp_r2_append.c
│   │   │       │   │   ├── test_dsp_r2_balign.c
│   │   │       │   │   ├── test_dsp_r2_cmpgdu_eq_qb.c
│   │   │       │   │   ├── test_dsp_r2_cmpgdu_le_qb.c
│   │   │       │   │   ├── test_dsp_r2_cmpgdu_lt_qb.c
│   │   │       │   │   ├── test_dsp_r2_dpa_w_ph.c
│   │   │       │   │   ├── test_dsp_r2_dpaqx_s_w_ph.c
│   │   │       │   │   ├── test_dsp_r2_dpaqx_sa_w_ph.c
│   │   │       │   │   ├── test_dsp_r2_dpax_w_ph.c
│   │   │       │   │   ├── test_dsp_r2_dps_w_ph.c
│   │   │       │   │   ├── test_dsp_r2_dpsqx_s_w_ph.c
│   │   │       │   │   ├── test_dsp_r2_dpsqx_sa_w_ph.c
│   │   │       │   │   ├── test_dsp_r2_dpsx_w_ph.c
│   │   │       │   │   ├── test_dsp_r2_mul_ph.c
│   │   │       │   │   ├── test_dsp_r2_mul_s_ph.c
│   │   │       │   │   ├── test_dsp_r2_mulq_rs_w.c
│   │   │       │   │   ├── test_dsp_r2_mulq_s_ph.c
│   │   │       │   │   ├── test_dsp_r2_mulq_s_w.c
│   │   │       │   │   ├── test_dsp_r2_mulsa_w_ph.c
│   │   │       │   │   ├── test_dsp_r2_mulsaq_s_w_ph.c
│   │   │       │   │   ├── test_dsp_r2_precr_qb_ph.c
│   │   │       │   │   ├── test_dsp_r2_precr_sra_ph_w.c
│   │   │       │   │   ├── test_dsp_r2_precr_sra_r_ph_w.c
│   │   │       │   │   ├── test_dsp_r2_prepend.c
│   │   │       │   │   ├── test_dsp_r2_shra_qb.c
│   │   │       │   │   ├── test_dsp_r2_shra_r_qb.c
│   │   │       │   │   ├── test_dsp_r2_shrav_qb.c
│   │   │       │   │   ├── test_dsp_r2_shrav_r_qb.c
│   │   │       │   │   ├── test_dsp_r2_shrl_ph.c
│   │   │       │   │   ├── test_dsp_r2_shrlv_ph.c
│   │   │       │   │   ├── test_dsp_r2_subqh_ph.c
│   │   │       │   │   ├── test_dsp_r2_subqh_r_ph.c
│   │   │       │   │   ├── test_dsp_r2_subqh_r_w.c
│   │   │       │   │   ├── test_dsp_r2_subqh_w.c
│   │   │       │   │   ├── test_dsp_r2_subu_ph.c
│   │   │       │   │   ├── test_dsp_r2_subu_s_ph.c
│   │   │       │   │   ├── test_dsp_r2_subuh_qb.c
│   │   │       │   │   └── test_dsp_r2_subuh_r_qb.c
│   │   │       │   └── msa
│   │   │       │       ├── bit-count
│   │   │       │       │   ├── test_msa_nloc_b.c
│   │   │       │       │   ├── test_msa_nloc_d.c
│   │   │       │       │   ├── test_msa_nloc_h.c
│   │   │       │       │   ├── test_msa_nloc_w.c
│   │   │       │       │   ├── test_msa_nlzc_b.c
│   │   │       │       │   ├── test_msa_nlzc_d.c
│   │   │       │       │   ├── test_msa_nlzc_h.c
│   │   │       │       │   ├── test_msa_nlzc_w.c
│   │   │       │       │   ├── test_msa_pcnt_b.c
│   │   │       │       │   ├── test_msa_pcnt_d.c
│   │   │       │       │   ├── test_msa_pcnt_h.c
│   │   │       │       │   └── test_msa_pcnt_w.c
│   │   │       │       ├── bit-move
│   │   │       │       │   ├── test_msa_binsl_b.c
│   │   │       │       │   ├── test_msa_binsl_d.c
│   │   │       │       │   ├── test_msa_binsl_h.c
│   │   │       │       │   ├── test_msa_binsl_w.c
│   │   │       │       │   ├── test_msa_binsr_b.c
│   │   │       │       │   ├── test_msa_binsr_d.c
│   │   │       │       │   ├── test_msa_binsr_h.c
│   │   │       │       │   ├── test_msa_binsr_w.c
│   │   │       │       │   ├── test_msa_bmnz_v.c
│   │   │       │       │   ├── test_msa_bmz_v.c
│   │   │       │       │   └── test_msa_bsel_v.c
│   │   │       │       ├── bit-set
│   │   │       │       │   ├── test_msa_bclr_b.c
│   │   │       │       │   ├── test_msa_bclr_d.c
│   │   │       │       │   ├── test_msa_bclr_h.c
│   │   │       │       │   ├── test_msa_bclr_w.c
│   │   │       │       │   ├── test_msa_bneg_b.c
│   │   │       │       │   ├── test_msa_bneg_d.c
│   │   │       │       │   ├── test_msa_bneg_h.c
│   │   │       │       │   ├── test_msa_bneg_w.c
│   │   │       │       │   ├── test_msa_bset_b.c
│   │   │       │       │   ├── test_msa_bset_d.c
│   │   │       │       │   ├── test_msa_bset_h.c
│   │   │       │       │   └── test_msa_bset_w.c
│   │   │       │       ├── fixed-multiply
│   │   │       │       │   ├── test_msa_madd_q_h.c
│   │   │       │       │   ├── test_msa_madd_q_w.c
│   │   │       │       │   ├── test_msa_maddr_q_h.c
│   │   │       │       │   ├── test_msa_maddr_q_w.c
│   │   │       │       │   ├── test_msa_msub_q_h.c
│   │   │       │       │   ├── test_msa_msub_q_w.c
│   │   │       │       │   ├── test_msa_msubr_q_h.c
│   │   │       │       │   ├── test_msa_msubr_q_w.c
│   │   │       │       │   ├── test_msa_mul_q_h.c
│   │   │       │       │   ├── test_msa_mul_q_w.c
│   │   │       │       │   ├── test_msa_mulr_q_h.c
│   │   │       │       │   └── test_msa_mulr_q_w.c
│   │   │       │       ├── float-max-min
│   │   │       │       │   ├── test_msa_fmax_a_d.c
│   │   │       │       │   ├── test_msa_fmax_a_w.c
│   │   │       │       │   ├── test_msa_fmax_d.c
│   │   │       │       │   ├── test_msa_fmax_w.c
│   │   │       │       │   ├── test_msa_fmin_a_d.c
│   │   │       │       │   ├── test_msa_fmin_a_w.c
│   │   │       │       │   ├── test_msa_fmin_d.c
│   │   │       │       │   └── test_msa_fmin_w.c
│   │   │       │       ├── int-add
│   │   │       │       │   ├── test_msa_add_a_b.c
│   │   │       │       │   ├── test_msa_add_a_d.c
│   │   │       │       │   ├── test_msa_add_a_h.c
│   │   │       │       │   ├── test_msa_add_a_w.c
│   │   │       │       │   ├── test_msa_adds_a_b.c
│   │   │       │       │   ├── test_msa_adds_a_d.c
│   │   │       │       │   ├── test_msa_adds_a_h.c
│   │   │       │       │   ├── test_msa_adds_a_w.c
│   │   │       │       │   ├── test_msa_adds_s_b.c
│   │   │       │       │   ├── test_msa_adds_s_d.c
│   │   │       │       │   ├── test_msa_adds_s_h.c
│   │   │       │       │   ├── test_msa_adds_s_w.c
│   │   │       │       │   ├── test_msa_adds_u_b.c
│   │   │       │       │   ├── test_msa_adds_u_d.c
│   │   │       │       │   ├── test_msa_adds_u_h.c
│   │   │       │       │   ├── test_msa_adds_u_w.c
│   │   │       │       │   ├── test_msa_addv_b.c
│   │   │       │       │   ├── test_msa_addv_d.c
│   │   │       │       │   ├── test_msa_addv_h.c
│   │   │       │       │   ├── test_msa_addv_w.c
│   │   │       │       │   ├── test_msa_hadd_s_d.c
│   │   │       │       │   ├── test_msa_hadd_s_h.c
│   │   │       │       │   ├── test_msa_hadd_s_w.c
│   │   │       │       │   ├── test_msa_hadd_u_d.c
│   │   │       │       │   ├── test_msa_hadd_u_h.c
│   │   │       │       │   └── test_msa_hadd_u_w.c
│   │   │       │       ├── int-average
│   │   │       │       │   ├── test_msa_ave_s_b.c
│   │   │       │       │   ├── test_msa_ave_s_d.c
│   │   │       │       │   ├── test_msa_ave_s_h.c
│   │   │       │       │   ├── test_msa_ave_s_w.c
│   │   │       │       │   ├── test_msa_ave_u_b.c
│   │   │       │       │   ├── test_msa_ave_u_d.c
│   │   │       │       │   ├── test_msa_ave_u_h.c
│   │   │       │       │   ├── test_msa_ave_u_w.c
│   │   │       │       │   ├── test_msa_aver_s_b.c
│   │   │       │       │   ├── test_msa_aver_s_d.c
│   │   │       │       │   ├── test_msa_aver_s_h.c
│   │   │       │       │   ├── test_msa_aver_s_w.c
│   │   │       │       │   ├── test_msa_aver_u_b.c
│   │   │       │       │   ├── test_msa_aver_u_d.c
│   │   │       │       │   ├── test_msa_aver_u_h.c
│   │   │       │       │   └── test_msa_aver_u_w.c
│   │   │       │       ├── int-compare
│   │   │       │       │   ├── test_msa_ceq_b.c
│   │   │       │       │   ├── test_msa_ceq_d.c
│   │   │       │       │   ├── test_msa_ceq_h.c
│   │   │       │       │   ├── test_msa_ceq_w.c
│   │   │       │       │   ├── test_msa_cle_s_b.c
│   │   │       │       │   ├── test_msa_cle_s_d.c
│   │   │       │       │   ├── test_msa_cle_s_h.c
│   │   │       │       │   ├── test_msa_cle_s_w.c
│   │   │       │       │   ├── test_msa_cle_u_b.c
│   │   │       │       │   ├── test_msa_cle_u_d.c
│   │   │       │       │   ├── test_msa_cle_u_h.c
│   │   │       │       │   ├── test_msa_cle_u_w.c
│   │   │       │       │   ├── test_msa_clt_s_b.c
│   │   │       │       │   ├── test_msa_clt_s_d.c
│   │   │       │       │   ├── test_msa_clt_s_h.c
│   │   │       │       │   ├── test_msa_clt_s_w.c
│   │   │       │       │   ├── test_msa_clt_u_b.c
│   │   │       │       │   ├── test_msa_clt_u_d.c
│   │   │       │       │   ├── test_msa_clt_u_h.c
│   │   │       │       │   └── test_msa_clt_u_w.c
│   │   │       │       ├── int-divide
│   │   │       │       │   ├── test_msa_div_s_b.c
│   │   │       │       │   ├── test_msa_div_s_d.c
│   │   │       │       │   ├── test_msa_div_s_h.c
│   │   │       │       │   ├── test_msa_div_s_w.c
│   │   │       │       │   ├── test_msa_div_u_b.c
│   │   │       │       │   ├── test_msa_div_u_d.c
│   │   │       │       │   ├── test_msa_div_u_h.c
│   │   │       │       │   └── test_msa_div_u_w.c
│   │   │       │       ├── int-dot-product
│   │   │       │       │   ├── test_msa_dotp_s_d.c
│   │   │       │       │   ├── test_msa_dotp_s_h.c
│   │   │       │       │   ├── test_msa_dotp_s_w.c
│   │   │       │       │   ├── test_msa_dotp_u_d.c
│   │   │       │       │   ├── test_msa_dotp_u_h.c
│   │   │       │       │   ├── test_msa_dotp_u_w.c
│   │   │       │       │   ├── test_msa_dpadd_s_d.c
│   │   │       │       │   ├── test_msa_dpadd_s_h.c
│   │   │       │       │   ├── test_msa_dpadd_s_w.c
│   │   │       │       │   ├── test_msa_dpadd_u_d.c
│   │   │       │       │   ├── test_msa_dpadd_u_h.c
│   │   │       │       │   ├── test_msa_dpadd_u_w.c
│   │   │       │       │   ├── test_msa_dpsub_s_d.c
│   │   │       │       │   ├── test_msa_dpsub_s_h.c
│   │   │       │       │   ├── test_msa_dpsub_s_w.c
│   │   │       │       │   ├── test_msa_dpsub_u_d.c
│   │   │       │       │   ├── test_msa_dpsub_u_h.c
│   │   │       │       │   └── test_msa_dpsub_u_w.c
│   │   │       │       ├── int-max-min
│   │   │       │       │   ├── test_msa_max_a_b.c
│   │   │       │       │   ├── test_msa_max_a_d.c
│   │   │       │       │   ├── test_msa_max_a_h.c
│   │   │       │       │   ├── test_msa_max_a_w.c
│   │   │       │       │   ├── test_msa_max_s_b.c
│   │   │       │       │   ├── test_msa_max_s_d.c
│   │   │       │       │   ├── test_msa_max_s_h.c
│   │   │       │       │   ├── test_msa_max_s_w.c
│   │   │       │       │   ├── test_msa_max_u_b.c
│   │   │       │       │   ├── test_msa_max_u_d.c
│   │   │       │       │   ├── test_msa_max_u_h.c
│   │   │       │       │   ├── test_msa_max_u_w.c
│   │   │       │       │   ├── test_msa_min_a_b.c
│   │   │       │       │   ├── test_msa_min_a_d.c
│   │   │       │       │   ├── test_msa_min_a_h.c
│   │   │       │       │   ├── test_msa_min_a_w.c
│   │   │       │       │   ├── test_msa_min_s_b.c
│   │   │       │       │   ├── test_msa_min_s_d.c
│   │   │       │       │   ├── test_msa_min_s_h.c
│   │   │       │       │   ├── test_msa_min_s_w.c
│   │   │       │       │   ├── test_msa_min_u_b.c
│   │   │       │       │   ├── test_msa_min_u_d.c
│   │   │       │       │   ├── test_msa_min_u_h.c
│   │   │       │       │   └── test_msa_min_u_w.c
│   │   │       │       ├── int-modulo
│   │   │       │       │   ├── test_msa_mod_s_b.c
│   │   │       │       │   ├── test_msa_mod_s_d.c
│   │   │       │       │   ├── test_msa_mod_s_h.c
│   │   │       │       │   ├── test_msa_mod_s_w.c
│   │   │       │       │   ├── test_msa_mod_u_b.c
│   │   │       │       │   ├── test_msa_mod_u_d.c
│   │   │       │       │   ├── test_msa_mod_u_h.c
│   │   │       │       │   └── test_msa_mod_u_w.c
│   │   │       │       ├── int-multiply
│   │   │       │       │   ├── test_msa_maddv_b.c
│   │   │       │       │   ├── test_msa_maddv_d.c
│   │   │       │       │   ├── test_msa_maddv_h.c
│   │   │       │       │   ├── test_msa_maddv_w.c
│   │   │       │       │   ├── test_msa_msubv_b.c
│   │   │       │       │   ├── test_msa_msubv_d.c
│   │   │       │       │   ├── test_msa_msubv_h.c
│   │   │       │       │   ├── test_msa_msubv_w.c
│   │   │       │       │   ├── test_msa_mulv_b.c
│   │   │       │       │   ├── test_msa_mulv_d.c
│   │   │       │       │   ├── test_msa_mulv_h.c
│   │   │       │       │   └── test_msa_mulv_w.c
│   │   │       │       ├── int-subtract
│   │   │       │       │   ├── test_msa_asub_s_b.c
│   │   │       │       │   ├── test_msa_asub_s_d.c
│   │   │       │       │   ├── test_msa_asub_s_h.c
│   │   │       │       │   ├── test_msa_asub_s_w.c
│   │   │       │       │   ├── test_msa_asub_u_b.c
│   │   │       │       │   ├── test_msa_asub_u_d.c
│   │   │       │       │   ├── test_msa_asub_u_h.c
│   │   │       │       │   ├── test_msa_asub_u_w.c
│   │   │       │       │   ├── test_msa_hsub_s_d.c
│   │   │       │       │   ├── test_msa_hsub_s_h.c
│   │   │       │       │   ├── test_msa_hsub_s_w.c
│   │   │       │       │   ├── test_msa_hsub_u_d.c
│   │   │       │       │   ├── test_msa_hsub_u_h.c
│   │   │       │       │   ├── test_msa_hsub_u_w.c
│   │   │       │       │   ├── test_msa_subs_s_b.c
│   │   │       │       │   ├── test_msa_subs_s_d.c
│   │   │       │       │   ├── test_msa_subs_s_h.c
│   │   │       │       │   ├── test_msa_subs_s_w.c
│   │   │       │       │   ├── test_msa_subs_u_b.c
│   │   │       │       │   ├── test_msa_subs_u_d.c
│   │   │       │       │   ├── test_msa_subs_u_h.c
│   │   │       │       │   ├── test_msa_subs_u_w.c
│   │   │       │       │   ├── test_msa_subsus_u_b.c
│   │   │       │       │   ├── test_msa_subsus_u_d.c
│   │   │       │       │   ├── test_msa_subsus_u_h.c
│   │   │       │       │   ├── test_msa_subsus_u_w.c
│   │   │       │       │   ├── test_msa_subsuu_s_b.c
│   │   │       │       │   ├── test_msa_subsuu_s_d.c
│   │   │       │       │   ├── test_msa_subsuu_s_h.c
│   │   │       │       │   ├── test_msa_subsuu_s_w.c
│   │   │       │       │   ├── test_msa_subv_b.c
│   │   │       │       │   ├── test_msa_subv_d.c
│   │   │       │       │   ├── test_msa_subv_h.c
│   │   │       │       │   └── test_msa_subv_w.c
│   │   │       │       ├── interleave
│   │   │       │       │   ├── test_msa_ilvev_b.c
│   │   │       │       │   ├── test_msa_ilvev_d.c
│   │   │       │       │   ├── test_msa_ilvev_h.c
│   │   │       │       │   ├── test_msa_ilvev_w.c
│   │   │       │       │   ├── test_msa_ilvl_b.c
│   │   │       │       │   ├── test_msa_ilvl_d.c
│   │   │       │       │   ├── test_msa_ilvl_h.c
│   │   │       │       │   ├── test_msa_ilvl_w.c
│   │   │       │       │   ├── test_msa_ilvod_b.c
│   │   │       │       │   ├── test_msa_ilvod_d.c
│   │   │       │       │   ├── test_msa_ilvod_h.c
│   │   │       │       │   ├── test_msa_ilvod_w.c
│   │   │       │       │   ├── test_msa_ilvr_b.c
│   │   │       │       │   ├── test_msa_ilvr_d.c
│   │   │       │       │   ├── test_msa_ilvr_h.c
│   │   │       │       │   └── test_msa_ilvr_w.c
│   │   │       │       ├── logic
│   │   │       │       │   ├── test_msa_and_v.c
│   │   │       │       │   ├── test_msa_nor_v.c
│   │   │       │       │   ├── test_msa_or_v.c
│   │   │       │       │   └── test_msa_xor_v.c
│   │   │       │       ├── move
│   │   │       │       │   └── test_msa_move_v.c
│   │   │       │       ├── pack
│   │   │       │       │   ├── test_msa_pckev_b.c
│   │   │       │       │   ├── test_msa_pckev_d.c
│   │   │       │       │   ├── test_msa_pckev_h.c
│   │   │       │       │   ├── test_msa_pckev_w.c
│   │   │       │       │   ├── test_msa_pckod_b.c
│   │   │       │       │   ├── test_msa_pckod_d.c
│   │   │       │       │   ├── test_msa_pckod_h.c
│   │   │       │       │   ├── test_msa_pckod_w.c
│   │   │       │       │   ├── test_msa_vshf_b.c
│   │   │       │       │   ├── test_msa_vshf_d.c
│   │   │       │       │   ├── test_msa_vshf_h.c
│   │   │       │       │   └── test_msa_vshf_w.c
│   │   │       │       ├── README
│   │   │       │       ├── shift
│   │   │       │       │   ├── test_msa_sll_b.c
│   │   │       │       │   ├── test_msa_sll_d.c
│   │   │       │       │   ├── test_msa_sll_h.c
│   │   │       │       │   ├── test_msa_sll_w.c
│   │   │       │       │   ├── test_msa_sra_b.c
│   │   │       │       │   ├── test_msa_sra_d.c
│   │   │       │       │   ├── test_msa_sra_h.c
│   │   │       │       │   ├── test_msa_sra_w.c
│   │   │       │       │   ├── test_msa_srar_b.c
│   │   │       │       │   ├── test_msa_srar_d.c
│   │   │       │       │   ├── test_msa_srar_h.c
│   │   │       │       │   ├── test_msa_srar_w.c
│   │   │       │       │   ├── test_msa_srl_b.c
│   │   │       │       │   ├── test_msa_srl_d.c
│   │   │       │       │   ├── test_msa_srl_h.c
│   │   │       │       │   ├── test_msa_srl_w.c
│   │   │       │       │   ├── test_msa_srlr_b.c
│   │   │       │       │   ├── test_msa_srlr_d.c
│   │   │       │       │   ├── test_msa_srlr_h.c
│   │   │       │       │   └── test_msa_srlr_w.c
│   │   │       │       ├── test_msa_compile_32r5eb.sh
│   │   │       │       ├── test_msa_compile_32r5el.sh
│   │   │       │       ├── test_msa_compile_64r6eb.sh
│   │   │       │       ├── test_msa_compile_64r6el.sh
│   │   │       │       ├── test_msa_run_32r5eb.sh
│   │   │       │       ├── test_msa_run_32r5el.sh
│   │   │       │       ├── test_msa_run_64r6eb.sh
│   │   │       │       └── test_msa_run_64r6el.sh
│   │   │       └── isa
│   │   │           ├── mips64r6
│   │   │           │   ├── bit-count
│   │   │           │   │   ├── test_mips64r6_clo.c
│   │   │           │   │   ├── test_mips64r6_clz.c
│   │   │           │   │   ├── test_mips64r6_dclo.c
│   │   │           │   │   └── test_mips64r6_dclz.c
│   │   │           │   ├── bit-swap
│   │   │           │   │   ├── test_mips64r6_bitswap.c
│   │   │           │   │   └── test_mips64r6_dbitswap.c
│   │   │           │   ├── int-multiply
│   │   │           │   │   ├── test_mips64r6_dmuh.c
│   │   │           │   │   ├── test_mips64r6_dmuhu.c
│   │   │           │   │   ├── test_mips64r6_dmul.c
│   │   │           │   │   ├── test_mips64r6_dmulu.c
│   │   │           │   │   ├── test_mips64r6_muh.c
│   │   │           │   │   ├── test_mips64r6_muhu.c
│   │   │           │   │   ├── test_mips64r6_mul.c
│   │   │           │   │   └── test_mips64r6_mulu.c
│   │   │           │   ├── logic
│   │   │           │   │   ├── test_mips64r6_and.c
│   │   │           │   │   ├── test_mips64r6_nor.c
│   │   │           │   │   ├── test_mips64r6_or.c
│   │   │           │   │   └── test_mips64r6_xor.c
│   │   │           │   └── shift
│   │   │           │       ├── test_mips64r6_dsllv.c
│   │   │           │       ├── test_mips64r6_dsrav.c
│   │   │           │       ├── test_mips64r6_dsrlv.c
│   │   │           │       ├── test_mips64r6_sllv.c
│   │   │           │       ├── test_mips64r6_srav.c
│   │   │           │       └── test_mips64r6_srlv.c
│   │   │           └── r5900
│   │   │               ├── Makefile
│   │   │               ├── test_r5900_div1.c
│   │   │               ├── test_r5900_divu1.c
│   │   │               ├── test_r5900_madd.c
│   │   │               ├── test_r5900_maddu.c
│   │   │               ├── test_r5900_mflohi1.c
│   │   │               ├── test_r5900_mtlohi1.c
│   │   │               ├── test_r5900_mult.c
│   │   │               └── test_r5900_multu.c
│   │   ├── multiarch
│   │   │   ├── arm-compat-semi
│   │   │   │   ├── semiconsole.c
│   │   │   │   └── semihosting.c
│   │   │   ├── catch-syscalls.c
│   │   │   ├── check-plugin-output.sh
│   │   │   ├── float_convd.c
│   │   │   ├── float_convs.c
│   │   │   ├── float_helpers.h
│   │   │   ├── float_madds.c
│   │   │   ├── follow-fork-mode.c
│   │   │   ├── gdbstub
│   │   │   │   ├── catch-syscalls.py
│   │   │   │   ├── follow-fork-mode-child.py
│   │   │   │   ├── follow-fork-mode-parent.py
│   │   │   │   ├── interrupt.py
│   │   │   │   ├── late-attach.py
│   │   │   │   ├── memory.py
│   │   │   │   ├── prot-none.py
│   │   │   │   ├── registers.py
│   │   │   │   ├── sha1.py
│   │   │   │   ├── test-proc-mappings.py
│   │   │   │   ├── test-qxfer-auxv-read.py
│   │   │   │   ├── test-qxfer-siginfo-read.py
│   │   │   │   └── test-thread-breakpoint.py
│   │   │   ├── late-attach.c
│   │   │   ├── libs
│   │   │   │   └── float_helpers.c
│   │   │   ├── linux
│   │   │   │   ├── linux-madvise.c
│   │   │   │   ├── linux-shmat-maps.c
│   │   │   │   ├── linux-shmat-null.c
│   │   │   │   ├── linux-sigrtminmax.c
│   │   │   │   ├── linux-test.c
│   │   │   │   └── test-vma.c
│   │   │   ├── Makefile.target
│   │   │   ├── munmap-pthread.c
│   │   │   ├── noexec.c.inc
│   │   │   ├── nop_func.h
│   │   │   ├── overflow.c
│   │   │   ├── prot-none.c
│   │   │   ├── README
│   │   │   ├── segfault.c
│   │   │   ├── sha1.c
│   │   │   ├── sha512.c
│   │   │   ├── sigbus.c
│   │   │   ├── signals.c
│   │   │   ├── sigreturn-sigmask.c
│   │   │   ├── system
│   │   │   │   ├── hello.c
│   │   │   │   ├── interrupt.c
│   │   │   │   ├── Makefile.softmmu-target
│   │   │   │   ├── memory.c
│   │   │   │   └── validate-memory-counts.py
│   │   │   ├── test-aes-main.c.inc
│   │   │   ├── test-mmap.c
│   │   │   ├── test-plugin-mem-access.c
│   │   │   ├── testthread.c
│   │   │   ├── threadcount.c
│   │   │   └── vma-pthread.c
│   │   ├── openrisc
│   │   │   ├── Makefile
│   │   │   ├── test_add.c
│   │   │   ├── test_addc.c
│   │   │   ├── test_addi.c
│   │   │   ├── test_addic.c
│   │   │   ├── test_and_or.c
│   │   │   ├── test_bf.c
│   │   │   ├── test_bnf.c
│   │   │   ├── test_div.c
│   │   │   ├── test_divu.c
│   │   │   ├── test_extx.c
│   │   │   ├── test_fx.c
│   │   │   ├── test_j.c
│   │   │   ├── test_jal.c
│   │   │   ├── test_lf_add.c
│   │   │   ├── test_lf_div.c
│   │   │   ├── test_lf_eqs.c
│   │   │   ├── test_lf_ges.c
│   │   │   ├── test_lf_gts.c
│   │   │   ├── test_lf_les.c
│   │   │   ├── test_lf_lts.c
│   │   │   ├── test_lf_mul.c
│   │   │   ├── test_lf_nes.c
│   │   │   ├── test_lf_rem.c
│   │   │   ├── test_lf_sub.c
│   │   │   ├── test_logic.c
│   │   │   ├── test_lx.c
│   │   │   ├── test_movhi.c
│   │   │   ├── test_mul.c
│   │   │   ├── test_muli.c
│   │   │   ├── test_mulu.c
│   │   │   ├── test_sfeq.c
│   │   │   ├── test_sfeqi.c
│   │   │   ├── test_sfges.c
│   │   │   ├── test_sfgesi.c
│   │   │   ├── test_sfgeu.c
│   │   │   ├── test_sfgeui.c
│   │   │   ├── test_sfgts.c
│   │   │   ├── test_sfgtsi.c
│   │   │   ├── test_sfgtu.c
│   │   │   ├── test_sfgtui.c
│   │   │   ├── test_sfles.c
│   │   │   ├── test_sflesi.c
│   │   │   ├── test_sfleu.c
│   │   │   ├── test_sfleui.c
│   │   │   ├── test_sflts.c
│   │   │   ├── test_sfltsi.c
│   │   │   ├── test_sfltu.c
│   │   │   ├── test_sfltui.c
│   │   │   ├── test_sfne.c
│   │   │   ├── test_sfnei.c
│   │   │   └── test_sub.c
│   │   ├── plugins
│   │   │   ├── bb.c
│   │   │   ├── empty.c
│   │   │   ├── inline.c
│   │   │   ├── insn.c
│   │   │   ├── mem.c
│   │   │   ├── meson.build
│   │   │   ├── reset.c
│   │   │   └── syscall.c
│   │   ├── ppc64
│   │   │   ├── bcdsub.c
│   │   │   ├── byte_reverse.c
│   │   │   ├── Makefile.target
│   │   │   ├── mffsce.c
│   │   │   ├── mtfsf.c
│   │   │   ├── non_signalling_xscv.c
│   │   │   ├── signal_save_restore_xer.c
│   │   │   ├── test-aes.c
│   │   │   ├── vector.c
│   │   │   ├── vsx_f2i_nan.c
│   │   │   └── xxspltw.c
│   │   ├── ppc64le
│   │   │   ├── float_convs.ref
│   │   │   ├── float_madds.ref
│   │   │   └── Makefile.target
│   │   ├── README
│   │   ├── riscv64
│   │   │   ├── issue1060.S
│   │   │   ├── Makefile.softmmu-target
│   │   │   ├── Makefile.target
│   │   │   ├── noexec.c
│   │   │   ├── semicall.h
│   │   │   ├── semihost.ld
│   │   │   ├── test-aes.c
│   │   │   ├── test-div.c
│   │   │   ├── test-fcvtmod.c
│   │   │   └── test-noc.S
│   │   ├── s390x
│   │   │   ├── add-logical-with-carry.c
│   │   │   ├── bal.S
│   │   │   ├── br-odd.S
│   │   │   ├── branch-relative-long.c
│   │   │   ├── cdsg.c
│   │   │   ├── cgebra.c
│   │   │   ├── cgrl-unaligned.S
│   │   │   ├── chrl.c
│   │   │   ├── cksm.S
│   │   │   ├── clc.c
│   │   │   ├── clgebr.c
│   │   │   ├── clm.S
│   │   │   ├── clrl-unaligned.S
│   │   │   ├── clst.c
│   │   │   ├── console.c
│   │   │   ├── crl-unaligned.S
│   │   │   ├── csst.c
│   │   │   ├── cvb.c
│   │   │   ├── cvd.c
│   │   │   ├── div.c
│   │   │   ├── epsw.c
│   │   │   ├── ex-branch.c
│   │   │   ├── ex-odd.S
│   │   │   ├── ex-relative-long.c
│   │   │   ├── ex-smc.c
│   │   │   ├── exrl-ssm-early.S
│   │   │   ├── exrl-trt.c
│   │   │   ├── exrl-trtr.c
│   │   │   ├── float.h
│   │   │   ├── fma.c
│   │   │   ├── gdbstub
│   │   │   │   ├── test-signals-s390x.py
│   │   │   │   └── test-svc.py
│   │   │   ├── head64.S
│   │   │   ├── hello-s390x-asm.S
│   │   │   ├── hello-s390x.c
│   │   │   ├── icm.S
│   │   │   ├── ipm.c
│   │   │   ├── laalg.c
│   │   │   ├── lae.c
│   │   │   ├── larl.c
│   │   │   ├── lcbb.c
│   │   │   ├── lgrl-unaligned.S
│   │   │   ├── llgfrl-unaligned.S
│   │   │   ├── locfhr.c
│   │   │   ├── long-double.c
│   │   │   ├── lpsw.S
│   │   │   ├── lpswe-early.S
│   │   │   ├── lpswe-unaligned.S
│   │   │   ├── lra.S
│   │   │   ├── lrl-unaligned.S
│   │   │   ├── Makefile.softmmu-target
│   │   │   ├── Makefile.target
│   │   │   ├── mc.S
│   │   │   ├── mdeb.c
│   │   │   ├── mie3-compl.c
│   │   │   ├── mie3-mvcrl.c
│   │   │   ├── mie3-sel.c
│   │   │   ├── mvc-smc.c
│   │   │   ├── mvc.c
│   │   │   ├── mvo.c
│   │   │   ├── mxdb.c
│   │   │   ├── noexec.c
│   │   │   ├── pack.c
│   │   │   ├── per.S
│   │   │   ├── pgm-specification-softmmu.S
│   │   │   ├── pgm-specification-user.c
│   │   │   ├── pgm-specification.mak
│   │   │   ├── precise-smc-softmmu.S
│   │   │   ├── precise-smc-user.c
│   │   │   ├── rxsbg.c
│   │   │   ├── sam.S
│   │   │   ├── shift.c
│   │   │   ├── signals-s390x.c
│   │   │   ├── softmmu.ld
│   │   │   ├── ssm-early.S
│   │   │   ├── stgrl-unaligned.S
│   │   │   ├── stosm-early.S
│   │   │   ├── stpq.S
│   │   │   ├── strl-unaligned.S
│   │   │   ├── trap.c
│   │   │   ├── ts.c
│   │   │   ├── unaligned-lowcore.S
│   │   │   ├── vcksm.c
│   │   │   ├── vfminmax.c
│   │   │   ├── vistr.c
│   │   │   ├── vrep.c
│   │   │   ├── vstl.c
│   │   │   ├── vx.h
│   │   │   ├── vxeh2_vcvt.c
│   │   │   ├── vxeh2_vlstr.c
│   │   │   ├── vxeh2_vs.c
│   │   │   └── vxeh2_vstrs.c
│   │   ├── sh4
│   │   │   ├── Makefile.target
│   │   │   ├── test-addv.c
│   │   │   ├── test-macl.c
│   │   │   ├── test-macw.c
│   │   │   └── test-subv.c
│   │   ├── tricore
│   │   │   ├── asm
│   │   │   │   ├── macros.h
│   │   │   │   ├── test_abs.S
│   │   │   │   ├── test_bmerge.S
│   │   │   │   ├── test_clz.S
│   │   │   │   ├── test_crcn.S
│   │   │   │   ├── test_dextr.S
│   │   │   │   ├── test_dvstep.S
│   │   │   │   ├── test_fadd.S
│   │   │   │   ├── test_fmul.S
│   │   │   │   ├── test_ftohp.S
│   │   │   │   ├── test_ftoi.S
│   │   │   │   ├── test_ftou.S
│   │   │   │   ├── test_hptof.S
│   │   │   │   ├── test_imask.S
│   │   │   │   ├── test_insert.S
│   │   │   │   ├── test_ld_bu.S
│   │   │   │   ├── test_ld_h.S
│   │   │   │   ├── test_madd.S
│   │   │   │   ├── test_msub.S
│   │   │   │   └── test_muls.S
│   │   │   ├── c
│   │   │   │   ├── crt0-tc2x.S
│   │   │   │   ├── test_boot_to_main.c
│   │   │   │   ├── test_context_save_areas.c
│   │   │   │   └── testdev_assert.h
│   │   │   ├── link.ld
│   │   │   └── Makefile.softmmu-target
│   │   ├── x86_64
│   │   │   ├── adox.c
│   │   │   ├── cmpxchg.c
│   │   │   ├── cross-modifying-code.c
│   │   │   ├── float_convd.ref
│   │   │   ├── float_convs.ref
│   │   │   ├── fma.c
│   │   │   ├── Makefile.softmmu-target
│   │   │   ├── Makefile.target
│   │   │   ├── noexec.c
│   │   │   ├── system
│   │   │   │   ├── boot.S
│   │   │   │   └── kernel.ld
│   │   │   ├── test-1648.c
│   │   │   ├── test-2175.c
│   │   │   ├── test-2413.c
│   │   │   └── vsyscall.c
│   │   ├── xtensa
│   │   │   ├── crt.S
│   │   │   ├── fpu.h
│   │   │   ├── linker.ld.S
│   │   │   ├── macros.inc
│   │   │   ├── Makefile.softmmu-target
│   │   │   ├── test_b.S
│   │   │   ├── test_bi.S
│   │   │   ├── test_boolean.S
│   │   │   ├── test_break.S
│   │   │   ├── test_bz.S
│   │   │   ├── test_cache.S
│   │   │   ├── test_clamps.S
│   │   │   ├── test_dfp0_arith.S
│   │   │   ├── test_exclusive.S
│   │   │   ├── test_extui.S
│   │   │   ├── test_flix.S
│   │   │   ├── test_fp_cpenable.S
│   │   │   ├── test_fp0_arith.S
│   │   │   ├── test_fp0_conv.S
│   │   │   ├── test_fp0_div.S
│   │   │   ├── test_fp0_sqrt.S
│   │   │   ├── test_fp1.S
│   │   │   ├── test_interrupt.S
│   │   │   ├── test_load_store.S
│   │   │   ├── test_loop.S
│   │   │   ├── test_lsc.S
│   │   │   ├── test_mac16.S
│   │   │   ├── test_max.S
│   │   │   ├── test_min.S
│   │   │   ├── test_mmu.S
│   │   │   ├── test_mul16.S
│   │   │   ├── test_mul32.S
│   │   │   ├── test_nsa.S
│   │   │   ├── test_phys_mem.S
│   │   │   ├── test_quo.S
│   │   │   ├── test_rem.S
│   │   │   ├── test_rst0.S
│   │   │   ├── test_s32c1i.S
│   │   │   ├── test_sar.S
│   │   │   ├── test_sext.S
│   │   │   ├── test_shift.S
│   │   │   ├── test_sr.S
│   │   │   ├── test_timer.S
│   │   │   ├── test_windowed.S
│   │   │   └── vectors.S
│   │   └── xtensaeb
│   │       └── Makefile.softmmu-target
│   ├── test-qht-par.c
│   ├── tsan
│   │   ├── ignore.tsan
│   │   └── suppressions.tsan
│   ├── uefi-test-tools
│   │   ├── build.sh
│   │   ├── LICENSE
│   │   ├── Makefile
│   │   ├── uefi-test-build.config
│   │   └── UefiTestToolsPkg
│   │       ├── BiosTablesTest
│   │       │   ├── BiosTablesTest.c
│   │       │   └── BiosTablesTest.inf
│   │       ├── Include
│   │       │   └── Guid
│   │       │       └── BiosTablesTest.h
│   │       ├── UefiTestToolsPkg.dec
│   │       └── UefiTestToolsPkg.dsc
│   ├── unit
│   │   ├── check-block-qdict.c
│   │   ├── check-qdict.c
│   │   ├── check-qjson.c
│   │   ├── check-qlist.c
│   │   ├── check-qlit.c
│   │   ├── check-qnull.c
│   │   ├── check-qnum.c
│   │   ├── check-qobject.c
│   │   ├── check-qom-interface.c
│   │   ├── check-qom-proplist.c
│   │   ├── check-qstring.c
│   │   ├── crypto-tls-psk-helpers.c
│   │   ├── crypto-tls-psk-helpers.h
│   │   ├── crypto-tls-x509-helpers.c
│   │   ├── crypto-tls-x509-helpers.h
│   │   ├── io-channel-helpers.c
│   │   ├── io-channel-helpers.h
│   │   ├── iothread.c
│   │   ├── iothread.h
│   │   ├── meson.build
│   │   ├── pkix_asn1_tab.c.inc
│   │   ├── ptimer-test-stubs.c
│   │   ├── ptimer-test.c
│   │   ├── ptimer-test.h
│   │   ├── rcutorture.c
│   │   ├── socket-helpers.c
│   │   ├── socket-helpers.h
│   │   ├── test-aio-multithread.c
│   │   ├── test-aio.c
│   │   ├── test-authz-list.c
│   │   ├── test-authz-listfile.c
│   │   ├── test-authz-pam.c
│   │   ├── test-authz-simple.c
│   │   ├── test-base64.c
│   │   ├── test-bdrv-drain.c
│   │   ├── test-bdrv-graph-mod.c
│   │   ├── test-bitcnt.c
│   │   ├── test-bitmap.c
│   │   ├── test-bitops.c
│   │   ├── test-block-backend.c
│   │   ├── test-block-iothread.c
│   │   ├── test-blockjob-txn.c
│   │   ├── test-blockjob.c
│   │   ├── test-bufferiszero.c
│   │   ├── test-char.c
│   │   ├── test-clone-visitor.c
│   │   ├── test-coroutine.c
│   │   ├── test-crypto-afsplit.c
│   │   ├── test-crypto-akcipher.c
│   │   ├── test-crypto-block.c
│   │   ├── test-crypto-cipher.c
│   │   ├── test-crypto-der.c
│   │   ├── test-crypto-hash.c
│   │   ├── test-crypto-hmac.c
│   │   ├── test-crypto-ivgen.c
│   │   ├── test-crypto-pbkdf.c
│   │   ├── test-crypto-secret.c
│   │   ├── test-crypto-tlscredsx509.c
│   │   ├── test-crypto-tlssession.c
│   │   ├── test-crypto-xts.c
│   │   ├── test-cutils.c
│   │   ├── test-div128.c
│   │   ├── test-error-report.c
│   │   ├── test-fifo.c
│   │   ├── test-forward-visitor.c
│   │   ├── test-hbitmap.c
│   │   ├── test-image-locking.c
│   │   ├── test-int128.c
│   │   ├── test-interval-tree.c
│   │   ├── test-io-channel-buffer.c
│   │   ├── test-io-channel-command.c
│   │   ├── test-io-channel-file.c
│   │   ├── test-io-channel-null.c
│   │   ├── test-io-channel-socket.c
│   │   ├── test-io-channel-tls.c
│   │   ├── test-io-task.c
│   │   ├── test-iov.c
│   │   ├── test-keyval.c
│   │   ├── test-logging.c
│   │   ├── test-mul64.c
│   │   ├── test-nested-aio-poll.c
│   │   ├── test-opts-visitor.c
│   │   ├── test-qapi-util.c
│   │   ├── test-qdev-global-props.c
│   │   ├── test-qdist.c
│   │   ├── test-qemu-opts.c
│   │   ├── test-qga.c
│   │   ├── test-qgraph.c
│   │   ├── test-qht.c
│   │   ├── test-qmp-cmds.c
│   │   ├── test-qmp-event.c
│   │   ├── test-qobject-input-visitor.c
│   │   ├── test-qobject-output-visitor.c
│   │   ├── test-qtree.c
│   │   ├── test-rcu-list.c
│   │   ├── test-rcu-simpleq.c
│   │   ├── test-rcu-slist.c
│   │   ├── test-rcu-tailq.c
│   │   ├── test-replication.c
│   │   ├── test-resv-mem.c
│   │   ├── test-seccomp.c
│   │   ├── test-shift128.c
│   │   ├── test-smp-parse.c
│   │   ├── test-string-input-visitor.c
│   │   ├── test-string-output-visitor.c
│   │   ├── test-thread-pool.c
│   │   ├── test-throttle.c
│   │   ├── test-timed-average.c
│   │   ├── test-util-filemonitor.c
│   │   ├── test-util-sockets.c
│   │   ├── test-uuid.c
│   │   ├── test-virtio-dmabuf.c
│   │   ├── test-visitor-serialization.c
│   │   ├── test-vmstate.c
│   │   ├── test-write-threshold.c
│   │   ├── test-x86-topo.c
│   │   ├── test-xbzrle.c
│   │   ├── test-xs-node.c
│   │   └── test-yank.c
│   ├── vhost-user-bridge.c
│   ├── vm
│   │   ├── aarch64vm.py
│   │   ├── basevm.py
│   │   ├── centos-8-aarch64.ks
│   │   ├── centos.aarch64
│   │   ├── conf_example_aarch64.yml
│   │   ├── conf_example_x86.yml
│   │   ├── freebsd
│   │   ├── generated
│   │   │   ├── freebsd.json
│   │   │   └── README
│   │   ├── haiku.x86_64
│   │   ├── Makefile.include
│   │   ├── netbsd
│   │   ├── openbsd
│   │   ├── README
│   │   ├── ubuntu.aarch64
│   │   └── ubuntuvm.py
│   └── vmstate-static-checker-data
│       ├── dump1.json
│       └── dump2.json
├── tools
│   ├── ebpf
│   │   ├── Makefile.ebpf
│   │   └── rss.bpf.c
│   ├── i386
│   │   ├── qemu-vmsr-helper.c
│   │   └── rapl-msr-index.h
│   └── meson.build
├── trace
│   ├── control-internal.h
│   ├── control-target.c
│   ├── control.c
│   ├── control.h
│   ├── event-internal.h
│   ├── ftrace.c
│   ├── ftrace.h
│   ├── meson.build
│   ├── qmp.c
│   ├── simple.c
│   ├── simple.h
│   └── trace-hmp-cmds.c
├── trace-events
├── ui
│   ├── clipboard.c
│   ├── cocoa.m
│   ├── console-gl.c
│   ├── console-priv.h
│   ├── console-vc-stubs.c
│   ├── console-vc.c
│   ├── console.c
│   ├── curses_keys.h
│   ├── curses.c
│   ├── cursor_hidden.xpm
│   ├── cursor_left_ptr.xpm
│   ├── cursor.c
│   ├── dbus-chardev.c
│   ├── dbus-clipboard.c
│   ├── dbus-console.c
│   ├── dbus-display1.xml
│   ├── dbus-error.c
│   ├── dbus-listener.c
│   ├── dbus-module.c
│   ├── dbus.c
│   ├── dbus.h
│   ├── dmabuf.c
│   ├── egl-context.c
│   ├── egl-headless.c
│   ├── egl-helpers.c
│   ├── gtk-clipboard.c
│   ├── gtk-egl.c
│   ├── gtk-gl-area.c
│   ├── gtk.c
│   ├── icons
│   │   ├── Makefile
│   │   ├── meson.build
│   │   ├── qemu_128x128.png
│   │   ├── qemu_16x16.png
│   │   ├── qemu_24x24.png
│   │   ├── qemu_256x256.png
│   │   ├── qemu_32x32.bmp
│   │   ├── qemu_32x32.png
│   │   ├── qemu_48x48.png
│   │   ├── qemu_512x512.png
│   │   ├── qemu_64x64.png
│   │   └── qemu.svg
│   ├── input-barrier.c
│   ├── input-barrier.h
│   ├── input-keymap.c
│   ├── input-legacy.c
│   ├── input-linux.c
│   ├── input.c
│   ├── kbd-state.c
│   ├── keymaps.c
│   ├── keymaps.h
│   ├── meson.build
│   ├── qemu-pixman.c
│   ├── qemu-x509.h
│   ├── qemu.desktop
│   ├── sdl2-2d.c
│   ├── sdl2-gl.c
│   ├── sdl2-input.c
│   ├── sdl2.c
│   ├── shader
│   │   ├── meson.build
│   │   ├── texture-blit-flip.vert
│   │   ├── texture-blit.frag
│   │   └── texture-blit.vert
│   ├── shader.c
│   ├── spice-app.c
│   ├── spice-core.c
│   ├── spice-display.c
│   ├── spice-input.c
│   ├── spice-module.c
│   ├── trace-events
│   ├── trace.h
│   ├── udmabuf.c
│   ├── ui-hmp-cmds.c
│   ├── ui-qmp-cmds.c
│   ├── util.c
│   ├── vdagent.c
│   ├── vgafont.h
│   ├── vnc_keysym.h
│   ├── vnc-auth-sasl.c
│   ├── vnc-auth-sasl.h
│   ├── vnc-auth-vencrypt.c
│   ├── vnc-auth-vencrypt.h
│   ├── vnc-clipboard.c
│   ├── vnc-enc-hextile-template.h
│   ├── vnc-enc-hextile.c
│   ├── vnc-enc-tight.c
│   ├── vnc-enc-tight.h
│   ├── vnc-enc-zlib.c
│   ├── vnc-enc-zrle.c
│   ├── vnc-enc-zrle.c.inc
│   ├── vnc-enc-zrle.h
│   ├── vnc-enc-zywrle-template.c
│   ├── vnc-enc-zywrle.h
│   ├── vnc-jobs.c
│   ├── vnc-jobs.h
│   ├── vnc-palette.c
│   ├── vnc-palette.h
│   ├── vnc-stubs.c
│   ├── vnc-ws.c
│   ├── vnc-ws.h
│   ├── vnc.c
│   ├── vnc.h
│   ├── win32-kbd-hook.c
│   ├── x_keymap.c
│   └── x_keymap.h
├── util
│   ├── aio-posix.c
│   ├── aio-posix.h
│   ├── aio-wait.c
│   ├── aio-win32.c
│   ├── aiocb.c
│   ├── async.c
│   ├── atomic64.c
│   ├── base64.c
│   ├── bitmap.c
│   ├── bitops.c
│   ├── block-helpers.c
│   ├── block-helpers.h
│   ├── buffer.c
│   ├── bufferiszero.c
│   ├── cacheflush.c
│   ├── chardev_open.c
│   ├── compatfd.c
│   ├── coroutine-sigaltstack.c
│   ├── coroutine-ucontext.c
│   ├── coroutine-wasm.c
│   ├── coroutine-windows.c
│   ├── cpuinfo-aarch64.c
│   ├── cpuinfo-i386.c
│   ├── cpuinfo-loongarch.c
│   ├── cpuinfo-ppc.c
│   ├── cpuinfo-riscv.c
│   ├── crc-ccitt.c
│   ├── crc32c.c
│   ├── cutils.c
│   ├── dbus.c
│   ├── defer-call.c
│   ├── drm.c
│   ├── envlist.c
│   ├── error-report.c
│   ├── error.c
│   ├── event_notifier-posix.c
│   ├── event_notifier-win32.c
│   ├── event.c
│   ├── fdmon-epoll.c
│   ├── fdmon-io_uring.c
│   ├── fdmon-poll.c
│   ├── fifo8.c
│   ├── filemonitor-inotify.c
│   ├── filemonitor-stub.c
│   ├── getauxval.c
│   ├── guest-random.c
│   ├── hbitmap.c
│   ├── hexdump.c
│   ├── host-utils.c
│   ├── id.c
│   ├── int128.c
│   ├── interval-tree.c
│   ├── iov.c
│   ├── iova-tree.c
│   ├── keyval.c
│   ├── lockcnt.c
│   ├── log.c
│   ├── main-loop.c
│   ├── memalign.c
│   ├── memfd.c
│   ├── meson.build
│   ├── mmap-alloc.c
│   ├── module.c
│   ├── notify.c
│   ├── nvdimm-utils.c
│   ├── osdep.c
│   ├── oslib-posix.c
│   ├── oslib-win32.c
│   ├── path.c
│   ├── qdist.c
│   ├── qemu-co-shared-resource.c
│   ├── qemu-co-timeout.c
│   ├── qemu-config.c
│   ├── qemu-coroutine-io.c
│   ├── qemu-coroutine-lock.c
│   ├── qemu-coroutine-sleep.c
│   ├── qemu-coroutine.c
│   ├── qemu-option.c
│   ├── qemu-print.c
│   ├── qemu-progress.c
│   ├── qemu-sockets.c
│   ├── qemu-thread-common.h
│   ├── qemu-thread-posix.c
│   ├── qemu-thread-win32.c
│   ├── qemu-timer-common.c
│   ├── qemu-timer.c
│   ├── qht.c
│   ├── qsp.c
│   ├── qtree.c
│   ├── range.c
│   ├── rcu.c
│   ├── readline.c
│   ├── reserved-region.c
│   ├── s390x_pci_mmio.c
│   ├── selfmap.c
│   ├── stats64.c
│   ├── sys_membarrier.c
│   ├── systemd.c
│   ├── thread-context.c
│   ├── thread-pool.c
│   ├── throttle.c
│   ├── timed-average.c
│   ├── trace-events
│   ├── trace.h
│   ├── transactions.c
│   ├── unicode.c
│   ├── userfaultfd.c
│   ├── uuid.c
│   ├── vfio-helpers.c
│   ├── vhost-user-server.c
│   └── yank.c
├── VERSION
└── version.rc

700 directories, 10465 files
