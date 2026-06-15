---
type: source
source_url: http://searle.x10host.com/z80/SimpleZ80.html
tags: [grant-searle, simple-z80, microsoft-basic, nascom, sbc, z80]
related: [rc2014.co.uk, mbasic-reference-manual, nascom-basic-manual]
product: searle-z80
detail_level: brief
created: 2026-06-15
updated: 2026-06-15
---

**Index entry.** Grant Searle's "7-chip Z80 computer" — the minimal Z80 single-board computer running Microsoft BASIC that is the direct design ancestor of the RC2014's ROM BASIC. Deep-dive later for the full circuit and ROM details.

_All claims below are sourced from ../../raw/web/searle.x10host.com.md unless otherwise noted._

## What it covers
- A minimal Z80 SBC: 7 ICs (6 with a USB-TTL cable), 8K ROM, 56K RAM (32K version also provided), Z80 overclocked to 7.3728 MHz, 115200 baud interrupt-driven serial with handshaking, ~200mA.
- Memory map: 0000–1FFF ROM, 2000–FFFF RAM. I/O: serial at 80–81 (covers 80–BF), rest free.
- Microsoft BASIC from the NASCOM 2, adapted for the SBC with serial I/O and inapplicable commands removed.
- Page sections cover specification, circuit, prototype, ROM hex/assembly, power-up, load/save, and interfacing; links to 6809/6502/FPGA and a CP/M-running Z80 variant.

## Significance
This design (and its NASCOM-derived BASIC) is what the RC2014 ([[rc2014.co.uk]]) built on; the BASIC matches the [[mbasic-reference-manual]] / [[nascom-basic-manual]] lineage.
