# Signup Rate — Karazhan / Gruul / Magtheridon

Counterpart of `signup-history-karazhan-gruul-mag.md` that expresses engagement as a percentage: the share of in-scope raids a player has signed up for since their first in-scope signup. Tracks only current non-officer members; officers, former members, and players with zero in-scope signups are excluded.

## What the stat means

- **Signups** — the count from `signup-history-karazhan-gruul-mag.md` → Current members (Karazhan / Gruul / Magtheridon scope only).
- **First signup** — earliest date the player appears in the `## Signups (from Discord)` section of any **in-scope** set file in `sets/` (Karazhan / Gruul's Lair / Magtheridon's Lair only — old-world sets are ignored for this file, matching the numerator scope).
- **Raids in window** — the count of in-scope set files in `sets/` dated on or after the player's first signup. Each player has their own window starting at their own first signup; no rolling, no cap.
- **Signup rate** — `Signups ÷ Raids-in-window`, expressed as a percentage. Range 0.0% to 100.0%.

The rate is fully cumulative over the player's in-scope tenure — a miss from months ago still drags the current percentage down, and only asymptotically recovers as more attended raids stack up. Both numerator and denominator change only when a new in-scope set is filed, so calendar drift alone never moves the rate.

## Scope and maintenance

Both numerator and denominator follow the scope of `signup-history-karazhan-gruul-mag.md` (Karazhan / Gruul's Lair / Magtheridon's Lair sets only).

Update on any trigger that updates `signup-history-karazhan-gruul-mag.md` — a new in-scope set, an edit to one, a join, a leave, a rename. For every current non-officer member, recompute Signups and Raids-in-window using the player's First signup date, then recompute Signup rate. Re-sort by Signup rate desc (alphabetical case-insensitive tiebreak) and renumber `#` from `1`.

No recompute is needed between in-scope set events — the stat is stable until a new set lands.

## Computed as of

**2026-04-20**

## Current members — signup rate since first in-scope signup

| #  | Player              | First signup | Signup rate |
|----|---------------------|--------------|-------------|
| 1  | Beaverfist          | 2026-03-15   | 100.0%      |
| 2  | Bergamotka/Tymoti   | 2026-03-15   | 100.0%      |
| 3  | Bombzor             | 2026-03-22   | 100.0%      |
| 4  | Dankyn              | 2026-03-04   | 100.0%      |
| 5  | Ebonybolt           | 2026-03-22   | 100.0%      |
| 6  | Gresac              | 2026-02-22   | 100.0%      |
| 7  | Leontes             | 2026-04-08   | 100.0%      |
| 8  | Lightweit           | 2026-04-08   | 100.0%      |
| 9  | Lynelen             | 2026-03-11   | 100.0%      |
| 10 | Pergatori           | 2026-03-22   | 100.0%      |
| 11 | Roossy/Keatala      | 2026-03-15   | 100.0%      |
| 12 | Spot/Yorekbarn      | 2026-04-19   | 100.0%      |
| 13 | Verysadge           | 2026-02-22   | 100.0%      |
| 14 | Marino-Varthier     | 2026-02-22   | 94.4%       |
| 15 | OomToDoom           | 2026-02-22   | 94.4%       |
| 16 | Thordrel            | 2026-02-22   | 94.4%       |
| 17 | Vaelruna            | 2026-02-22   | 94.4%       |
| 18 | Yxanb               | 2026-03-04   | 92.9%       |
| 19 | Jabbadhutt          | 2026-03-15   | 90.9%       |
| 20 | Tonsen              | 2026-03-15   | 90.9%       |
| 21 | Ostbirger           | 2026-03-22   | 88.9%       |
| 22 | Gigakox             | 2026-03-25   | 87.5%       |
| 23 | McHughes            | 2026-02-22   | 83.3%       |
| 24 | Heligeman/Fugleman  | 2026-04-05   | 80.0%       |
| 25 | Dwarfytron          | 2026-03-22   | 77.8%       |
| 26 | CptKavior           | 2026-04-08   | 75.0%       |
| 27 | McJudgin            | 2026-03-29   | 71.4%       |
| 28 | BestPractice        | 2026-02-22   | 66.7%       |
| 29 | CodeHunt/Rainbound  | 2026-03-25   | 62.5%       |
| 30 | Siljes/Ejlis        | 2026-03-25   | 62.5%       |
| 31 | Rhoator             | 2026-03-01   | 60.0%       |
| 32 | Doughball           | 2026-03-11   | 50.0%       |
| 33 | Ōtsu                | 2026-03-04   | 42.9%       |
| 34 | Eselman             | 2026-03-22   | 33.3%       |
| 35 | Sjwammie            | 2026-03-11   | 33.3%       |
| 36 | Lightstarr          | 2026-03-18   | 30.0%       |
| 37 | Varva               | 2026-04-08   | 25.0%       |
| 38 | Drillbabe           | 2026-03-04   | 21.4%       |
| 39 | Blacksi             | 2026-02-22   | 5.6%        |