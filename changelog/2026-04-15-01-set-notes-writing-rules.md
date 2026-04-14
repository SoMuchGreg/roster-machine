## Change

Added a canonical "Writing the `## Notes` section of a set file" subsection to `reference/file-operations-manual.md`, defining what belongs in a set's Notes section, what does not, and the required style. Both set templates (`reference/templates/25man-set.md`, `reference/templates/karazhan-set.md`) had their inline 2-bullet guidance replaced with a pointer to the new subsection. Also rewrote the Notes section of `sets/2026-04-15-wed-gruul-mag.md` to conform, and corrected its stale `## Bench (4)` header to `## Bench (3)` (Pergatori had been promoted off the bench when Ōtsu withdrew).

## Reason

Past Notes sections drifted into rule restatements, rule-compliance logs, standing guild conditions, and restatements of facts already in other sections of the same set file. This duplicated content the rule files already own and made the section noisy and hard to scan. Centralising the rules for what Notes is for — and what it explicitly is not for — protects the single-source-of-truth principle and keeps each set file readable.

## Files touched

- `reference/file-operations-manual.md`
- `reference/templates/25man-set.md`
- `reference/templates/karazhan-set.md`
- `sets/2026-04-15-wed-gruul-mag.md`