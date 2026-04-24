# Historical Gruul+Mag Assignments (Pre-Template Corpus)

## Purpose

Pre-template historical encounter-assignment data for Gruul+Mag (High King Maulgar council + Magtheridon cube clickers). Supplies continuity data to `rules/05-encounter-assignments.md` → "Assignment algorithm" for raids that predate the `## Encounter assignments` section in date-indexed record files.

This file lives in `records/` as the lone non-date-indexed outlier — the leading `_` in the filename signals that it breaks the standard `YYYY-MM-DD-day-raid.md` naming convention. It is categorically a historical record (per `CLAUDE.md` → "File purposes" → Historical record), just in a grouped, undated form.

## Status

- **Static.** This corpus does not grow. New assignments are recorded in standard date-indexed record files under `records/` (structure defined in `reference/templates/gruul-mag-record.md`) via their `## Encounter assignments` section. Once those accumulate, they become the primary continuity source per `rules/05-encounter-assignments.md` → "Continuity data sources".
- **Non-normative, not a rule.** The rule that *uses* this data is `rules/05-encounter-assignments.md`. Do not promote entries here into rules or restate them elsewhere.
- **Datasets are undated.** Datasets A through G below were provided by the user without dates and are not linked to specific date-indexed record files. For continuity decisions, treat every dataset as "prior" without any finer relative ordering — use dataset order (A first, G last) as the sole tiebreaker when the continuity algorithm in `rules/05-encounter-assignments.md` needs a recency call.
- **Player names are verbatim; role labels are normalized.** The *player name* cells below preserve the original spellings (e.g., `Mirhol` for `Mirohl`, `Mairën`/`Marien` for the former player `Mairen/Zorÿa`, `Varathier` for `Marino-Varthier`, `Valeruna` for `Vaelruna`) — the repetition of a spelling across datasets is itself signal that the same real player held the role. *Role labels* (the left side of each bullet), however, are normalized to match `rules/05-encounter-assignments.md` → "Encounter roles" so that continuity lookup is a direct string match — the one intentional exception is `Boomy Tank` (see the terminology bullet below), which is distinctive enough to preserve as prior vocabulary. When the assignment algorithm builds its continuity list, normalize each player name against `rules/04-players.md` → canonical `Player` column (using `Character(s)` and `Notes` to disambiguate); do **not** rewrite this file.
- **Former-guild players appear freely.** Many names below refer to players now in `rules/04-players.md` → Former players (Venguard, Calendril, Aserrah, Ryro, Sourbuns, Rhoator, Mairen/Zorÿa, Jinothy, Bhandage, Bombzor, Lixly, Kryxs, Zemp, Fredfull, etc.). They contribute to the historical record but **cannot satisfy continuity for current raids** — they're not eligible for the roster. The algorithm's step 1 (filter by eligibility) drops them automatically.
- **"Boomy Tank" is prior terminology for "Kiggler Tank".** Dataset A uses the older label; treat `Boomy Tank` / `Boomy Tank Healer` / `Boomy Tank MD` as continuity entries for the Kiggler Tank / Kiggler Tank Healer / Kiggler Tank MD roles respectively.
- **Off-scope continuity.** Datasets A–G include information that `rules/05-encounter-assignments.md` → "Intentionally out of scope" excludes from formal assignment tracking. Those entries are preserved verbatim as context and may be consulted by the raid leader, but the assignment algorithm only reads roles that `rules/05-encounter-assignments.md` → "Encounter roles" defines. Out-of-scope stanzas below are grouped under explicit `(out of scope for rule 05, recorded for context)` sub-headings.

## Datasets

### Dataset A

**High King Maulgar:**
- Maulgar Tank: Venguard, Mirhol
- Maulgar Healer: Thordrel, Calendri
- Maulgar Tank MD: Vaelruna
- Mage Tank: Oomtoodoom
- Mage Tank Healer: Bhandage
- Boomy Tank: Gresac
- Boomy Tank Healer: Aserrah
- Boomy Tank MD: Rhoator

**Olm the Summoner:**
- Olm Tank: Ryro (until Felhunter has been summoned)
- Felhunter Subjugate: Marien

**Blindeye the Seer:**
- Blindeye Tank: Sourbuns
- Blindeye Tank MD: Lixly

**Gruul (the Dragonkiller) — out of scope for rule 05, recorded for context:**
- Main Tank: Venguard
- Off-Tank: Sourbuns
- Main Tank Healer: Thordrel
- Off-Tank Healer: Calendril
- Main Tank MD: Vaelruna
- Off-Tank MD: Rhoator

**Magtheridon — Phase 1 add tanks (out of scope for rule 05, recorded for context):**
- South (Kill-target 1): Venguard
- South East (Kill-target 2): Venguard
- South West (Kill-target 3): Mirhol
- North East (Kill-target 4): Ryro
- North West (Kill-target 5): Sourbuns

**Magtheridon — elemental banishers (out of scope for rule 05, recorded for context):**
- First 3 elementals banished by: Marien (1), BestPractice (2), McHughes (3). All exceeding elementals must be killed.

**Magtheridon — main fight (out of scope for rule 05, recorded for context):**
- Main Tank: Venguard
- Main Tank Healers: Thordrel, Calendril, Kres/Dissi
- Off-Tank: Mirhol

**Magtheridon — Cube Clickers:**
- South (Star): Sourbuns
- South East (Triangle): Marien
- South West (Circle): Gresac
- North East (Square): Greg (Ucannotpass)
- North West (Diamond): Ryro

