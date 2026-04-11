# Project Configuration

## Project metadata

- **Name:** CoffeeBreak
- **Created:** 2026-04-10
- **Type:** Non-code, rule-based set generation
- **Tool:** Claude Code (cognitive + research + memory)

## Requirements

These are the foundational requirements as specified at project creation:

1. **No actual code.** This project produces markdown and text files only.
2. **Rule completeness.** Every generated set must satisfy every active rule — no exceptions.
3. **Set chaining.** Each new set is influenced by all predecessor sets (especially bench history).
4. **Rule evolution.** Rules will change over time. When they do, downstream effects on existing and future sets must be considered.
5. **Domain specificity.** The project operates within WoW TBC 20th Anniversary Edition raid planning.
6. **Self-referencing.** All output files in this project form the input context for every subsequent prompt.
7. **Traceability.** Changes to rules and their impact on sets are tracked in `changelog/`.
8. **No assumptions about players.** If unsure about a player's class, spec, or role — ask the user. Never guess.

## Domain

**World of Warcraft: The Burning Crusade 20th Anniversary Edition** — raid and group composition planning.

The user will provide Discord signup screenshots. From those, raid groups must be formed respecting all active rules. The output is raid rosters for each raid night.

## Terminology

| Term | Meaning |
|------|---------|
| **Raid team** | The full 10 or 25-man group forming the raid squad (e.g., "Team Restaurant") |
| **Raid location** | The specific raid instance: Karazhan, Gruul, Magtheridon, Serpentshrine Cavern, Tempest Keep, etc. |
| **Party group** (or "party", "single group") | The 5-man unit within a raid team. 10-man raids = 2 party groups, 25-man raids = 5 party groups |

## Raid schedule

| Night | Content            | Format                | Raid teams |
|-------|--------------------|-----------------------|--------|
| 1     | Karazhan           | 10-man raid           | 3      |
| 2     | Gruul + Magtheridon| 25-man raid           | 1      |

## Officers (exempt from bench rotation)

| Officer name         | Notes                          |
|----------------------|--------------------------------|
| Mirohl               |                                |
| Jar                  |                                |
| Glaivemaster Baebay  |                                |
| Kres/Dissi           | Same person, two characters    |
| Greg (Ucannotpass)   | Character name: Ucannotpass    |

## Active settings

| Setting              | Value                     | Notes                                         |
|----------------------|---------------------------|-----------------------------------------------|
| Domain               | WoW TBC 20th Anniversary  | Raid composition planning                     |
| Rule strictness      | Absolute                  | Every rule must be respected, no exceptions   |
| Set ordering         | Sequential                | Sets are date-named and chained chronologically |
| Research allowed     | Yes                       | Online research for TBC class/raid knowledge  |
| Output format        | Markdown/Text             | All deliverables as .md or .txt files         |
| Input method         | Discord screenshots       | User provides signup screenshots              |

## What's next

- Continue generating weekly raid rosters from Discord signup screenshots
- Refine rules as new edge cases emerge
- Add 5-man group composition rules (upcoming)
