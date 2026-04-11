# CoffeeBreak — Claude Code Session Guide

## What this project is

CoffeeBreak is a **raid composition planner** for **World of Warcraft: The Burning Crusade 20th Anniversary Edition**. It uses Claude Code to form raid groups from Discord signup screenshots, respecting a strict set of rules.

## How this project works

1. **Rules** define constraints (composition, bench rotation, player constraints, specs). They live in `rules/` and evolve over time.
2. **Sets** are raid rosters — the output. They are generated into `sets/`, and each set informs the next (especially bench history).
3. **Reference material** (TBC class/raid knowledge) lives in `reference/`.
4. **Configuration** (raid schedule, officers, settings) lives in `config/project.md`.
5. **Changelog** tracks rule and roster changes in `changelog/`.

## Communication conventions

- When the user says **"make a note of it"**, **"write it down"**, or similar — always save the information to the appropriate **project file** (rules/, config/, reference/, etc.), not just to Claude memory. Project files are the source of truth.

## Key principles

- **Every rule matters.** Never skip, relax, or approximate a rule. If a conflict is discovered, flag it to the user before proceeding.
- **Sets are chained.** Bench history carries forward. Always read all prior sets before generating a new one.
- **Never assume player info.** If you don't know a player's class, spec, or role — ask. Do not guess.
- **Rules evolve.** When the user updates rules, note the change in `changelog/` and re-evaluate affected sets.
- **Research is allowed.** TBC class mechanics, raid requirements, etc. can be researched online. Store findings in `reference/`.

## Before generating a raid roster

1. Read `config/project.md` for raid schedule, officers, and settings.
2. Read all files in `rules/` for the current rule set.
3. Read all existing files in `sets/` (in order) for bench history and predecessor context.
4. Parse the Discord signup screenshot provided by the user.
5. **Cross-reference every player name against `rules/04-player-specs.md`** to identify class. But **always check the spec icon in the signup screenshot** — it shows the player's chosen spec for THIS raid and takes precedence over any previously recorded spec/role. Players can change specs between raids.
6. For icon/color reference, read `reference/class-colors-and-spec-icons.md` and compare against reference images in `reference/icons/`.
7. If any player's class/spec is unknown after cross-referencing, ask before proceeding.
8. Generate the roster, verifying every rule is satisfied.
9. List who is benched (if applicable) and why they were chosen for the bench.

## File operations manual

See `reference/file-operations-manual.md` for the complete guide on which files to read and update for every type of interaction (new signup, rule change, player info, etc.), including a dependency map and checklist.

## Directory layout

```
config/          → Raid schedule, officers, project settings
rules/           → Composition rules, bench rules, player constraints, spec info
sets/            → Generated raid rosters (date-named, chronologically ordered)
reference/       → TBC class/raid research material
changelog/       → Record of rule and roster changes over time
```
