## Change

Added a "When to write a changelog entry at all" subsection to `reference/file-operations-manual.md` → "Changelog scope rule", making changelog entries conditional rather than mandatory. An entry is now required only when the change (a) alters an algorithm, vocabulary, or defined term, (b) touches multiple files under `rules/`, `config/`, or `reference/`, or (c) could retroactively reframe how prior sets should be read. All other edits — typos, wording clarifications, formatting, single-file tweaks, link updates — skip the changelog. The "Event: User reports a new rule or rule change" table and the corresponding line in `CLAUDE.md` were updated to match.

## Reason

The changelog was duplicating what `git log` already records, growing linearly with every rule edit, and forcing repeated exclusion carve-outs because reading it during roster formation is unsafe. Most entries described changes that no future reader would actually search for. Restricting the changelog to consequential changes preserves the narrative-summary value for the few edits that warrant it, while letting git carry the routine audit trail.

## Files touched

- `reference/file-operations-manual.md`
- `CLAUDE.md`