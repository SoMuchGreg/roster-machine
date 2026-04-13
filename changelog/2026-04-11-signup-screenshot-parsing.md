# 2026-04-11 — Signup screenshot parsing rules

## Change
Added explicit rules for interpreting the Discord signup screenshot header (the `X (+Y)` format, overflow benching, and treating each screenshot as a point-in-time snapshot) to `reference/file-operations-manual.md` → Step 2.

## Reason
A previous set had been recorded with the wrong roster size because the signup count was misinterpreted as the roster size rather than as "players who want to raid, before bench-overflow is applied".

## Files touched
- `reference/file-operations-manual.md`