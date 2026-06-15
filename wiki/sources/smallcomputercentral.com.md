---
type: source
source_url: https://smallcomputercentral.com/small-computer-monitor/small-computer-monitor-v1-0/
tags: [small-computer-monitor, scm, z80-monitor, steve-cousins, debugging]
related: [rc2014.co.uk, kianryan.co.uk]
product: small-computer-monitor
detail_level: brief
created: 2026-06-15
updated: 2026-06-15
---

**Index entry.** Small Computer Central is Steve Cousins' site and the home of the Small Computer Monitor (SCM) v1.0 — the Z80 machine-code monitor that ships as one of the RC2014's firmware options. Deep-dive later for command reference and ROM-building.

_All claims below are sourced from ../../raw/web/smallcomputercentral.com.md unless otherwise noted._

## What it covers
- **SCM** — "a classic machine code monitor for Z80 based systems": inline assembler/disassembler, register and memory examine/set, breakpoints, single-step, Intel `.hex` loading. (Known limit: single-step won't advance on non-branching conditional jumps.)
- **Supported hardware:** RC2014; the Small Computer series (SC101/108/111/114/118); LiNC80; Z280RC; Z80SBC64; Tom Szolyga's SBC-C; Z80sc.
- **Docs/downloads:** Installation guide, Reference Sheet, Tutorial, User Guide (edition 1.0.0, plus Italian translation); the SCWorkshop v0.2.0 package bundles source, prebuilt ROM images, and docs.

## Notes
SCM is the same monitor referenced by [[rc2014.co.uk]] (versions "9"/"88" in the factory ROM scheme) and is the ROM used in the z80asm tutorial at [[kianryan.co.uk]].
