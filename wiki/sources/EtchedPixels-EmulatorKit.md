---
type: source
source_url: https://github.com/EtchedPixels/EmulatorKit
tags: [emulator, rc2014, rcbus, retrobrew, z80, fuzix]
related: [rc2014z80]
product: emulatorkit
detail_level: brief
created: 2026-06-15
updated: 2026-06-15
---

**Index entry.** EmulatorKit (Alan Cox / EtchedPixels) is a collection of C emulators focused on the RC2014/RCbus environment and Retrobrew (N8VEM) systems, aimed at software development and testing rather than cycle-accurate simulation. Deep-dive later for build and per-machine usage.

_All claims below are sourced from ../../raw/github/EtchedPixels-EmulatorKit.md unless otherwise noted._

## What it covers
- Many CPU cores: Z80/Z180/Z280, 8080/8085/8086/8008, 6502/65C02/65C816, 6800/6803/6809/68HC11, 68000-family, 1802, NS32K, Z8, and more.
- RC2014/RCbus/BP80 processor cards and official RC2014 card emulation (512K ROM/RAM, Compact Flash, dual SIO/2, IDE 82C55 PPIDE, pageable/switchable ROM, RTC, 64K RAM) plus many other RCbus peripherals (TMS9918A, CTC, floppy, PS/2 keyboard, W5100…).
- Integrated systems (SC108/114/126/720, Easy Z80, Z280RC…), Retrobrew machines, Grant Searle's 9-chip Z80, Nascom 1/2/3, and numerous vintage computers.

## Status
Active development (168★, GPLv3, C).
