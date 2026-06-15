# searle.x10host.com

## Fetch log
- Inbox URL: http://searle.x10host.com/z80/SimpleZ80.html
- Final URL: http://searle.x10host.com/z80/SimpleZ80.html
- Fetched: 2026-06-15
- Pages: 1
- Mode: brief (fetched via curl; site's HTTPS cert altname is invalid so WebFetch was bypassed)

## Landing page — Grant's 7-chip Z80 computer

Grant Searle's "Grant's 7-chip Z80 computer (only 6 chips if using a USB to TTL serial cable) — a fully operational Z80 computer running BASIC." Last updated 12 Oct 2017.

Specification:
- 8K ROM, 56K RAM (a 32K-RAM version is also provided)
- Z80 processor overclocked to 7.3728 MHz (4MHz+ Z80B parts work; halving the crystal to 3.6864 MHz drops serial to 57600 baud)
- 115200 baud serial interface, RS232 voltage levels, full interrupt-driven input with buffer and hardware handshaking
- ~200mA power consumption
- Microsoft BASIC as used in the Nascom 2, modified for the SBC with all I/O via serial; commands not applicable to the SBC removed
- Minimal component count — 7 ICs plus a few discrete components

Memory map: 0000–1FFF = 8K ROM; 2000–FFFF = RAM (56K). I/O map: 00–7F free (128 in/128 out ports); 80–81 serial interface (minimally decoded, covers 80–BF); C0–FF free.

Page sections: Specification, Memory and I/O map, Circuit diagram/description, Prototype, ROM assembly and hex files, ROM BASIC details, Powering up, Loading and saving, Interfacing. Also links to 6809, 6502, FPGA, and a more complex Z80-running-CP/M version. This minimal design is the direct ancestor of the RC2014's Microsoft BASIC.
