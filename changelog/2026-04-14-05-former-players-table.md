# 2026-04-14 — Separate "Former players" sub-table

## Change
Added a new `### Former players` sub-table at the bottom of `rules/04-players.md`, below Regular players. Moved `Thalynora` (the only departed player currently in the roster) out of the Priest rows in Regular players into the new table. The Former players table uses a minimal schema — `Player | Character(s) | Class | Notes` — since departed players have no live spec or priority. Updated the **Table ordering** paragraph to name all three sub-tables and to require that departing players be moved into Former players rather than tombstoned in place.

## Reason
Tombstoned (`~~struck-through~~`) rows inside Regular players polluted the active roster: they showed up in class counts, broke the sort-by-name visual scan, and risked being accidentally included in selection logic. A dedicated Former players table keeps historical names resolvable (for old signup screenshots, set files, and changelog entries) without mixing them into live raid-building data.

## Files touched
- `rules/04-players.md` — Table ordering paragraph updated; Thalynora removed from Regular players; new Former players sub-table added
- `changelog/2026-04-14-05-former-players-table.md` — this file
