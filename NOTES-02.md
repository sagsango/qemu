# Init the keyboard
main()
  └── machine->init(...)
        └── pc_init_pci()
              └── pc_init1()
                    └── i8042_init(...)

pc_init1()
 ├── i8259_init()
 │     └── i8259[1]  (IRQ1)
 │
 └── i8042_init(i8259[1], i8259[12], 0x60)
        ├── ps2_kbd_init(IRQ1)
        ├── ps2_mouse_init(IRQ12)
        ├── register_ioport(0x60)
        └── register_ioport(0x64)




# How and who will use this keyboard to give inputs
-----------------------
[ Host Keyboard ]
        |
        v
[ SDL / VNC / Cocoa ]
        |
        v
[ kbd_put_keycode() ]
        |
        v
[ PS2KbdState FIFO ]
        |
        v
[ KBDState (i8042) ]
  |  ports 0x60/0x64
  |  IRQ1
        |
        v
[ i8259 PIC ]
        |
        v
[ Guest CPU IRQ1 ]

-----------------------


--------------------------------------------------
Host key press
  ↓
SDL_PollEvent()                    (sdl.c)
  ↓
sdl_process_key()
  ↓
kbd_put_keycode(scancode)          (input glue)
  ↓
ps2_queue(&kbd->common, byte)      (ps2.c)
  ↓
KBDState notices pending data       (pckbd.c)
  ↓
qemu_set_irq(IRQ1, 1)              (i8259)
  ↓
Guest CPU interrupt
  ↓
Guest reads port 0x60
--------------------------------------------------
