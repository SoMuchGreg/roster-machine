# 2026-04-12 — Set file templates introduced

## Change
Added `reference/templates/karazhan-set.md` and `reference/templates/25man-set.md` as canonical structures for new set files. `reference/file-operations-manual.md` Step 4 now instructs Claude to start from a template (copying it into `sets/` with the date-based filename).

## Reason
Historical sets had drifted into several different structures (bench/roster ordering, 25-man roster style, Karazhan team order, column sets). A canonical template removes that ambiguity and forces consistent structure for downstream bench-history reads. Templates live under `reference/templates/` rather than `sets/` because they are reference scaffolding for *how to write a set*, not raid sets themselves — `sets/` stays a clean append-only log of actual raid nights.

## Files touched
- `reference/templates/karazhan-set.md` (new)
- `reference/templates/25man-set.md` (new)
- `reference/file-operations-manual.md`