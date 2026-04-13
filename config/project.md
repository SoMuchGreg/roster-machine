# Project Configuration

This file holds CoffeeBreak's **configuration data** — the canonical facts that other rules and workflows read. The project's purpose and structure live in `README.md`; the session workflow and key principles live in `CLAUDE.md`. This file is data only.

## Terminology

| Term | Meaning |
|------|---------|
| **Raid team** | The full 10 or 25-man group forming the raid squad (e.g., "Team Restaurant") |
| **Raid location** | The specific raid instance: Karazhan, Gruul, Magtheridon, Serpentshrine Cavern, Tempest Keep, etc. |
| **Party group** (or "party", "single group") | The 5-man unit within a raid team. 10-man raids = 2 party groups, 25-man raids = 5 party groups |

## Raid schedule

| Night | Content            | Format                | Raid teams |
|-------|--------------------|-----------------------|------------|
| 1     | Karazhan           | 10-man raid           | 3          |
| 2     | Gruul + Magtheridon| 25-man raid           | 1          |

## Officers

Guild leadership list. This is project metadata — a record of who the guild's officers are. It is **not** what controls bench exemption. Bench exemption is enforced by the **raid spot priority** system in `rules/04-player-specs.md` (Priority column) and `rules/02-bench-rotation.md` (definitions and selection algorithm). Officer status and priority are conceptually distinct; if you ever need a non-officer to always play, or an officer to be bench-eligible, edit the Priority column in `rules/04-player-specs.md` — do not edit this list.

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