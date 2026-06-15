# wwarthen/RomWBW

## Metadata
- Stars: 413
- Primary language: Assembly
- Default branch: master
- Latest release: v3.7.0-dev.11 (pre-release, 2026-06-07)
- License: GNU AGPLv3
- Homepage: http://wwarthen.github.io/RomWBW/
- Fetched: 2026-06-15
- Final URL: https://github.com/wwarthen/RomWBW

## Description
System Software for Z80/Z180/Z280 Computers.

## README (excerpt — brief/index capture)
RomWBW (Version 3.7, Wayne Warthen) provides a complete, commercial-quality implementation of CP/M (and work-alike) operating systems and applications for modern Z80/Z180/Z280 retro-computing hardware.

Supported developer communities/platforms include RetroBrew Computers, RC2014 (rc2014.co.uk) and RC2014-Z80, Retro Computing, and Small Computer Central.

Primary features — RomWBW isolates hardware-specific functions in the ROM, providing a hardware abstraction layer (HBIOS) so a disk (CF/SD/USB) is portable between systems:
- Z80 family CPUs: Z80, Z180, Z280
- Banked memory services for several banking designs
- Disk drivers: RAM, ROM, Floppy, IDE ATA/ATAPI, CF, SD, USB, Zip, Iomega
- Serial drivers: UART (16550-like), ASCI, ACIA, SIO
- Video drivers: TMS9918, SY6545, MOS8563, HD6445, Xosera
- Keyboard (PS/2) via VT8242 or PPI
- RTC drivers: DS1302, BQ4845
- CP/NET networking via Wiznet, MT011 or Serial
- Built-in VT-100 terminal emulation
- Dynamic disk drive-letter assignment; multiple slices (up to 256 per device, up to 2GB) per mass-storage device.

## Top-level structure
Not captured at brief/index level (metadata + README only). Documentation includes "RomWBW Hardware.pdf" and other guides under `Doc/`. Deep-dive later for full repo structure.
