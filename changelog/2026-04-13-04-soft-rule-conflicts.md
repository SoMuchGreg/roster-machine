# 2026-04-13 — Soft rule conflicts: pick arbitrarily

## Change
Added a "Soft rule conflicts" subsection to `rules/01-raid-compositions.md` → "General principles". When two or more soft rules can't all be satisfied for a given team or roster, the planner picks arbitrarily — soft rules have no fixed priority order among themselves, and there is no need to ask the user.

## Reason
Several soft rules exist (e.g., per-team Priest preference, per-team Enhancement Shaman preference, per-team Resto Druid soft cap) and rule 01 was previously silent on what to do when they conflict. A fresh Claude session would have had to either pick without authorization or ask the user every time.

## Files touched
- `rules/01-raid-compositions.md`