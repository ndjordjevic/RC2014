# RC2014 Micro — from the schematic up · Resources

> High-trust only. Knowledge is drawn from here, not parametric guesses. Annotate every entry.

## Knowledge — primary (verified against the artifact)

- [RC2014 Micro schematic — Rev 1.1, March 2019 (KiCad)](assets/RC2014-Micro-schematic.pdf) · PNG: [assets/RC2014-Micro-schematic.png](assets/RC2014-Micro-schematic.png)
  **The** primary source for this mission — the actual board drawing. Every component/net claim must trace here.
  Original: https://8b8bf43264c2f150841a.b-cdn.net/wp-content/uploads/2019/08/RC2014-Micro.pdf
- [RC2014 Micro Assembly Guide (PDF)](assets/RC2014-Micro-Assembly-Guide.pdf)
  Official build manual — bill of materials, placement, power-up. Use for: confirming part values/positions.
  Original: https://8b8bf43264c2f150841a.b-cdn.net/wp-content/uploads/2019/08/RC2014-Micro-Assembly-Guide.pdf
- [Local wiki — RC2014 Micro](../wiki/sources/rc2014.co.uk.md) and [[../wiki/sources/factory.md]] context
  Repo's curated knowledge base. **Start lookups here** per `../AGENTS.md`. Use for: kit specs, the ROM 8-digit
  bank-label scheme (the factory ROM page), firmware options.
- [Grant Searle — Simple Z80 computer](http://searle.x10host.com/z80/SimpleZ80.html) · local: [../raw/web/searle.x10host.com.md](../raw/web/searle.x10host.com.md)
  The minimal Z80 + Microsoft BASIC design the RC2014 descends from. Use for: memory-map lineage
  (8K ROM low / 32K–56K RAM high), why A15 splits ROM vs RAM, the serial-only console model.

## Knowledge — datasheets (component-level, fetch when a block needs depth)

- Zilog **Z80 CPU** (Z84C00) datasheet/user manual — pinout, bus signals, timing. *(queue when we do the CPU block)*
- **HM62256** 32K×8 SRAM datasheet — the RAM (U3). *(queue for the memory block)*
- **27C512** 64K×8 EPROM datasheet — the ROM (U6); A13–A15 high lines. *(queue for ROM/bank block)*
- **MC68B50** ACIA datasheet — the serial controller (U2); CS0–CS2/RS/E register decode. *(queue for serial block)*
- **74LS32** quad OR gate / **74HCT04** hex inverter datasheets — the glue logic. *(queue for decode block)*

## Wisdom — Communities

- [RC2014-Z80 Google Group](https://groups.google.com/g/rc2014-z80) · local: [../raw/web/google-group-rc2014-z80.md](../raw/web/google-group-rc2014-z80.md)
  The main RC2014 community forum. Use for: design questions, "why is this wired this way", mods.
  **Access method (verified 2026-06-16):** `WebSearch` with `site:groups.google.com/g/rc2014-z80 <topic>`
  finds relevant threads (e.g. ROM/RAM jumper settings, board quirks); `WebFetch` on the resulting thread URL
  then pulls the actual posts, often with author attribution (confirmed working on a thread from Spencer Owen,
  RC2014's designer). Google's own Groups UI is JS-heavy, but this two-step search→fetch path renders real
  content reliably. Queue any thread that yields a load-bearing fact via `/pin-llm-wiki queue <url>` so it's
  captured as a cited source rather than re-fetched each time.

## Gaps
- No annotated/verified memory-map document for the Micro yet — the exact address decode boolean
  (RAM /CS, ROM /CE, ACIA select ports) should be traced from the schematic and written up as a
  reference doc during the memory/decode lesson, rather than asserted from generic Z80 knowledge.
