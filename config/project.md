# Project Configuration

This file holds CoffeeBreak's **configuration data** — the canonical facts that other rules and workflows read. The project's purpose and structure live in `README.md`; the session workflow and key principles live in `CLAUDE.md`. This file is data only.

## Terminology

| Term | Meaning |
|------|---------|
| **Raid team** | The full 10 or 25-man group forming the raid squad (e.g., "Team Restaurant") |
| **Raid location** | The specific raid instance: Karazhan, Gruul, Magtheridon, Serpentshrine Cavern, Tempest Keep, etc. |
| **Party group** (or "party", "single group") | The 5-man unit within a raid team. 10-man raids = 2 party groups, 25-man raids = 5 party groups |
| **Canonical name** | The `Player` column value in `rules/04-players.md` — the identifier under which a player's signups, benches, and historical data are aggregated. May be a single name (e.g., `Mirohl`) or a **composite** joining two or more names commonly used to refer to the player: `Kres/Dissi` (multiple characters), `Marino-Varthier` (real name + character), `Glaivemaster Baebay` (title + character). A name is added to the composite whenever it is commonly used to refer to that player; rarely-used names stay in `Character(s)` only. Signups under any component of the composite, any `Character(s)` entry, or a decorated form like `Greg (Ucannotpass)` all collapse to the canonical |
| **Character** | A single in-game character. A player may control one or several characters, listed in the `Character(s)` column of `rules/04-players.md` |
| **Main** | A player's primary character — the one whose class/spec appears in the `Class` and `Spec 1 (role)` columns of `rules/04-players.md` |
| **Alt** | Any secondary character of the same player, typically of a different class or role. Listed alongside the main in `Character(s)`; called out in the `Notes` column (e.g., *"Dissi = Druid alt"*, *"Warrior main, Shaman alt"*) |

## Raid schedule

| Night | Content            | Format                | Raid teams |
|-------|--------------------|-----------------------|------------|
| 1     | Karazhan           | 10-man raid           | 3          |
| 2     | Gruul + Magtheridon| 25-man raid           | 1          |

## Old World raids

A historical raid category: **signup tracking only, no roster formation**. No composition targets, no bench rotation, no dual-spec flex — none of the rules under `rules/` apply to these raids. They exist in the project solely to record who signed up.

Raids in this category:

| Abbreviation | Full name          |
|--------------|--------------------|
| ZG           | Zul'Gurub          |
| AQ20         | Ahn'Qiraj (20-man) |
| Ony          | Onyxia's Lair      |

## Active settings

| Setting              | Value                     | Notes                                         |
|----------------------|---------------------------|-----------------------------------------------|
| Domain               | WoW TBC 20th Anniversary  | Raid composition planning                     |
| Input method         | Discord screenshots       | User provides signup screenshots              |

## What's next

- Continue generating weekly raid rosters from Discord signup screenshots
- Refine rules as new edge cases emerge
- Add 5-man group composition rules (upcoming)