# File Operations Manual

Step-by-step guide for when to read and update each file, organized by trigger event.

---

## Event: New signup screenshot received

### Step 1 — Read (before parsing)

| File | Why |
|------|-----|
| `rules/04-player-specs.md` | Know existing players' classes, specs, and notes (last resort, no-show, etc.) |
| `reference/class-colors-and-spec-icons.md` | Identify unknown players by icon/color |
| `reference/icons/specs/*.jpg` | Compare spec icons side-by-side if needed |
| `reference/icons/classes/*.png` | Compare class icons side-by-side if needed |
| `reference/bench-history.md` | Know who has been benched most/least for fair rotation |
| `rules/01-raid-compositions.md` | Know required tank/healer/DPS counts |
| `rules/02-bench-rotation.md` | Know bench rules and officer exemptions |
| `rules/03-player-constraints.md` | Know must-together, must-not-together, availability constraints |
| All files in `sets/` | Predecessor context, especially recent bench history |

### Step 2 — Parse the screenshot

1. Identify all signups by name, cross-referencing `04-player-specs.md` for class.
2. **Check the spec icon for every player** — it shows their spec for THIS raid and overrides any previously recorded spec/role.
3. For unknown players: use icon/color to determine class+spec. If unsure, ask the user.
4. Note absent players and late signups.

### Step 3 — Build the roster (if asked to)

1. Apply all rules from `rules/`.
2. Determine bench based on `reference/bench-history.md` (bench those with fewest benches, never officers).
3. Respect player constraints from `rules/03-player-constraints.md`.
4. Respect "last resort" and "low priority" flags from `rules/04-player-specs.md`.
5. Present roster to user for approval.

### Step 4 — Write/Update (after user confirms)

| File | What to update |
|------|----------------|
| `sets/YYYY-MM-DD-day-raid.md` | **Create new file.** Record signups, roster, bench, notes. |
| `reference/bench-history.md` | **Update.** Add new bench entries, increment counts. |
| `rules/04-player-specs.md` | **Update IF** a new player appeared, or an existing player's spec changed. |

---

## Event: User provides historical roster data

Same as above, but:
- The roster is already decided — just record it.
- Still update `bench-history.md` and `04-player-specs.md` with any new information.

---

## Event: User reports a new rule or rule change

### Update these files:

| File | What to update |
|------|----------------|
| The relevant `rules/*.md` file | Add/modify the rule |
| `changelog/*.md` | **Create entry** documenting what changed and when |
| `config/project.md` | Update if it affects raid schedule, officers, or settings |
| `CLAUDE.md` | Update if it affects the workflow process |

### Then check:
- Do any existing sets in `sets/` need to be re-evaluated?
- Does `bench-history.md` need adjustment?

---

## Event: User provides player-specific information

(e.g., "X is a warrior", "Y has two specs", "Z is last resort only")

### Update:

| File | What to update |
|------|----------------|
| `rules/04-player-specs.md` | Update player's class, spec, or notes |
| `rules/03-player-constraints.md` | Update if it's a must-together/must-not-together/availability constraint |

---

## Event: A player joins or leaves the guild

### Update:

| File | What to update |
|------|----------------|
| `rules/04-player-specs.md` | Add new player row, or strike through departed player |
| `reference/bench-history.md` | Strike through departed player (keep for history) |
| `rules/03-player-constraints.md` | Remove any constraints involving departed player |

---

## Event: User asks me to form raid groups

This is the core deliverable. Follow the full "New signup screenshot received" flow above, plus:

1. Read **every** file in `sets/` to understand predecessor context.
2. Present the proposed roster clearly (tables with player, role, class).
3. Explicitly list who is benched and why (bench count).
4. Flag any rule conflicts or impossible constraints.
5. Wait for user confirmation before saving.

---

## File dependency map

```
config/project.md ─────────────┐
                                │
rules/01-raid-compositions.md ──┤
rules/02-bench-rotation.md ─────┤
rules/03-player-constraints.md ─┼──> INPUTS for generating a set
rules/04-player-specs.md ───────┤
                                │
reference/bench-history.md ─────┤
reference/class-colors-and-spec-icons.md ──> REFERENCE for parsing screenshots
reference/icons/**/* ───────────┘

sets/*.md ──────────────────────> OUTPUTS (each set is also INPUT for the next)

changelog/*.md ─────────────────> AUDIT TRAIL (written when rules change)

CLAUDE.md ──────────────────────> META (workflow instructions, read every session)
README.md ──────────────────────> META (project overview, rarely updated)
```

---

## Quick checklist: "Did I forget to update something?"

After any interaction, check:

- [ ] New player seen? → `04-player-specs.md`
- [ ] Someone benched? → `bench-history.md`
- [ ] Spec changed from previous? → `04-player-specs.md`
- [ ] Rule added/changed? → `rules/*.md` + `changelog/`
- [ ] Player left/joined? → `04-player-specs.md` + `03-player-constraints.md` + `bench-history.md`
- [ ] New set created? → `sets/YYYY-MM-DD-day-raid.md`
- [ ] Constraint added? → `03-player-constraints.md`
