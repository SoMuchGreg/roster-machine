# 2026-04-14 — Row-index `#` column added to roster tables

## Change
Added a leading `#` column to all three roster sub-tables in `rules/04-players.md` (Officers, Regular players, Former players). The column holds a single continuous integer that runs from `1` in Officers through Regular players and into Former players, so every player in the file has a unique small integer. Officers currently occupy `1`–`5`, Regular players `6`–`42`, Former players `43`. Added a **Row index (`#` column)** paragraph directly under **Table ordering**, explaining that the index is derived from sort order — not a stable ID — and must be renumbered from `1` whenever rows are added, removed, moved between sub-tables, or reordered.

## Reason
Referring to a specific player by "the shaman at position N" or "row N" was clumsy, and with 43 rows across three sub-tables it was easy to miscount. A continuous integer index gives every player a short, unambiguous handle that is cheap to type, easy to say out loud, and trivial to cross-reference from other documents (sets, notes, screenshots). Making the index continuous across sub-tables — rather than restarting at 1 per table — avoids collisions when players are moved (e.g., retiring into Former players) and keeps "player 27" meaning one and only one person at any moment.

## Files touched
- `rules/04-players.md` — new `Row index (#)` paragraph, new `#` column in all three roster sub-tables, all rows numbered 1–43
- `changelog/2026-04-14-06-roster-row-index.md` — this file
