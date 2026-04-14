# 2026-04-12 — Resto Druid cap on 25-man raids

## Change
New hard rule in `rules/01-raid-compositions.md` capping the number of Resto Druids in any 25-man raid when the healer signup count exceeds the slot count. Bench rotation among capped Resto Druids still follows the standard fair-rotation rule in `rules/02-bench-rotation.md`, which gains a new "Composition caps override pure fairness" subsection describing the interaction.

## Reason
The roster has a relatively large pool of Resto Druids. Capping their count when healer signups overflow keeps healing composition diverse instead of stacking druids; the side effect of Resto Druids benching more often in overflow situations is intentional.

## Files touched
- `rules/01-raid-compositions.md`
- `rules/02-bench-rotation.md`