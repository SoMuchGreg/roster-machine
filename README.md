# CoffeeBreak

Raid composition planner for **World of Warcraft: The Burning Crusade 20th Anniversary Edition**, powered by Claude Code.

## Purpose

Form raid groups from Discord signups, respecting strict composition rules, player constraints, and fair bench rotation.

## Raid schedule

| Night | Content             | Format    | Groups |
|-------|---------------------|-----------|--------|
| 1     | Karazhan            | 10-man    | 3      |
| 2     | Gruul + Magtheridon | 25-man    | 1      |

## Structure

| Directory    | Purpose                                              |
|------------- |------------------------------------------------------|
| `config/`    | Raid schedule, officers, project settings             |
| `rules/`     | Composition rules, bench rotation, player constraints |
| `sets/`      | Generated raid rosters (ordered, chained)             |
| `reference/` | TBC class and raid research material                  |
| `changelog/` | History of rule and roster changes                    |

## How it works

1. User provides a **Discord signup screenshot** for a raid night.
2. Claude Code reads all rules and prior rosters (bench history).
3. Raid groups are formed respecting every rule.
4. Output is saved as a numbered set in `sets/`.

## Key files

- `CLAUDE.md` — Persistent instructions for Claude Code sessions
- `config/project.md` — Active configuration (schedule, officers, settings)
- `rules/01-raid-compositions.md` — Required tank/healer/DPS counts
- `rules/02-bench-rotation.md` — Bench fairness and officer exemption
- `rules/03-player-constraints.md` — Must-be-together / must-not-be-together
- `rules/04-player-specs.md` — Player classes and specializations
