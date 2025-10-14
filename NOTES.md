.
├── a.out.h
├── acl.c
├── acl.h
├── aes.c
├── aes.h
├── aio.c
├── alpha-dis.c
├── alpha.ld
├── arch_init.c
├── arch_init.h
├── arm-dis.c
├── arm-semi.c
├── arm.ld
├── async.c
├── audio
│   ├── alsaaudio.c
│   ├── audio_int.h
│   ├── audio_pt_int.c
│   ├── audio_pt_int.h
│   ├── audio_template.h
│   ├── audio_win_int.c
│   ├── audio_win_int.h
│   ├── audio.c
│   ├── audio.h
│   ├── coreaudio.c
│   ├── dsound_template.h
│   ├── dsoundaudio.c
│   ├── esdaudio.c
│   ├── fmodaudio.c
│   ├── mixeng_template.h
│   ├── mixeng.c
│   ├── mixeng.h
│   ├── noaudio.c
│   ├── ossaudio.c
│   ├── paaudio.c
│   ├── rate_template.h
│   ├── sdlaudio.c
│   ├── spiceaudio.c
│   ├── wavaudio.c
│   ├── wavcapture.c
│   └── winwaveaudio.c
├── balloon.c
├── balloon.h
├── bitmap.c
├── bitmap.h
├── bitops.c
├── bitops.h
├── block
│   ├── blkdebug.c
│   ├── blkverify.c
│   ├── bochs.c
│   ├── cloop.c
│   ├── cow.c
│   ├── curl.c
│   ├── dmg.c
│   ├── iscsi.c
│   ├── nbd.c
│   ├── parallels.c
│   ├── qcow.c
│   ├── qcow2-cache.c
│   ├── qcow2-cluster.c
│   ├── qcow2-refcount.c
│   ├── qcow2-snapshot.c
│   ├── qcow2.c
│   ├── qcow2.h
│   ├── qed-check.c
│   ├── qed-cluster.c
│   ├── qed-gencb.c
│   ├── qed-l2-cache.c
│   ├── qed-table.c
│   ├── qed.c
│   ├── qed.h
│   ├── raw-posix-aio.h
│   ├── raw-posix.c
│   ├── raw-win32.c
│   ├── raw.c
│   ├── rbd.c
│   ├── sheepdog.c
│   ├── vdi.c
│   ├── vmdk.c
│   ├── vpc.c
│   └── vvfat.c
├── block_int.h
├── block-migration.c
├── block-migration.h
├── block.c
├── block.h
├── blockdev.c
├── blockdev.h
├── bsd-user
│   ├── bsd-mman.h
│   ├── bsdload.c
│   ├── elfload.c
│   ├── errno_defs.h
│   ├── freebsd
│   │   ├── strace.list
│   │   └── syscall_nr.h
│   ├── i386
│   │   ├── syscall.h
│   │   └── target_signal.h
│   ├── main.c
│   ├── mmap.c
│   ├── netbsd
│   │   ├── strace.list
│   │   └── syscall_nr.h
│   ├── openbsd
│   │   ├── strace.list
│   │   └── syscall_nr.h
│   ├── qemu-types.h
│   ├── qemu.h
│   ├── signal.c
│   ├── sparc
│   │   ├── syscall.h
│   │   └── target_signal.h
│   ├── sparc64
│   │   ├── syscall.h
│   │   └── target_signal.h
│   ├── strace.c
│   ├── syscall_defs.h
│   ├── syscall.c
│   ├── uaccess.c
│   └── x86_64
│       ├── syscall.h
│       └── target_signal.h
├── bswap.h
├── bt-host.c
├── bt-host.h
├── bt-vhci.c
├── buffered_file.c
├── buffered_file.h
├── cache-utils.c
├── cache-utils.h
├── Changelog
├── check-qdict.c
├── check-qfloat.c
├── check-qint.c
├── check-qjson.c
├── check-qlist.c
├── check-qstring.c
├── cmd.c
├── cmd.h
├── CODING_STYLE
├── compatfd.c
├── compatfd.h
├── compiler.h
├── config.h
├── configure
├── console.c
├── console.h
├── COPYING
├── COPYING.LIB
├── coroutine-gthread.c
├── coroutine-ucontext.c
├── coroutine-win32.c
├── cpu-all.h
├── cpu-common.h
├── cpu-defs.h
├── cpu-exec.c
├── cpus.c
├── cpus.h
├── cris-dis.c
├── cursor_hidden.xpm
├── cursor_left_ptr.xpm
├── cursor.c
├── cutils.c
├── darwin-user
│   ├── commpage.c
│   ├── ioctls_types.h
│   ├── ioctls.h
│   ├── machload.c
│   ├── main.c
│   ├── mmap.c
│   ├── qemu.h
│   ├── signal.c
│   ├── syscall.c
│   └── syscalls.h
├── def-helper.h
├── default-configs
│   ├── alpha-linux-user.mak
│   ├── alpha-softmmu.mak
│   ├── arm-linux-user.mak
│   ├── arm-softmmu.mak
│   ├── armeb-linux-user.mak
│   ├── cris-linux-user.mak
│   ├── cris-softmmu.mak
│   ├── i386-bsd-user.mak
│   ├── i386-darwin-user.mak
│   ├── i386-linux-user.mak
│   ├── i386-softmmu.mak
│   ├── lm32-softmmu.mak
│   ├── m68k-linux-user.mak
│   ├── m68k-softmmu.mak
│   ├── microblaze-linux-user.mak
│   ├── microblaze-softmmu.mak
│   ├── microblazeel-linux-user.mak
│   ├── microblazeel-softmmu.mak
│   ├── mips-linux-user.mak
│   ├── mips-softmmu.mak
│   ├── mips64-softmmu.mak
│   ├── mips64el-softmmu.mak
│   ├── mipsel-linux-user.mak
│   ├── mipsel-softmmu.mak
│   ├── pci.mak
│   ├── ppc-darwin-user.mak
│   ├── ppc-linux-user.mak
│   ├── ppc-softmmu.mak
│   ├── ppc64-linux-user.mak
│   ├── ppc64-softmmu.mak
│   ├── ppc64abi32-linux-user.mak
│   ├── ppcemb-softmmu.mak
│   ├── s390x-linux-user.mak
│   ├── s390x-softmmu.mak
│   ├── sh4-linux-user.mak
│   ├── sh4-softmmu.mak
│   ├── sh4eb-linux-user.mak
│   ├── sh4eb-softmmu.mak
│   ├── sparc-bsd-user.mak
│   ├── sparc-linux-user.mak
│   ├── sparc-softmmu.mak
│   ├── sparc32plus-linux-user.mak
│   ├── sparc64-bsd-user.mak
│   ├── sparc64-linux-user.mak
│   ├── sparc64-softmmu.mak
│   ├── unicore32-linux-user.mak
│   ├── x86_64-bsd-user.mak
│   ├── x86_64-linux-user.mak
│   ├── x86_64-softmmu.mak
│   ├── xtensa-softmmu.mak
│   └── xtensaeb-softmmu.mak
├── device_tree.c
├── device_tree.h
├── dis-asm.h
├── disas.c
├── disas.h
├── dma-helpers.c
├── dma.h
├── docs
│   ├── blkverify.txt
│   ├── bootindex.txt
│   ├── ccid.txt
│   ├── ich9-ehci-uhci.cfg
│   ├── libcacard.txt
│   ├── memory.txt
│   ├── migration.txt
│   ├── qapi-code-gen.txt
│   ├── qdev-device-use.txt
│   ├── specs
│   │   ├── acpi_pci_hotplug.txt
│   │   ├── ivshmem_device_spec.txt
│   │   ├── qcow2.txt
│   │   └── qed_spec.txt
│   ├── tracing.txt
│   └── usb2.txt
├── dyngen-exec.h
├── elf.h
├── envlist.c
├── envlist.h
├── error_int.h
├── error.c
├── error.h
├── event_notifier.c
├── event_notifier.h
├── exec-all.h
├── exec-memory.h
├── exec.c
├── fpu
│   ├── softfloat-macros.h
│   ├── softfloat-specialize.h
│   ├── softfloat.c
│   └── softfloat.h
├── fsdev
│   ├── file-op-9p.h
│   ├── qemu-fsdev-dummy.c
│   ├── qemu-fsdev.c
│   └── qemu-fsdev.h
├── gdb-xml
│   ├── arm-core.xml
│   ├── arm-neon.xml
│   ├── arm-vfp.xml
│   ├── arm-vfp3.xml
│   ├── cf-core.xml
│   ├── cf-fp.xml
│   ├── power-altivec.xml
│   ├── power-core.xml
│   ├── power-fpu.xml
│   ├── power-spe.xml
│   └── power64-core.xml
├── gdbstub.c
├── gdbstub.h
├── gen-icount.h
├── HACKING
├── hmp-commands.hx
├── hmp.c
├── hmp.h
├── host-utils.c
├── host-utils.h
├── hppa-dis.c
├── hppa.ld
├── hw
│   ├── 9p.h
│   ├── 9pfs
│   │   ├── codir.c
│   │   ├── cofile.c
│   │   ├── cofs.c
│   │   ├── coxattr.c
│   │   ├── virtio-9p-coth.c
│   │   ├── virtio-9p-coth.h
│   │   ├── virtio-9p-device.c
│   │   ├── virtio-9p-handle.c
│   │   ├── virtio-9p-local.c
│   │   ├── virtio-9p-posix-acl.c
│   │   ├── virtio-9p-synth.c
│   │   ├── virtio-9p-synth.h
│   │   ├── virtio-9p-xattr-user.c
│   │   ├── virtio-9p-xattr.c
│   │   ├── virtio-9p-xattr.h
│   │   ├── virtio-9p.c
│   │   └── virtio-9p.h
│   ├── a9mpcore.c
│   ├── ac97.c
│   ├── acpi_piix4.c
│   ├── acpi.c
│   ├── acpi.h
│   ├── adb.c
│   ├── adb.h
│   ├── adlib.c
│   ├── ads7846.c
│   ├── alpha_dp264.c
│   ├── alpha_pci.c
│   ├── alpha_sys.h
│   ├── alpha_typhoon.c
│   ├── an5206.c
│   ├── apb_pci.c
│   ├── apb_pci.h
│   ├── apic.c
│   ├── apic.h
│   ├── apm.c
│   ├── apm.h
│   ├── applesmc.c
│   ├── arm_boot.c
│   ├── arm_gic.c
│   ├── arm_pic.c
│   ├── arm_sysctl.c
│   ├── arm_timer.c
│   ├── arm-misc.h
│   ├── arm11mpcore.c
│   ├── armv7m_nvic.c
│   ├── armv7m.c
│   ├── audiodev.h
│   ├── axis_dev88.c
│   ├── baum.c
│   ├── baum.h
│   ├── bitbang_i2c.c
│   ├── bitbang_i2c.h
│   ├── blizzard_template.h
│   ├── blizzard.c
│   ├── boards.h
│   ├── bonito.c
│   ├── bt-hci-csr.c
│   ├── bt-hci.c
│   ├── bt-hid.c
│   ├── bt-l2cap.c
│   ├── bt-sdp.c
│   ├── bt.c
│   ├── bt.h
│   ├── cbus.c
│   ├── ccid-card-emulated.c
│   ├── ccid-card-passthru.c
│   ├── ccid.h
│   ├── cdrom.c
│   ├── cirrus_vga_rop.h
│   ├── cirrus_vga_rop2.h
│   ├── cirrus_vga.c
│   ├── collie.c
│   ├── cris_pic_cpu.c
│   ├── cris-boot.c
│   ├── cris-boot.h
│   ├── cs4231.c
│   ├── cs4231a.c
│   ├── cuda.c
│   ├── debugcon.c
│   ├── dec_pci.c
│   ├── dec_pci.h
│   ├── device-hotplug.c
│   ├── devices.h
│   ├── dma.c
│   ├── dp8393x.c
│   ├── ds1225y.c
│   ├── ds1338.c
│   ├── dummy_m68k.c
│   ├── e1000_hw.h
│   ├── e1000.c
│   ├── ecc.c
│   ├── eccmemctl.c
│   ├── eepro100.c
│   ├── eeprom93xx.c
│   ├── eeprom93xx.h
│   ├── elf_ops.h
│   ├── empty_slot.c
│   ├── empty_slot.h
│   ├── es1370.c
│   ├── escc.c
│   ├── escc.h
│   ├── esp.c
│   ├── esp.h
│   ├── etraxfs_dma.c
│   ├── etraxfs_dma.h
│   ├── etraxfs_eth.c
│   ├── etraxfs_pic.c
│   ├── etraxfs_ser.c
│   ├── etraxfs_timer.c
│   ├── etraxfs.h
│   ├── fdc.c
│   ├── fdc.h
│   ├── firmware_abi.h
│   ├── flash.h
│   ├── fmopl.c
│   ├── fmopl.h
│   ├── framebuffer.c
│   ├── framebuffer.h
│   ├── fw_cfg.c
│   ├── fw_cfg.h
│   ├── g364fb.c
│   ├── grackle_pci.c
│   ├── grlib_apbuart.c
│   ├── grlib_gptimer.c
│   ├── grlib_irqmp.c
│   ├── grlib.h
│   ├── gt64xxx.c
│   ├── gumstix.c
│   ├── gus.c
│   ├── gusemu_hal.c
│   ├── gusemu_mixer.c
│   ├── gusemu.h
│   ├── gustate.h
│   ├── hda-audio.c
│   ├── heathrow_pic.c
│   ├── hid.c
│   ├── hid.h
│   ├── hpet_emul.h
│   ├── hpet.c
│   ├── hw.h
│   ├── i2c.c
│   ├── i2c.h
│   ├── i8254.c
│   ├── i8259.c
│   ├── ide
│   │   ├── ahci.c
│   │   ├── ahci.h
│   │   ├── atapi.c
│   │   ├── cmd646.c
│   │   ├── core.c
│   │   ├── ich.c
│   │   ├── internal.h
│   │   ├── isa.c
│   │   ├── macio.c
│   │   ├── microdrive.c
│   │   ├── mmio.c
│   │   ├── pci.c
│   │   ├── pci.h
│   │   ├── piix.c
│   │   ├── qdev.c
│   │   └── via.c
│   ├── ide.h
│   ├── integratorcp.c
│   ├── intel-hda-defs.h
│   ├── intel-hda.c
│   ├── intel-hda.h
│   ├── ioapic.c
│   ├── ioapic.h
│   ├── ioh3420.c
│   ├── ioh3420.h
│   ├── irq.c
│   ├── irq.h
│   ├── isa_mmio.c
│   ├── isa-bus.c
│   ├── isa.h
│   ├── ivshmem.c
│   ├── jazz_led.c
│   ├── kvmclock.c
│   ├── kvmclock.h
│   ├── lan9118.c
│   ├── lance.c
│   ├── leon3.c
│   ├── lm32_boards.c
│   ├── lm32_hwsetup.h
│   ├── lm32_juart.c
│   ├── lm32_juart.h
│   ├── lm32_pic.c
│   ├── lm32_pic.h
│   ├── lm32_sys.c
│   ├── lm32_timer.c
│   ├── lm32_uart.c
│   ├── lm32.h
│   ├── lm4549.c
│   ├── lm4549.h
│   ├── lm832x.c
│   ├── loader.c
│   ├── loader.h
│   ├── lsi53c895a.c
│   ├── m48t59.c
│   ├── mac_dbdma.c
│   ├── mac_dbdma.h
│   ├── mac_nvram.c
│   ├── macio.c
│   ├── mainstone.c
│   ├── marvell_88w8618_audio.c
│   ├── max111x.c
│   ├── max7310.c
│   ├── mc146818rtc.c
│   ├── mc146818rtc.h
│   ├── mcf_fec.c
│   ├── mcf_intc.c
│   ├── mcf_uart.c
│   ├── mcf.h
│   ├── mcf5206.c
│   ├── mcf5208.c
│   ├── microblaze_pic_cpu.c
│   ├── microblaze_pic_cpu.h
│   ├── milkymist-ac97.c
│   ├── milkymist-hpdmc.c
│   ├── milkymist-hw.h
│   ├── milkymist-memcard.c
│   ├── milkymist-minimac2.c
│   ├── milkymist-pfpu.c
│   ├── milkymist-softusb.c
│   ├── milkymist-sysctl.c
│   ├── milkymist-tmu2.c
│   ├── milkymist-uart.c
│   ├── milkymist-vgafb_template.h
│   ├── milkymist-vgafb.c
│   ├── milkymist.c
│   ├── mips_addr.c
│   ├── mips_cpudevs.h
│   ├── mips_fulong2e.c
│   ├── mips_int.c
│   ├── mips_jazz.c
│   ├── mips_malta.c
│   ├── mips_mipssim.c
│   ├── mips_r4k.c
│   ├── mips_timer.c
│   ├── mips-bios.h
│   ├── mips.h
│   ├── mipsnet.c
│   ├── mpc8544_guts.c
│   ├── mpcore.c
│   ├── msi.c
│   ├── msi.h
│   ├── msix.c
│   ├── msix.h
│   ├── msmouse.c
│   ├── msmouse.h
│   ├── mst_fpga.c
│   ├── multiboot.c
│   ├── multiboot.h
│   ├── musicpal.c
│   ├── nand.c
│   ├── ne2000-isa.c
│   ├── ne2000.c
│   ├── ne2000.h
│   ├── nseries.c
│   ├── nvram.h
│   ├── omap_clk.c
│   ├── omap_dma.c
│   ├── omap_dss.c
│   ├── omap_gpio.c
│   ├── omap_gpmc.c
│   ├── omap_gptimer.c
│   ├── omap_i2c.c
│   ├── omap_intc.c
│   ├── omap_l4.c
│   ├── omap_lcd_template.h
│   ├── omap_lcdc.c
│   ├── omap_mmc.c
│   ├── omap_sdrc.c
│   ├── omap_spi.c
│   ├── omap_sx1.c
│   ├── omap_synctimer.c
│   ├── omap_tap.c
│   ├── omap_uart.c
│   ├── omap.h
│   ├── omap1.c
│   ├── omap2.c
│   ├── onenand.c
│   ├── opencores_eth.c
│   ├── openpic.c
│   ├── openpic.h
│   ├── palm.c
│   ├── parallel.c
│   ├── pc_piix.c
│   ├── pc.c
│   ├── pc.h
│   ├── pci_bridge.c
│   ├── pci_bridge.h
│   ├── pci_host.c
│   ├── pci_host.h
│   ├── pci_ids.h
│   ├── pci_internals.h
│   ├── pci_regs.h
│   ├── pci-hotplug.c
│   ├── pci-stub.c
│   ├── pci.c
│   ├── pci.h
│   ├── pcie_aer.c
│   ├── pcie_aer.h
│   ├── pcie_host.c
│   ├── pcie_host.h
│   ├── pcie_port.c
│   ├── pcie_port.h
│   ├── pcie_regs.h
│   ├── pcie.c
│   ├── pcie.h
│   ├── pckbd.c
│   ├── pcmcia.h
│   ├── pcnet-pci.c
│   ├── pcnet.c
│   ├── pcnet.h
│   ├── pcspk.c
│   ├── petalogix_ml605_mmu.c
│   ├── petalogix_s3adsp1800_mmu.c
│   ├── pflash_cfi01.c
│   ├── pflash_cfi02.c
│   ├── piix_pci.c
│   ├── piix4.c
│   ├── pixel_ops.h
│   ├── pl011.c
│   ├── pl022.c
│   ├── pl031.c
│   ├── pl041.c
│   ├── pl041.h
│   ├── pl041.hx
│   ├── pl050.c
│   ├── pl061.c
│   ├── pl080.c
│   ├── pl110_template.h
│   ├── pl110.c
│   ├── pl181.c
│   ├── pl190.c
│   ├── pm_smbus.c
│   ├── pm_smbus.h
│   ├── ppc_booke.c
│   ├── ppc_mac.h
│   ├── ppc_newworld.c
│   ├── ppc_oldworld.c
│   ├── ppc_prep.c
│   ├── ppc-viosrp.h
│   ├── ppc.c
│   ├── ppc.h
│   ├── ppc405_boards.c
│   ├── ppc405_uc.c
│   ├── ppc405.h
│   ├── ppc440_bamboo.c
│   ├── ppc440.c
│   ├── ppc440.h
│   ├── ppc4xx_devs.c
│   ├── ppc4xx_pci.c
│   ├── ppc4xx.h
│   ├── ppce500_mpc8544ds.c
│   ├── ppce500_pci.c
│   ├── ppce500_spin.c
│   ├── prep_pci.c
│   ├── prep_pci.h
│   ├── primecell.h
│   ├── ps2.c
│   ├── ps2.h
│   ├── ptimer.c
│   ├── pxa.h
│   ├── pxa2xx_dma.c
│   ├── pxa2xx_gpio.c
│   ├── pxa2xx_keypad.c
│   ├── pxa2xx_lcd.c
│   ├── pxa2xx_mmci.c
│   ├── pxa2xx_pcmcia.c
│   ├── pxa2xx_pic.c
│   ├── pxa2xx_template.h
│   ├── pxa2xx_timer.c
│   ├── pxa2xx.c
│   ├── qdev-addr.c
│   ├── qdev-addr.h
│   ├── qdev-properties.c
│   ├── qdev.c
│   ├── qdev.h
│   ├── qxl-logger.c
│   ├── qxl-render.c
│   ├── qxl.c
│   ├── qxl.h
│   ├── r2d.c
│   ├── rc4030.c
│   ├── realview_gic.c
│   ├── realview.c
│   ├── rtl8139.c
│   ├── s390-virtio-bus.c
│   ├── s390-virtio-bus.h
│   ├── s390-virtio.c
│   ├── sb16.c
│   ├── sbi.c
│   ├── scsi-bus.c
│   ├── scsi-defs.h
│   ├── scsi-disk.c
│   ├── scsi-generic.c
│   ├── scsi.h
│   ├── sd.c
│   ├── sd.h
│   ├── serial.c
│   ├── sga.c
│   ├── sh_intc.c
│   ├── sh_intc.h
│   ├── sh_pci.c
│   ├── sh_serial.c
│   ├── sh_timer.c
│   ├── sh.h
│   ├── sh7750_regnames.c
│   ├── sh7750_regnames.h
│   ├── sh7750_regs.h
│   ├── sh7750.c
│   ├── sharpsl.h
│   ├── shix.c
│   ├── slavio_intctl.c
│   ├── slavio_misc.c
│   ├── slavio_timer.c
│   ├── sm501_template.h
│   ├── sm501.c
│   ├── smbios.c
│   ├── smbios.h
│   ├── smbus_eeprom.c
│   ├── smbus.c
│   ├── smbus.h
│   ├── smc91c111.c
│   ├── soc_dma.c
│   ├── soc_dma.h
│   ├── spapr_hcall.c
│   ├── spapr_llan.c
│   ├── spapr_pci.c
│   ├── spapr_pci.h
│   ├── spapr_rtas.c
│   ├── spapr_vio.c
│   ├── spapr_vio.h
│   ├── spapr_vscsi.c
│   ├── spapr_vty.c
│   ├── spapr.c
│   ├── spapr.h
│   ├── sparc32_dma.c
│   ├── sparc32_dma.h
│   ├── spitz.c
│   ├── srp.h
│   ├── ssd0303.c
│   ├── ssd0323.c
│   ├── ssi-sd.c
│   ├── ssi.c
│   ├── ssi.h
│   ├── stellaris_enet.c
│   ├── stellaris_input.c
│   ├── stellaris.c
│   ├── strongarm.c
│   ├── strongarm.h
│   ├── sun4c_intctl.c
│   ├── sun4m_iommu.c
│   ├── sun4m.c
│   ├── sun4m.h
│   ├── sun4u.c
│   ├── syborg_fb.c
│   ├── syborg_interrupt.c
│   ├── syborg_keyboard.c
│   ├── syborg_pointer.c
│   ├── syborg_rtc.c
│   ├── syborg_serial.c
│   ├── syborg_timer.c
│   ├── syborg_virtio.c
│   ├── syborg.c
│   ├── syborg.h
│   ├── sysbus.c
│   ├── sysbus.h
│   ├── tc58128.c
│   ├── tc6393xb_template.h
│   ├── tc6393xb.c
│   ├── tcx.c
│   ├── tmp105.c
│   ├── tosa.c
│   ├── tsc2005.c
│   ├── tsc210x.c
│   ├── tusb6010.c
│   ├── twl92230.c
│   ├── unin_pci.c
│   ├── usb-bt.c
│   ├── usb-bus.c
│   ├── usb-ccid.c
│   ├── usb-desc.c
│   ├── usb-desc.h
│   ├── usb-ehci.c
│   ├── usb-hid.c
│   ├── usb-hub.c
│   ├── usb-libhw.c
│   ├── usb-msd.c
│   ├── usb-musb.c
│   ├── usb-net.c
│   ├── usb-ohci.c
│   ├── usb-ohci.h
│   ├── usb-serial.c
│   ├── usb-uhci.c
│   ├── usb-uhci.h
│   ├── usb-wacom.c
│   ├── usb.c
│   ├── usb.h
│   ├── versatile_pci.c
│   ├── versatilepb.c
│   ├── vexpress.c
│   ├── vga_int.h
│   ├── vga_template.h
│   ├── vga-isa-mm.c
│   ├── vga-isa.c
│   ├── vga-pci.c
│   ├── vga.c
│   ├── vhost_net.c
│   ├── vhost_net.h
│   ├── vhost.c
│   ├── vhost.h
│   ├── virtex_ml507.c
│   ├── virtio-balloon.c
│   ├── virtio-balloon.h
│   ├── virtio-blk.c
│   ├── virtio-blk.h
│   ├── virtio-console.c
│   ├── virtio-net.c
│   ├── virtio-net.h
│   ├── virtio-pci.c
│   ├── virtio-pci.h
│   ├── virtio-serial-bus.c
│   ├── virtio-serial.h
│   ├── virtio.c
│   ├── virtio.h
│   ├── vmmouse.c
│   ├── vmport.c
│   ├── vmware_vga.c
│   ├── vmware_vga.h
│   ├── vt82c686.c
│   ├── vt82c686.h
│   ├── watchdog.c
│   ├── watchdog.h
│   ├── wdt_i6300esb.c
│   ├── wdt_ib700.c
│   ├── wm8750.c
│   ├── xen_backend.c
│   ├── xen_backend.h
│   ├── xen_blkif.h
│   ├── xen_common.h
│   ├── xen_console.c
│   ├── xen_devconfig.c
│   ├── xen_disk.c
│   ├── xen_domainbuild.c
│   ├── xen_domainbuild.h
│   ├── xen_machine_pv.c
│   ├── xen_nic.c
│   ├── xen_platform.c
│   ├── xen.h
│   ├── xenfb.c
│   ├── xics.c
│   ├── xics.h
│   ├── xilinx_axidma.c
│   ├── xilinx_axidma.h
│   ├── xilinx_axienet.c
│   ├── xilinx_ethlite.c
│   ├── xilinx_intc.c
│   ├── xilinx_timer.c
│   ├── xilinx_uartlite.c
│   ├── xilinx.h
│   ├── xio3130_downstream.c
│   ├── xio3130_downstream.h
│   ├── xio3130_upstream.c
│   ├── xio3130_upstream.h
│   ├── xtensa_bootparam.h
│   ├── xtensa_lx60.c
│   ├── xtensa_pic.c
│   ├── xtensa_sim.c
│   ├── z2.c
│   └── zaurus.c
├── i386-dis.c
├── i386.ld
├── ia64-dis.c
├── ia64.ld
├── input.c
├── int128.h
├── iohandler.c
├── ioport-user.c
├── ioport.c
├── ioport.h
├── iorange.h
├── iov.c
├── iov.h
├── json-lexer.c
├── json-lexer.h
├── json-parser.c
├── json-parser.h
├── json-streamer.c
├── json-streamer.h
├── kvm-all.c
├── kvm-stub.c
├── kvm.h
├── libcacard
│   ├── cac.c
│   ├── cac.h
│   ├── card_7816.c
│   ├── card_7816.h
│   ├── card_7816t.h
│   ├── event.c
│   ├── eventt.h
│   ├── libcacard.pc.in
│   ├── link_test.c
│   ├── Makefile
│   ├── vcard_emul_nss.c
│   ├── vcard_emul_type.c
│   ├── vcard_emul_type.h
│   ├── vcard_emul.h
│   ├── vcard.c
│   ├── vcard.h
│   ├── vcardt.h
│   ├── vevent.h
│   ├── vreader.c
│   ├── vreader.h
│   ├── vreadert.h
│   ├── vscard_common.h
│   └── vscclient.c
├── libfdt_env.h
├── LICENSE
├── linux-aio.c
├── linux-headers
│   ├── asm-powerpc
│   │   ├── kvm_para.h
│   │   └── kvm.h
│   ├── asm-s390
│   │   ├── kvm_para.h
│   │   └── kvm.h
│   ├── asm-x86
│   │   ├── hyperv.h
│   │   ├── kvm_para.h
│   │   └── kvm.h
│   ├── COPYING
│   ├── linux
│   │   ├── kvm_para.h
│   │   ├── kvm.h
│   │   ├── vhost.h
│   │   ├── virtio_config.h
│   │   └── virtio_ring.h
│   └── README
├── linux-user
│   ├── alpha
│   │   ├── syscall_nr.h
│   │   ├── syscall.h
│   │   ├── target_signal.h
│   │   └── termbits.h
│   ├── arm
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
│   │   │   └── single_cpdo.c
│   │   ├── syscall_nr.h
│   │   ├── syscall.h
│   │   ├── target_signal.h
│   │   └── termbits.h
│   ├── cpu-uname.c
│   ├── cpu-uname.h
│   ├── cris
│   │   ├── syscall_nr.h
│   │   ├── syscall.h
│   │   ├── target_signal.h
│   │   └── termbits.h
│   ├── elfload.c
│   ├── errno_defs.h
│   ├── flat.h
│   ├── flatload.c
│   ├── i386
│   │   ├── syscall_nr.h
│   │   ├── syscall.h
│   │   ├── target_signal.h
│   │   └── termbits.h
│   ├── ioctls.h
│   ├── linux_loop.h
│   ├── linuxload.c
│   ├── m68k
│   │   ├── syscall_nr.h
│   │   ├── syscall.h
│   │   ├── target_signal.h
│   │   └── termbits.h
│   ├── m68k-sim.c
│   ├── main.c
│   ├── microblaze
│   │   ├── syscall_nr.h
│   │   ├── syscall.h
│   │   ├── target_signal.h
│   │   └── termbits.h
│   ├── mips
│   │   ├── syscall_nr.h
│   │   ├── syscall.h
│   │   ├── target_signal.h
│   │   └── termbits.h
│   ├── mips64
│   │   ├── syscall_nr.h
│   │   ├── syscall.h
│   │   ├── target_signal.h
│   │   └── termbits.h
│   ├── mipsn32
│   │   ├── syscall_nr.h
│   │   ├── syscall.h
│   │   ├── target_signal.h
│   │   └── termbits.h
│   ├── mmap.c
│   ├── ppc
│   │   ├── syscall_nr.h
│   │   ├── syscall.h
│   │   ├── target_signal.h
│   │   └── termbits.h
│   ├── qemu-types.h
│   ├── qemu.h
│   ├── s390x
│   │   ├── syscall_nr.h
│   │   ├── syscall.h
│   │   ├── target_signal.h
│   │   └── termbits.h
│   ├── sh4
│   │   ├── syscall_nr.h
│   │   ├── syscall.h
│   │   ├── target_signal.h
│   │   └── termbits.h
│   ├── signal.c
│   ├── socket.h
│   ├── sparc
│   │   ├── syscall_nr.h
│   │   ├── syscall.h
│   │   ├── target_signal.h
│   │   └── termbits.h
│   ├── sparc64
│   │   ├── syscall_nr.h
│   │   ├── syscall.h
│   │   ├── target_signal.h
│   │   └── termbits.h
│   ├── strace.c
│   ├── strace.list
│   ├── syscall_defs.h
│   ├── syscall_types.h
│   ├── syscall.c
│   ├── target_flat.h
│   ├── uaccess.c
│   ├── unicore32
│   │   ├── syscall_nr.h
│   │   ├── syscall.h
│   │   ├── target_signal.h
│   │   └── termbits.h
│   ├── vm86.c
│   └── x86_64
│       ├── syscall_nr.h
│       ├── syscall.h
│       ├── target_signal.h
│       └── termbits.h
├── m68k-dis.c
├── m68k-semi.c
├── m68k.ld
├── main-loop.c
├── main-loop.h
├── MAINTAINERS
├── Makefile
├── Makefile.dis
├── Makefile.hw
├── Makefile.objs
├── Makefile.target
├── Makefile.user
├── memory.c
├── memory.h
├── microblaze-dis.c
├── migration-exec.c
├── migration-fd.c
├── migration-tcp.c
├── migration-unix.c
├── migration.c
├── migration.h
├── mips-dis.c
├── mips.ld
├── module.c
├── module.h
├── monitor.c
├── monitor.h
├── nbd.c
├── nbd.h
├── net
│   ├── checksum.c
│   ├── checksum.h
│   ├── dump.c
│   ├── dump.h
│   ├── queue.c
│   ├── queue.h
│   ├── slirp.c
│   ├── slirp.h
│   ├── socket.c
│   ├── socket.h
│   ├── tap-aix.c
│   ├── tap-bsd.c
│   ├── tap-haiku.c
│   ├── tap-linux.c
│   ├── tap-linux.h
│   ├── tap-solaris.c
│   ├── tap-win32.c
│   ├── tap.c
│   ├── tap.h
│   ├── util.c
│   ├── util.h
│   ├── vde.c
│   └── vde.h
├── net.c
├── net.h
├── NOTES.md
├── notify.c
├── notify.h
├── os-posix.c
├── os-win32.c
├── osdep.c
├── osdep.h
├── oslib-posix.c
├── oslib-win32.c
├── path.c
├── pc-bios
│   ├── bamboo.dtb
│   ├── bamboo.dts
│   ├── bios.bin
│   ├── keymaps
│   │   ├── ar
│   │   ├── bepo
│   │   ├── common
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
│   │   ├── mk
│   │   ├── modifiers
│   │   ├── nl
│   │   ├── nl-be
│   │   ├── no
│   │   ├── pl
│   │   ├── pt
│   │   ├── pt-br
│   │   ├── ru
│   │   ├── sl
│   │   ├── sv
│   │   ├── th
│   │   └── tr
│   ├── linuxboot.bin
│   ├── Makefile
│   ├── mpc8544ds.dtb
│   ├── mpc8544ds.dts
│   ├── multiboot.bin
│   ├── ohw.diff
│   ├── openbios-ppc
│   ├── openbios-sparc32
│   ├── openbios-sparc64
│   ├── optionrom
│   │   ├── linuxboot.S
│   │   ├── Makefile
│   │   ├── multiboot.S
│   │   └── optionrom.h
│   ├── palcode-clipper
│   ├── petalogix-ml605.dtb
│   ├── petalogix-s3adsp1800.dtb
│   ├── ppc_rom.bin
│   ├── pxe-e1000.rom
│   ├── pxe-eepro100.rom
│   ├── pxe-ne2k_pci.rom
│   ├── pxe-pcnet.rom
│   ├── pxe-rtl8139.rom
│   ├── pxe-virtio.rom
│   ├── README
│   ├── s390-zipl.rom
│   ├── sgabios.bin
│   ├── slof.bin
│   ├── spapr-rtas
│   │   ├── Makefile
│   │   └── spapr-rtas.S
│   ├── spapr-rtas.bin
│   ├── vgabios-cirrus.bin
│   ├── vgabios-qxl.bin
│   ├── vgabios-stdvga.bin
│   ├── vgabios-vmware.bin
│   └── vgabios.bin
├── pci-ids.txt
├── pflib.c
├── pflib.h
├── poison.h
├── posix-aio-compat.c
├── ppc-dis.c
├── ppc.ld
├── ppc64.ld
├── qapi
│   ├── qapi-dealloc-visitor.c
│   ├── qapi-dealloc-visitor.h
│   ├── qapi-types-core.h
│   ├── qapi-visit-core.c
│   ├── qapi-visit-core.h
│   ├── qmp-core.h
│   ├── qmp-dispatch.c
│   ├── qmp-input-visitor.c
│   ├── qmp-input-visitor.h
│   ├── qmp-output-visitor.c
│   ├── qmp-output-visitor.h
│   └── qmp-registry.c
├── qapi-schema-guest.json
├── qapi-schema-test.json
├── qapi-schema.json
├── qbool.c
├── qbool.h
├── qdict-test-data.txt
├── qdict.c
├── qdict.h
├── qemu_socket.h
├── qemu-aio.h
├── qemu-barrier.h
├── qemu-char.c
├── qemu-char.h
├── qemu-common.h
├── qemu-config.c
├── qemu-config.h
├── qemu-coroutine-int.h
├── qemu-coroutine-lock.c
├── qemu-coroutine.c
├── qemu-coroutine.h
├── qemu-doc.texi
├── qemu-error.c
├── qemu-error.h
├── qemu-ga.c
├── qemu-img-cmds.hx
├── qemu-img.c
├── qemu-img.texi
├── qemu-io.c
├── qemu-lock.h
├── qemu-log.h
├── qemu-nbd.c
├── qemu-nbd.texi
├── qemu-objects.h
├── qemu-option.c
├── qemu-option.h
├── qemu-options.h
├── qemu-options.hx
├── qemu-os-posix.h
├── qemu-os-win32.h
├── qemu-progress.c
├── qemu-queue.h
├── qemu-sockets.c
├── qemu-tech.texi
├── qemu-thread-posix.c
├── qemu-thread-posix.h
├── qemu-thread-win32.c
├── qemu-thread-win32.h
├── qemu-thread.h
├── qemu-timer-common.c
├── qemu-timer.c
├── qemu-timer.h
├── qemu-tls.h
├── qemu-tool.c
├── qemu-x509.h
├── qemu-xattr.h
├── qemu.sasl
├── qerror.c
├── qerror.h
├── qfloat.c
├── qfloat.h
├── qga
│   ├── guest-agent-command-state.c
│   ├── guest-agent-commands.c
│   └── guest-agent-core.h
├── qint.c
├── qint.h
├── qjson.c
├── qjson.h
├── qlist.c
├── qlist.h
├── QMP
│   ├── qmp-events.txt
│   ├── qmp-shell
│   ├── qmp-spec.txt
│   ├── qmp.py
│   └── README
├── qmp-commands.hx
├── qmp.c
├── qobject.h
├── qstring.c
├── qstring.h
├── range.h
├── readline.c
├── readline.h
├── README
├── roms
│   ├── ipxe
│   ├── openbios
│   ├── qemu-palcode
│   ├── seabios
│   ├── sgabios
│   ├── SLOF
│   └── vgabios
├── rules.mak
├── s390-dis.c
├── s390.ld
├── savevm.c
├── scripts
│   ├── analyse-9p-simpletrace.py
│   ├── checkpatch.pl
│   ├── create_config
│   ├── feature_to_c.sh
│   ├── get_maintainer.pl
│   ├── hxtool
│   ├── kvm
│   │   ├── kvm_stat
│   │   └── vmxcap
│   ├── make_device_config.sh
│   ├── ordereddict.py
│   ├── qapi-commands.py
│   ├── qapi-types.py
│   ├── qapi-visit.py
│   ├── qapi.py
│   ├── qemu-binfmt-conf.sh
│   ├── refresh-pxe-roms.sh
│   ├── signrom.sh
│   ├── simpletrace.py
│   ├── texi2pod.pl
│   ├── tracetool
│   └── update-linux-headers.sh
├── sh4-dis.c
├── slirp
│   ├── arp_table.c
│   ├── bootp.c
│   ├── bootp.h
│   ├── cksum.c
│   ├── COPYRIGHT
│   ├── debug.h
│   ├── if.c
│   ├── if.h
│   ├── ip_icmp.c
│   ├── ip_icmp.h
│   ├── ip_input.c
│   ├── ip_output.c
│   ├── ip.h
│   ├── libslirp.h
│   ├── main.h
│   ├── mbuf.c
│   ├── mbuf.h
│   ├── misc.c
│   ├── misc.h
│   ├── sbuf.c
│   ├── sbuf.h
│   ├── slirp_config.h
│   ├── slirp.c
│   ├── slirp.h
│   ├── socket.c
│   ├── socket.h
│   ├── tcp_input.c
│   ├── tcp_output.c
│   ├── tcp_subr.c
│   ├── tcp_timer.c
│   ├── tcp_timer.h
│   ├── tcp_var.h
│   ├── tcp.h
│   ├── tcpip.h
│   ├── tftp.c
│   ├── tftp.h
│   ├── udp.c
│   └── udp.h
├── softmmu_defs.h
├── softmmu_exec.h
├── softmmu_header.h
├── softmmu_template.h
├── softmmu-semi.h
├── sparc-dis.c
├── sparc.ld
├── sparc64.ld
├── spice-qemu-char.c
├── sysconfigs
│   └── target
│       └── target-x86_64.conf
├── sysemu.h
├── target-alpha
│   ├── cpu.h
│   ├── helper.c
│   ├── helper.h
│   ├── machine.c
│   ├── op_helper.c
│   ├── STATUS
│   └── translate.c
├── target-arm
│   ├── cpu.h
│   ├── helper.c
│   ├── helper.h
│   ├── iwmmxt_helper.c
│   ├── machine.c
│   ├── neon_helper.c
│   ├── op_addsub.h
│   ├── op_helper.c
│   └── translate.c
├── target-cris
│   ├── cpu.h
│   ├── crisv10-decode.h
│   ├── crisv32-decode.h
│   ├── helper.c
│   ├── helper.h
│   ├── machine.c
│   ├── mmu.c
│   ├── mmu.h
│   ├── op_helper.c
│   ├── opcode-cris.h
│   ├── translate_v10.c
│   └── translate.c
├── target-i386             : XXX - This is our destiny
│   ├── cpu.h
│   ├── cpuid.c
│   ├── helper_template.h
│   ├── helper.c
│   ├── helper.h
│   ├── kvm.c
│   ├── machine.c
│   ├── op_helper.c
│   ├── ops_sse_header.h
│   ├── ops_sse.h
│   ├── svm.h
│   ├── TODO
│   └── translate.c
├── target-lm32
│   ├── cpu.h
│   ├── helper.c
│   ├── helper.h
│   ├── machine.c
│   ├── op_helper.c
│   ├── README
│   ├── TODO
│   └── translate.c
├── target-m68k
│   ├── cpu.h
│   ├── helper.c
│   ├── helpers.h
│   ├── m68k-qreg.h
│   ├── machine.c
│   ├── op_helper.c
│   ├── qregs.def
│   └── translate.c
├── target-microblaze
│   ├── cpu.h
│   ├── helper.c
│   ├── helper.h
│   ├── machine.c
│   ├── microblaze-decode.h
│   ├── mmu.c
│   ├── mmu.h
│   ├── op_helper.c
│   └── translate.c
├── target-mips
│   ├── cpu.h
│   ├── helper.c
│   ├── helper.h
│   ├── machine.c
│   ├── mips-defs.h
│   ├── op_helper.c
│   ├── TODO
│   ├── translate_init.c
│   └── translate.c
├── target-ppc
│   ├── cpu.h
│   ├── helper_regs.h
│   ├── helper.c
│   ├── helper.h
│   ├── kvm_ppc.c
│   ├── kvm_ppc.h
│   ├── kvm.c
│   ├── machine.c
│   ├── mfrom_table_gen.c
│   ├── mfrom_table.c
│   ├── op_helper.c
│   ├── STATUS
│   ├── translate_init.c
│   └── translate.c
├── target-s390x
│   ├── cpu.h
│   ├── helper.c
│   ├── helpers.h
│   ├── kvm.c
│   ├── machine.c
│   ├── op_helper.c
│   └── translate.c
├── target-sh4
│   ├── cpu.h
│   ├── helper.c
│   ├── helper.h
│   ├── machine.c
│   ├── op_helper.c
│   ├── README.sh4
│   └── translate.c
├── target-sparc
│   ├── cc_helper.c
│   ├── cpu_init.c
│   ├── cpu.h
│   ├── fop_helper.c
│   ├── helper.c
│   ├── helper.h
│   ├── int32_helper.c
│   ├── int64_helper.c
│   ├── ldst_helper.c
│   ├── machine.c
│   ├── mmu_helper.c
│   ├── op_helper.c
│   ├── TODO
│   ├── translate.c
│   ├── vis_helper.c
│   └── win_helper.c
├── target-unicore32
│   ├── cpu.h
│   ├── helper.c
│   ├── helper.h
│   ├── op_helper.c
│   └── translate.c
├── target-xtensa
│   ├── core-dc232b
│   │   ├── core-isa.h
│   │   └── gdb-config.c
│   ├── core-dc232b.c
│   ├── core-fsf
│   │   └── core-isa.h
│   ├── core-fsf.c
│   ├── cpu.h
│   ├── helper.c
│   ├── helpers.h
│   ├── machine.c
│   ├── op_helper.c
│   ├── overlay_tool.h
│   └── translate.c
├── targphys.h
├── tcg
│   ├── arm
│   │   ├── tcg-target.c
│   │   └── tcg-target.h
│   ├── hppa
│   │   ├── tcg-target.c
│   │   └── tcg-target.h
│   ├── i386
│   │   ├── tcg-target.c
│   │   └── tcg-target.h
│   ├── ia64
│   │   ├── tcg-target.c
│   │   └── tcg-target.h
│   ├── LICENSE
│   ├── mips
│   │   ├── tcg-target.c
│   │   └── tcg-target.h
│   ├── optimize.c
│   ├── ppc
│   │   ├── tcg-target.c
│   │   └── tcg-target.h
│   ├── ppc64
│   │   ├── tcg-target.c
│   │   └── tcg-target.h
│   ├── README
│   ├── s390
│   │   ├── tcg-target.c
│   │   └── tcg-target.h
│   ├── sparc
│   │   ├── tcg-target.c
│   │   └── tcg-target.h
│   ├── tcg-op.h
│   ├── tcg-opc.h
│   ├── tcg-runtime.h
│   ├── tcg.c
│   ├── tcg.h
│   ├── tci
│   │   ├── README
│   │   ├── tcg-target.c
│   │   └── tcg-target.h
│   └── TODO
├── tcg-runtime.c
├── tci-dis.c
├── tci.c
├── test-coroutine.c
├── test-qmp-commands.c
├── test-visitor.c
├── tests
│   ├── alpha
│   │   ├── crt.s
│   │   ├── hello-alpha.c
│   │   ├── Makefile
│   │   ├── test-cond.c
│   │   └── test-ovf.c
│   ├── cris
│   │   ├── check_abs.c
│   │   ├── check_addc.c
│   │   ├── check_addcm.c
│   │   ├── check_addi.s
│   │   ├── check_addiv32.s
│   │   ├── check_addm.s
│   │   ├── check_addo.c
│   │   ├── check_addoq.c
│   │   ├── check_addq.s
│   │   ├── check_addr.s
│   │   ├── check_addxc.s
│   │   ├── check_addxm.s
│   │   ├── check_addxr.s
│   │   ├── check_andc.s
│   │   ├── check_andm.s
│   │   ├── check_andq.s
│   │   ├── check_andr.s
│   │   ├── check_asr.s
│   │   ├── check_ba.s
│   │   ├── check_bas.s
│   │   ├── check_bcc.s
│   │   ├── check_bound.c
│   │   ├── check_boundc.s
│   │   ├── check_boundr.s
│   │   ├── check_btst.s
│   │   ├── check_clearfv32.s
│   │   ├── check_clrjmp1.s
│   │   ├── check_cmp-2.s
│   │   ├── check_cmpc.s
│   │   ├── check_cmpm.s
│   │   ├── check_cmpq.s
│   │   ├── check_cmpr.s
│   │   ├── check_cmpxc.s
│   │   ├── check_cmpxm.s
│   │   ├── check_dstep.s
│   │   ├── check_ftag.c
│   │   ├── check_gcctorture_pr28634-1.c
│   │   ├── check_gcctorture_pr28634.c
│   │   ├── check_glibc_kernelversion.c
│   │   ├── check_hello.c
│   │   ├── check_int64.c
│   │   ├── check_jsr.s
│   │   ├── check_lapc.s
│   │   ├── check_lsl.s
│   │   ├── check_lsr.s
│   │   ├── check_lz.c
│   │   ├── check_mapbrk.c
│   │   ├── check_mcp.s
│   │   ├── check_mmap1.c
│   │   ├── check_mmap2.c
│   │   ├── check_mmap3.c
│   │   ├── check_movdelsr1.s
│   │   ├── check_movecr.s
│   │   ├── check_movei.s
│   │   ├── check_movemr.s
│   │   ├── check_movemrv32.s
│   │   ├── check_moveq.c
│   │   ├── check_mover.s
│   │   ├── check_moverm.s
│   │   ├── check_movmp.s
│   │   ├── check_movpmv32.s
│   │   ├── check_movpr.s
│   │   ├── check_movprv32.s
│   │   ├── check_movscr.s
│   │   ├── check_movsm.s
│   │   ├── check_movsr.s
│   │   ├── check_movucr.s
│   │   ├── check_movum.s
│   │   ├── check_movur.s
│   │   ├── check_mulv32.s
│   │   ├── check_mulx.s
│   │   ├── check_neg.s
│   │   ├── check_not.s
│   │   ├── check_openpf1.c
│   │   ├── check_openpf2.c
│   │   ├── check_openpf3.c
│   │   ├── check_openpf4.c
│   │   ├── check_openpf5.c
│   │   ├── check_orc.s
│   │   ├── check_orm.s
│   │   ├── check_orq.s
│   │   ├── check_orr.s
│   │   ├── check_ret.s
│   │   ├── check_scc.s
│   │   ├── check_settls1.c
│   │   ├── check_sigalrm.c
│   │   ├── check_stat1.c
│   │   ├── check_stat2.c
│   │   ├── check_stat3.c
│   │   ├── check_stat4.c
│   │   ├── check_subc.s
│   │   ├── check_subm.s
│   │   ├── check_subq.s
│   │   ├── check_subr.s
│   │   ├── check_swap.c
│   │   ├── check_time1.c
│   │   ├── check_time2.c
│   │   ├── check_xarith.s
│   │   ├── crisutils.h
│   │   ├── crt.s
│   │   ├── Makefile
│   │   ├── README
│   │   ├── sys.c
│   │   ├── sys.h
│   │   └── testutils.inc
│   ├── hello-arm.c
│   ├── hello-i386.c
│   ├── hello-mips.c
│   ├── linux-test.c
│   ├── lm32
│   │   ├── crt.S
│   │   ├── linker.ld
│   │   ├── macros.inc
│   │   ├── Makefile
│   │   ├── test_add.S
│   │   ├── test_addi.S
│   │   ├── test_and.S
│   │   ├── test_andhi.S
│   │   ├── test_andi.S
│   │   ├── test_b.S
│   │   ├── test_be.S
│   │   ├── test_bg.S
│   │   ├── test_bge.S
│   │   ├── test_bgeu.S
│   │   ├── test_bgu.S
│   │   ├── test_bi.S
│   │   ├── test_bne.S
│   │   ├── test_break.S
│   │   ├── test_bret.S
│   │   ├── test_call.S
│   │   ├── test_calli.S
│   │   ├── test_cmpe.S
│   │   ├── test_cmpei.S
│   │   ├── test_cmpg.S
│   │   ├── test_cmpge.S
│   │   ├── test_cmpgei.S
│   │   ├── test_cmpgeu.S
│   │   ├── test_cmpgeui.S
│   │   ├── test_cmpgi.S
│   │   ├── test_cmpgu.S
│   │   ├── test_cmpgui.S
│   │   ├── test_cmpne.S
│   │   ├── test_cmpnei.S
│   │   ├── test_divu.S
│   │   ├── test_eret.S
│   │   ├── test_lb.S
│   │   ├── test_lbu.S
│   │   ├── test_lh.S
│   │   ├── test_lhu.S
│   │   ├── test_lw.S
│   │   ├── test_modu.S
│   │   ├── test_mul.S
│   │   ├── test_muli.S
│   │   ├── test_nor.S
│   │   ├── test_nori.S
│   │   ├── test_or.S
│   │   ├── test_orhi.S
│   │   ├── test_ori.S
│   │   ├── test_ret.S
│   │   ├── test_sb.S
│   │   ├── test_scall.S
│   │   ├── test_sextb.S
│   │   ├── test_sexth.S
│   │   ├── test_sh.S
│   │   ├── test_sl.S
│   │   ├── test_sli.S
│   │   ├── test_sr.S
│   │   ├── test_sri.S
│   │   ├── test_sru.S
│   │   ├── test_srui.S
│   │   ├── test_sub.S
│   │   ├── test_sw.S
│   │   ├── test_xnor.S
│   │   ├── test_xnori.S
│   │   ├── test_xor.S
│   │   └── test_xori.S
│   ├── Makefile
│   ├── pi_10.com
│   ├── qruncom.c
│   ├── runcom.c
│   ├── sha1.c
│   ├── test_path.c
│   ├── test-arm-iwmmxt.s
│   ├── test-i386-code16.S
│   ├── test-i386-muldiv.h
│   ├── test-i386-shift.h
│   ├── test-i386-ssse3.c
│   ├── test-i386-vm86.S
│   ├── test-i386.c
│   ├── test-i386.h
│   ├── test-mmap.c
│   ├── testthread.c
│   └── xtensa
│       ├── crt.S
│       ├── linker.ld
│       ├── macros.inc
│       ├── Makefile
│       ├── test_b.S
│       ├── test_bi.S
│       ├── test_boolean.S
│       ├── test_bz.S
│       ├── test_clamps.S
│       ├── test_fail.S
│       ├── test_interrupt.S
│       ├── test_loop.S
│       ├── test_mac16.S
│       ├── test_max.S
│       ├── test_min.S
│       ├── test_mmu.S
│       ├── test_mul16.S
│       ├── test_mul32.S
│       ├── test_nsa.S
│       ├── test_pipeline.S
│       ├── test_quo.S
│       ├── test_rem.S
│       ├── test_rst0.S
│       ├── test_sar.S
│       ├── test_sext.S
│       ├── test_shift.S
│       ├── test_timer.S
│       ├── test_windowed.S
│       └── vectors.S
├── thunk.c
├── thunk.h
├── TODO
├── trace
│   ├── control.c
│   ├── control.h
│   ├── default.c
│   ├── simple.c
│   ├── simple.h
│   ├── stderr.c
│   └── stderr.h
├── trace-events
├── translate-all.c
├── uboot_image.h
├── ui
│   ├── cocoa.m
│   ├── curses_keys.h
│   ├── curses.c
│   ├── d3des.c
│   ├── d3des.h
│   ├── keymaps.c
│   ├── keymaps.h
│   ├── qemu-spice.h
│   ├── sdl_keysym.h
│   ├── sdl_zoom_template.h
│   ├── sdl_zoom.c
│   ├── sdl_zoom.h
│   ├── sdl.c
│   ├── spice-core.c
│   ├── spice-display.c
│   ├── spice-display.h
│   ├── spice-input.c
│   ├── vnc_keysym.h
│   ├── vnc-auth-sasl.c
│   ├── vnc-auth-sasl.h
│   ├── vnc-auth-vencrypt.c
│   ├── vnc-auth-vencrypt.h
│   ├── vnc-enc-hextile-template.h
│   ├── vnc-enc-hextile.c
│   ├── vnc-enc-tight.c
│   ├── vnc-enc-tight.h
│   ├── vnc-enc-zlib.c
│   ├── vnc-enc-zrle-template.c
│   ├── vnc-enc-zrle.c
│   ├── vnc-enc-zrle.h
│   ├── vnc-enc-zywrle-template.c
│   ├── vnc-enc-zywrle.h
│   ├── vnc-jobs-async.c
│   ├── vnc-jobs-sync.c
│   ├── vnc-jobs.h
│   ├── vnc-palette.c
│   ├── vnc-palette.h
│   ├── vnc-tls.c
│   ├── vnc-tls.h
│   ├── vnc.c
│   ├── vnc.h
│   ├── x_keymap.c
│   └── x_keymap.h
├── usb-bsd.c
├── usb-linux.c
├── usb-redir.c
├── usb-stub.c
├── user-exec.c
├── VERSION
├── version.rc
├── vgafont.h
├── vl.c
├── x86_64.ld
├── xen-all.c
├── xen-mapcache.c
├── xen-mapcache.h
├── xen-stub.c
└── xtensa-semi.c

100 directories, 1802 files
