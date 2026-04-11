# 2026-04-11 — Bench rotation tracked per raid location

## Change

Rule 02 (Bench Rotation) updated: bench fairness is now tracked **per raid location** (Karazhan and Gruul+Mag independently), not just as a single overall count.

## Reason

It's unfair if one player always gets benched from Karazhan but never from Gruul+Mag (or vice versa). Per-location tracking ensures balanced rotation across both raid types.

## Impact

- `rules/02-bench-rotation.md` — updated fairness requirement language
- `reference/bench-history.md` — restructured into separate Karazhan and Gruul+Mag sections (data was already location-tagged, now formally split)
- No existing sets need regeneration — this applies going forward