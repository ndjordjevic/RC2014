# Mission: RC2014 Micro — from the schematic up

## Why
I own a couple of RC2014 computers and want to *truly* build and understand the **RC2014 Micro**
from the ground up — not as a user who flashes a ROM, but as someone who can look at the bare
schematic and explain what every chip, net, and jumper does, then build and modify with confidence.
Hardware first, the same ground-up way I'm learning the MEGA65.

## Success looks like
- Point at **any** symbol on the RC2014 Micro schematic (any IC, resistor, capacitor, jumper,
  net label, connector pin) and say what it is and which functional block it belongs to.
- Draw the Micro's block diagram from memory: CPU, clock, reset, RAM, ROM, address decoding,
  serial ACIA, the 40-pin bus — and how the buses tie them together.
- Explain the Micro's memory map and how the ROM **bank-selection jumpers** pick an 8K page.
- Trace a single bus cycle (e.g. "CPU reads a byte from ROM") through the glue logic.
- Eventually: assemble/modify the board and reason about changes confidently.

## Path (conceptual → deep)
1. **Read the schematic** — vocabulary, the title block, every component, the buses, the 9 blocks. *(start here — Lesson 01)*
2. Block by block: clock oscillator · reset · the Z80 buses · RAM/ROM & address decoding · ROM bank jumpers · the MC68B50 serial console · the 40-pin RC2014 bus.
3. Memory map & a full bus cycle, end to end.
4. Build/modify: assembly, bring-up, and changes.

## Constraints
- Hardware-first, concrete-first. Start from the real RC2014 Micro schematic (Rev 1.1, 2019), not generic Z80 theory.
- Self-paced, multi-session. Wiki-first per repo `AGENTS.md`, then primary docs (schematic, Searle's design), then web/community.
- Teach the **RC2014 Micro specifically**; note where the **Micro+** differs (39SF010 128K ROM vs 27C512).

## Out of scope (for now)
- Writing Z80 assembly / BASIC / CP/M software — that comes after the hardware foundation is solid.
- Other RC2014 form factors (Mini, Classic, Pro) except as brief contrast.
- Generic electronics fundamentals lectures — introduce concepts just-in-time, tied to a part on this board.
