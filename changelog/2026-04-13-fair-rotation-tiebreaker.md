# 2026-04-13 — Fair-rotation tiebreaker

## Change
Added a "Tiebreaker: composition target" subsection under "Fairness requirement" in `rules/02-bench-rotation.md`. Fair rotation previously had no answer when multiple candidates shared the same lowest cumulative bench count.

## Reason
Ties are common in practice (most priority-2 players currently share the same bench count for each raid location), so the rule needed to be deterministic and reproducible.

## Files touched
- `rules/02-bench-rotation.md`