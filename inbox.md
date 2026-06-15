# Inbox

Drop URLs below under `## Pending`. Run `/pin-llm-wiki run <url>` to ingest a single URL (auto-queues it if missing), or `/pin-llm-wiki run` to batch-process every pending item. Agents may use `/pin-llm-wiki queue <url>` to suggest URLs without immediately ingesting them.

## Pending

<!-- Add URLs here, one per line, as markdown checkboxes.
     Supported inline tags (append each wrapped in HTML comment syntax):
       detail:brief        — override detail level for this source
       detail:standard
       detail:deep
       branch:dev          — GitHub: use this branch instead of default
       clone               — GitHub deep: full git clone to raw/github/<org>-<repo>/
       skip                — skip this URL on the next run
       companion:github.com/<org>/<repo>  — web: use this repo as companion (skip auto-discovery)
       no-companion        — web: suppress companion GitHub fetch even if a repo is found
       note: <text>        — freeform note for human review (ignored by ingest)
-->

<!-- ── Tier 1: Official / canonical ── -->
- [ ] https://rc2014.co.uk/
- [ ] https://github.com/RC2014Z80
- [ ] https://github.com/RC2014Z80/RC2014/wiki/Using-Z88DK
- [ ] https://github.com/RC2014Z80/RC2014/tree/master/ROMs/Factory
- [ ] https://rc2014.co.uk/full-kits/rc2014-micro/
- [ ] https://rc2014.co.uk/1716/basic-cp-m-romwbw-or-small-computer-monitor/

<!-- ── Tier 2: Core software / firmware ── -->
- [ ] https://github.com/wwarthen/RomWBW
- [ ] https://smallcomputercentral.com/small-computer-monitor/small-computer-monitor-v1-0/
- [ ] http://searle.x10host.com/z80/SimpleZ80.html

<!-- ── Tier 3: Toolchain / development ── -->
- [ ] https://github.com/z88dk/techdocs/tree/master/targets/rc2014
- [ ] https://www.kianryan.co.uk/2023-01-05-getting-started-with-z80asm-on-the-rc2014/

<!-- ── Tier 4: Emulation ── -->
- [ ] https://github.com/EtchedPixels/EmulatorKit

<!-- ── Tier 5: CP/M, BASIC & FORTH reference ── -->
- [ ] https://en.wikipedia.org/wiki/CP/M
- [ ] http://www.primrosebank.net/computers/cpm/cpm_commands.htm
- [ ] https://archive.org/details/cpm-primer-second-edition
- [ ] https://8b8bf43264c2f150841a.b-cdn.net/wp-content/uploads/2019/08/RC2014-Micro-Assembly-Guide.pdf
- [ ] https://archive.org/stream/BASIC-80_MBASIC_Reference_Manual/BASIC-80_MBASIC_Reference_Manual_djvu.txt
- [ ] http://www.nascomhomepage.com/pdf/Basic.pdf
- [ ] https://archive.org/details/startingforthint0000brod_x5o5

<!-- ── Tier 6: Reviews, shop & community ── -->
- [ ] https://blabley.org/review-the-rc2014-micro-single-board-z80-retrocomputer/
- [ ] https://z80kits.com/shop/rc2014-micro/
- [ ] https://groups.google.com/g/rc2014-z80
- [ ] https://www.youtube.com/watch?v=MwHCpvYDoq8
- [ ] https://www.youtube.com/watch?v=jT_trjP0-rU

## Completed

<!-- Processed lines are moved here automatically.
     Format after ingest: - [x] https://... with an "ingested YYYY-MM-DD" HTML comment appended.
     To re-fetch: add a "refresh" HTML comment to the line, then run /pin-llm-wiki run.
     The refresh tag is removed automatically after re-fetch.
-->
