# 2026-04-13 — Under-cap raid behavior

## Change
Added under-cap rules to `rules/01-raid-compositions.md`. Universal default (in General principles): no one is benched for fair-rotation/priority/capacity reasons when signups are below the cap. Per-format overrides: 25-man raids always run regardless of signup count; Karazhan team count (2 vs 3) depends on signup thresholds, with explicit handling for the 25–26 ambiguous range, a hard "no outside tanks" recruitment limit at 27–29, and an insufficient-tanks override that drops to 2 teams when guild tank supply (after dual-spec flex) can't staff 3.

## Reason
Rule 01 was previously silent on under-cap behavior. A fresh Claude session would have had to guess whether to cancel, run short, or drop teams.

## Files touched
- `rules/01-raid-compositions.md`