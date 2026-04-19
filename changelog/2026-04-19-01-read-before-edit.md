# 2026-04-19 — Read-before-edit cadence + tiered reading list

## Change
Extended the canonical reading list from "before parsing a screenshot" to "before any `Edit` or `Write` call". Split it into **Tier 1** (every edit) and **Tier 2** (roster or screenshot edits only) and promoted it to a top-level section in `reference/file-operations-manual.md`; the screenshot event's Step 1 now points at the promoted list. Added a cadence rule (Tier 1 read once per session at the first edit, with targeted re-reads on open-file/selection signals, edit-target dependencies, or suspected context compaction) and a post-edit consistency grep for edits that change rule, config, reference, or derived-file schema text.

## Reason
Past sessions saw inference mistakes from stale context (wrong-file inferences, missed cross-file stale references). Reading before edits catches those; tiering keeps non-roster edits cheap; the per-session cadence avoids redundant reads when cache is fresh; the grep catches stale cross-file pointers before they drift.

## Files touched
- `CLAUDE.md` — new "Before any file edit" section (cadence + post-edit grep subsection)
- `reference/file-operations-manual.md` — Reading list promoted to top-level, tiered; Step 1 of screenshot event points at it
- `changelog/2026-04-19-01-read-before-edit.md` — this file
