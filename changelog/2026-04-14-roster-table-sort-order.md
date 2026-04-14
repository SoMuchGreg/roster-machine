# 2026-04-14 — Roster tables sorted by class, then by name

## Change
Added a **Table ordering** rule to `rules/04-players.md` directly under the `## Known player roster` heading: rows in both the Officers and Regular players sub-tables are sorted first by class alphabetically, then by player name alphabetically within each class. Reordered every row in both sub-tables to match. Tombstoned entries (e.g. `~~Thalynora~~`) stay in their alphabetical slot.

## Reason
The roster tables had grown in roughly chronological order, which made it hard to find a player, hard to spot duplicates, and hard to scan class coverage at a glance. A deterministic sort key removes those problems and makes "where does this new row go?" a mechanical question rather than a judgment call.

## Files touched
- `rules/04-players.md` — new **Table ordering** paragraph + both sub-tables reordered
- `changelog/2026-04-14-roster-table-sort-order.md` — this file
