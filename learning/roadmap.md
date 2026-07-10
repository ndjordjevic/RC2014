# RC2014 Micro — learning roadmap (ground-up)

The active driver is [MISSION.md](./MISSION.md). This is the wider path; lessons are produced one at a
time within the learner's zone of proximal development.

## Phase 1 — Read the board (you are here)
1. **Reading the schematic** — title block, reference designators, buses, net labels, power symbols,
   the 9 functional blocks, full component inventory. → *Lesson 01* ✅
   Reference: [Component Inventory](./reference/rc2014-micro-component-inventory.html), [Glossary](./reference/GLOSSARY.html).

## Phase 2 — Block by block
2. **Clock** — Y1 crystal + 74HCT04 oscillator; 7.3728 MHz; what CLK drives.
3. **Reset & Z80 control signals** — RESET, M1, MREQ/IORQ, RD/WR, WAIT, INT, BUSRQ/BUSACK.
4. **The three buses** — address (A0–A15), data (D0–D7), control; how chips share them.
5. **Memory & address decoding** — RAM (U3) vs ROM (U6) split on A15; the 74LS32/74HCT04 glue.
6. **ROM bank-selection jumpers** — JP2/JP3/JP4 (select nets S1–S3) → ROM A13–A15 → 8K page; tie to the factory ROM label scheme.
7. **Serial console** — MC68B50 ACIA (U2) + FTDI header; I/O-space decode; 115200 8-N-1.
8. **The 40-pin RC2014 bus** — Con1; what expansion modules see.

## Phase 3 — Put it together
9. **Memory map** — draw the full 64K map of the Micro.
10. **A bus cycle, end to end** — trace "CPU fetches a byte from ROM" through every signal.

## Phase 4 — Build & modify
11. Assembly walkthrough, bring-up, and reasoning about modifications.
