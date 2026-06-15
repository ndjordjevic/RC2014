# kianryan.co.uk

## Fetch log
- Inbox URL: https://www.kianryan.co.uk/2023-01-05-getting-started-with-z80asm-on-the-rc2014/
- Final URL: https://www.kianryan.co.uk/2023-01-05-getting-started-with-z80asm-on-the-rc2014/
- Fetched: 2026-06-15
- Pages: 1
- Mode: brief

## Landing page — Getting Started With z80asm on the RC2014

A tutorial covering a complete workflow for assembling Z80 code on a development machine and running it on an RC2014.

- **Hardware setup:** switch the RC2014 Classic II ROM bank from 32K BASIC to the Small Computer Monitor (SCM).
- **Toolchain install** (WSL or Ubuntu): `sudo apt install z80asm z80dasm srecord`.
- **Assemble:** use `z80asm` to compile source to a binary; "Hello World" example calls SCM's display API routine.
- **Convert to Intel HEX** for serial transfer: `srec_cat helloworld.bin -binary -offset 0x8000 -output helloworld.hex -intel -address-length=2`.
- **Run:** paste the hex into SCM to load into memory, then `g 8000` to execute at the address.
- **Tip:** the author uses tmux + minicom + vim for side-by-side editing and testing.
