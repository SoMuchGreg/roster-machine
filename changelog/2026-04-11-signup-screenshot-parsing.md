# 2026-04-11 — Signup screenshot parsing rules

## Change

Added explicit rules for interpreting Discord signup screenshots to `reference/file-operations-manual.md`:

1. **Signup count format:** `X (+Y)` means X want to raid, Y are benched/tentative. Total signups = X + Y.
2. **Overflow benching:** If X exceeds the raid cap, additional players must be benched beyond the Y already marked.
3. **Screenshots are snapshots:** They change over time as players sign up, withdraw, or get benched. Always use the latest screenshot.

## Reason

A previous set (12.04) was incorrectly recorded as "ran with 26" when the screenshot said "26 (+3)" for a 25-man raid — the 26 was misinterpreted as the roster size instead of the signup count that still needed one more bench.

## Impact

- `reference/file-operations-manual.md` — added 3 new steps at the start of screenshot parsing