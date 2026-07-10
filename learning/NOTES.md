# Teaching Notes — RC2014 Micro

## Workspace
- **Workspace root = this `learning/` folder** (not the repo root). All teach files live here:
  `MISSION.md`, `RESOURCES.md`, `lessons/`, `reference/`, `learning-records/`, `assets/`, this file.
- Primary artifact: `assets/RC2014-Micro-schematic.pdf` (Rev 1.1, 2019) + `.png` for embedding in lessons.

## Learner preferences
- Hardware-first, concrete-first, ground-up — start from the real schematic, not generic Z80 theory.
- Owns physical RC2014 machines; end goal is build + modify with full understanding.
- Same style as the MEGA65 learning project: grounded, cited, main points (not verbose), short lessons.

## Accuracy discipline (hard rule — mirrors MEGA65 project)
- **Cite every load-bearing claim against the schematic** (`assets/RC2014-Micro-schematic.*`). No parametric guesses.
- For exact pin/decode/timing facts, read the **datasheet** for that chip before asserting — don't infer.
- **Qualify variant-specific facts:** the **Micro** uses a **27C512** ROM (U6); the **Micro+** uses a
  **39SF010** (128K). Reset/clock/RAM are common. Never state a variant fact as universal.
- Separate verified fact from pedagogical framing. Mark anything not yet traced as "trace it" exercise, not fact.
- When a lesson surfaces a strong new source, queue it: `/pin-llm-wiki queue <url>`.

## Schematic facts established (Rev 1.1, transcribed + re-verified from 600–700 dpi crops of the drawing)
- ICs: **U4** Z80 CPU · **U3** HM62256 32K SRAM (RAM) · **U6** 27C512 64K EPROM (ROM) · **U2** MC68B50 ACIA
  (serial) · **U1** 74LS32 (OR; gates U1A/U1B/U1C visible) · **U10** 74LS32 (OR) ·
  **U5** 74HCT04 hex inverter (U5E/U5F = clock oscillator; **U5B → `IORQ`** confirmed; U5A/U5C/U5D
  used/spare in decode — *exact roles deferred to the decode lesson, not yet traced*).
- Clock: **Y1** crystal + **R6** feedback (across U5E, pin 11↔10) + **R7** series-to-crystal + **C7/C8**
  load caps → U5E (11→10) → U5F (13→12) → `CLK`. **7.3728 MHz is the standard RC2014 value from the
  BOM/assembly guide — the frequency is NOT printed on the schematic** (Y1 is labelled only "Crystal").
- Reset: **SW1** (SW_PUSH) + **R1** → `RESET`. **R5** = pull-up on the Z80 `INT`/`NMI` line(s) (control, not clock).
- ROM bank-selection: three 3-pin jumpers **JP2/JP3/JP4** (type JUMPER3, group "ROM Bank Selection");
  their select nets are labelled **S1/S2/S3** on the sheet → drive ROM A13/A14/A15 → pick an 8K page of
  the 64K EPROM (this IS the "factory ROM 8-digit label" scheme from `../wiki/sources/factory.md`).
  ⚠️ Earlier draft mislabelled the jumpers themselves as "S1/S2/S3" — corrected.
- Serial: **U2** ACIA + 6-pin **FTDI header = P1** (CONN_01x06; RX/TX via series **R3/R4** + two more `R`),
  small option jumper **JP1** → console 115200 8-N-1. ACIA register/port decode uses **A0→RS, A6→CS2,
  A7→CS1, M1→CS0, `WR`→R/W, `CLK`→RX/TX_CLK, IRQ→INT** (read off U2 pins — *to be written up in the serial lesson*).
- **Con1** = 40-pin RC2014 bus (A0–A15, D0–D7, control, 5V/GND, RX/TX, spares) → backplane expansion.
- Decoupling caps **C1–C5** array across VCC/GND.

## Next lesson candidates
- `0002` — **The clock block**: crystal + two 74HCT04 inverters as an oscillator; why 7.3728 MHz; what CLK feeds.
- `0003` — **Reset & the Z80 control signals** (RESET, M1, MREQ/IORQ, RD/WR, WAIT/INT).
- `0004` — **Memory & address decoding**: RAM vs ROM split on A15; ROM bank jumpers; build the memory map.
