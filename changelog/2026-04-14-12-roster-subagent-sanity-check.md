## Change

Added a mandatory sanity-check step to `reference/file-operations-manual.md` → Event: New signup screenshot received → Step 3 (Build the roster). After finalizing a roster and before presenting it to the user, spawn a fresh sub-agent that independently re-reads every active rule file and verifies the proposed roster against them. The sub-agent answers a single yes/no question — "Does this roster adhere to all rules specified in this project?" — and lists any violations. The main agent must not modify the roster based on the sub-agent's output, and must present the roster together with the verdict verbatim.

## Reason

A second, independent pass catches rule violations the main agent missed during construction. Keeping the roster frozen between the check and presentation preserves user agency: the user, not the planner, decides how to react to flagged violations.

## Files touched

- `reference/file-operations-manual.md`