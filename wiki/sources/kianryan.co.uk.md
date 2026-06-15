---
type: source
source_url: https://www.kianryan.co.uk/2023-01-05-getting-started-with-z80asm-on-the-rc2014/
tags: [z80asm, tutorial, rc2014, small-computer-monitor, srecord, assembly]
related: [smallcomputercentral.com, rc2014z80]
product: kianryan
detail_level: brief
created: 2026-06-15
updated: 2026-06-15
---

**Index entry.** A practical tutorial by Kian Ryan on getting started with `z80asm` on the RC2014 — assembling Z80 code on a PC and running it on the board via the Small Computer Monitor. A good hands-on counterpart to the z88dk C workflow. Deep-dive later if a fuller walkthrough is needed.

_All claims below are sourced from ../../raw/web/kianryan.co.uk.md unless otherwise noted._

## What it covers
- Switching an RC2014 Classic II from 32K BASIC to the Small Computer Monitor ([[smallcomputercentral.com]]).
- Installing the toolchain (WSL/Ubuntu): `sudo apt install z80asm z80dasm srecord`.
- Assembling a "Hello World" (calling SCM's display API), converting to Intel HEX with `srec_cat ... -offset 0x8000 ... -intel`, pasting into SCM, and running with `g 8000`.
- Workflow tip: tmux + minicom + vim.
