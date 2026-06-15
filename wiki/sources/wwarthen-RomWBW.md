---
type: source
source_url: https://github.com/wwarthen/RomWBW
tags: [romwbw, cpm, hbios, z80, z180, z280, firmware]
related: [rc2014.co.uk, smallcomputercentral.com, google-group-rc2014-z80]
product: romwbw
detail_level: brief
created: 2026-06-15
updated: 2026-06-15
---

**Index entry.** RomWBW (Wayne Warthen) is the major ROM-based system software for Z80/Z180/Z280 retro machines, including the RC2014 — a complete CP/M and work-alike implementation with a hardware-abstraction layer (HBIOS). One of the four firmware options listed on [[rc2014.co.uk]]. Deep-dive later for build/config details.

_All claims below are sourced from ../../raw/github/wwarthen-RomWBW.md unless otherwise noted._

## What it covers
- A portable CP/M / Z-System environment: HBIOS isolates hardware in the ROM, so a disk (CF/SD/USB) moves transparently between RomWBW systems.
- Broad hardware support: Z80/Z180/Z280 CPUs; banked memory; disk drivers (RAM, ROM, Floppy, IDE, CF, SD, USB); serial (UART/ASCI/ACIA/SIO); video (TMS9918, 6545, 8563, Xosera); PS/2 keyboard; RTC; CP/NET networking; VT-100 emulation.
- Dynamic drive-letter assignment and multi-slice mass storage (up to 256 slices/device, up to 2GB).
- Platforms: RetroBrew, RC2014, Small Computer Central, and more.

## Status
Active (413★, AGPLv3, latest pre-release v3.7.0-dev.11, June 2026).