### Dataset B

**High King Maulgar:**
- Maulgar Tank: Mirhol
- Maulgar Healer: Thordrel, (Pug)
- Mage Tank (Krosh): Oomtoodoom
- Mage Tank Healer: Kresnik
- Kiggler Tank: Valeruna & Ucannotpass
- Kiggler Tank Healer: Gresac
- Olm Tank: Dankyn (until felhunter)
- Felhunter Subjugate: Ôtsu
- Blindeye Tank: Varthier

**Magtheridon — Cube Clickers:**
- South (Star): UcannotPass
- South East (Triangle): Mairën
- South West (Circle): Vaelruna
- North East (Square): Ôtsu
- North West (Diamond): Jinothy

### Dataset C

**High King Maulgar:**
- Maulgar Tank: Mirhol
- Maulgar Healer: Thordrel, Beaverfist
- Mage Tank (Krosh): Oomtoodoom
- Mage Tank Healer: Kresnik
- Kiggler Tank: Tonsen & Ucannotpass
- Kiggler Tank Healer: Gresac
- Olm Tank: Eselman (until felhunter)
- Felhunter Subjugate: Ôtsu, McHughes
- Olm Tank Healer: Bombzor
- Blindeye Tank: Varthier
- Blindeye Tank Healer: Keatala

**Magtheridon — Main Tank (out of scope for rule 05, recorded for context):**
- Main Tank: Varthier

**Magtheridon — Cube Clickers:**
- South (Star): UcannotPass
- South East (Triangle): McHughes
- South West (Circle): Rhoator
- North East (Square): Mirohl
- North West (Diamond): Ôtsu

### Dataset D

**High King Maulgar:**
- Maulgar Tank: Varthier
- Maulgar Healer: Thordrel, Bombzor
- Mage Tank (Krosh): Oomtoodoom
- Mage Tank Healer: Beaverfist
- Kiggler Tank: CodeHunt & Ucannotpass
- Kiggler Tank Healer: Sjwammie
- Olm Tank: Eselman (until felhunter)
- Felhunter Subjugate: Jabbadhutt, McHughes
- Olm Tank Healer: Ejlis
- Blindeye Tank: Doughball
- Blindeye Tank Healer: Jar

**Magtheridon — Main Tank (out of scope for rule 05, recorded for context):**
- Main Tank: Varthier

**Magtheridon — Cube Clickers:**
- South (Star): UcannotPass
- South East (Triangle): McHughes
- South West (Circle): Pergatori
- North East (Square): Doughball
- North West (Diamond): Mirohl

### Dataset E

**High King Maulgar:**
- Maulgar Tank: Mirhol
- Maulgar Healer: Thordrel, Ejlis
- Mage Tank (Krosh): Oomtoodoom (Dwarfytron MD)
- Mage Tank Healer: Keatala
- Kiggler Tank: Beaverfist (Tonsen MD)
- Kiggler Tank Healer: Bombzor
- Olm Tank: Ostbirger (until felhunter)
- Felhunter Subjugate: BestPractice, McHughes
- Olm Tank Healer: Heligeman
- Blindeye Tank: Varthier (Vaelruna MD)
- Blindeye Tank Healer: Gresac

**Magtheridon — Main Tank (out of scope for rule 05, recorded for context):**
- Main Tank: Mirohl

**Magtheridon — Cube Clickers:**
- South (Star): UcannotPass
- South East (Triangle): McHughes
- South West (Circle): Bestpractice
- North East (Square): Varathier
- North West (Diamond): Ostbirger

### Dataset F

**High King Maulgar:**
- Maulgar Tank: Mirhol (Dwarfytron MD)
- Maulgar Healer: Thordrel, Ejlis
- Mage Tank (Krosh): OomTooDoom
- Mage Tank Healer: Beaverfist
- Kiggler Tank: Tonz & Ucannotpass
- Kiggler Tank Healer: Lightweit
- Olm Tank: Ostbirger (until felhunter)
- Felhunter Subjugate: Jabbadhutt
- Olm Tank Healer: McJudgin
- Blindeye Tank: Varthier (Vaelruna MD)
- Blindeye Tank Healer: Gresac

**Magtheridon — Main Tank (out of scope for rule 05, recorded for context):**
- Main Tank: Mirohl

**Magtheridon — Cube Clickers:**
- South (Star): Pergatori
- South East (Triangle): Ucannotpass
- South West (Circle): Jabbadhutt
- North East (Square): Varathier
- North West (Diamond): Ostbirger

### Dataset G

**High King Maulgar:**
- Maulgar Tank: Mirohl
- Maulgar Healer: Thordrel, Bombzor
- Mage Tank (Krosh): OomTooDoom
- Mage Tank Healer: Keatala
- Kiggler Tank: Beaverfist
- Kiggler Tank Healer: Lightweit
- Olm Tank: Varthier (until felhunter)
- Felhunter Subjugate: Jabbadhutt, McHughes
- Olm Tank Healer: McJudgin
- Blindeye Tank: Ostbirger (Vaelruna MD)
- Blindeye Tank Healer: Gresac

**Magtheridon — Main Tank (out of scope for rule 05, recorded for context):**
- Main Tank: Mirohl

**Magtheridon — Cube Clickers:**
- South (Star): Kresniik
- South East (Triangle): Ucannotpass
- South West (Circle): Mchughes
- North East (Square): Varathier
- North West (Diamond): Ostbirger
