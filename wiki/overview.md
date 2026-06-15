---
type: overview
domain: "RC2014 retro computer"
created: 2026-06-15
updated: 2026-06-15
sources: [rc2014.co.uk, rc2014z80, wwarthen-RomWBW, smallcomputercentral.com, searle.x10host.com, z88dk-techdocs-rc2014, kianryan.co.uk, EtchedPixels-EmulatorKit, wikipedia-cpm, primrosebank-cpm-commands, cpm-primer, rc2014-micro-assembly-guide, mbasic-reference-manual, nascom-basic-manual, starting-forth, blabley.org, z80kits.com, google-group-rc2014-z80, MwHCpvYDoq8-rc2014-mini, jT_trjP0-rU-adding-a-rc2014-micro-to-a-backplane]
---

# RC2014 retro computer — overview

This wiki is, for now, an **index** of RC2014 resources — one concise entry per source describing what it is and what it covers. We expand individual sources into depth later, when we need them. The RC2014 is a simple, modular 8-bit Z80 homebrew computer (8K ROM, 32K RAM, 7.3728 MHz, serial at 115,200 baud), originally built to run Microsoft BASIC and extended board by board on a backplane.

**Official project**

[[rc2014.co.uk]] is the official home and shop — indexing the kits, bus modules, assembly guides, troubleshooting, and the four firmware environments (Microsoft BASIC, CP/M, RomWBW, Small Computer Monitor).

[[rc2014z80]] is the official GitHub organisation behind the shop — indexing the flagship RC2014 repo (schematics, ROM build trees, CP/M images, BASIC programs), picoterm, the BASIC-programs collection, a z88dk mirror, plus the "Using Z88DK" guide and the Factory ROM set with its 8-digit label scheme.

**Firmware & software**

[[wwarthen-RomWBW]] is the major ROM-based CP/M / Z-System software (HBIOS) for Z80/Z180/Z280 machines including the RC2014.

[[smallcomputercentral.com]] is Steve Cousins' site and home of the Small Computer Monitor (SCM), the Z80 machine-code monitor that is one of the RC2014's firmware options.

[[searle.x10host.com]] is Grant Searle's minimal "7-chip" Z80 computer running Microsoft BASIC — the direct design ancestor of the RC2014's ROM BASIC.

**Development & tooling**

[[z88dk-techdocs-rc2014]] holds z88dk's RC2014-target reference docs (board doc, memory map, ROM configuration).

[[kianryan.co.uk]] is a hands-on tutorial for assembling Z80 code with `z80asm` and running it via SCM.

[[EtchedPixels-EmulatorKit]] is a collection of C emulators for the RC2014/RCbus environment (and many other vintage machines) aimed at software development and testing.

**CP/M reference**

[[wikipedia-cpm]] gives the background on CP/M — Kildall's 1974 OS (BIOS/BDOS/CCP, `.COM` files) that the RC2014 runs.

[[primrosebank-cpm-commands]] is a practical reference to CP/M's CCP and its internal vs transient commands.

[[cpm-primer]] is *The CP/M Primer*, a beginner's book on using CP/M.

**Kits, BASIC & FORTH references**

[[rc2014-micro-assembly-guide]] is the official build manual (PDF) for the RC2014 Micro.

[[mbasic-reference-manual]] is the Microsoft BASIC-80 (MBASIC) language reference — the lineage of RC2014 ROM BASIC.

[[nascom-basic-manual]] is the NASCOM BASIC manual, the closest documented ancestor of that ROM BASIC.

[[starting-forth]] is Leo Brodie's *Starting FORTH*, the classic introduction to FORTH on Z80 machines.

**Reviews, shop & community**

[[blabley.org]] is Brad Dickinson's review/build write-up of the RC2014 Micro.

[[z80kits.com]] is the official retailer's RC2014 Micro shop listing (price, kit contents, Micro/Micro+ variants).

[[google-group-rc2014-z80]] is the main RC2014 community forum.

[[MwHCpvYDoq8-rc2014-mini]] is a short video showcasing the RC2014 Mini.

[[jT_trjP0-rU-adding-a-rc2014-micro-to-a-backplane]] is a video covering assembly of a 5-slot backplane and adding the RC2014 Micro+.
