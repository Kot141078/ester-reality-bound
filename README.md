[![DOI](https://zenodo.org/badge/1131456026.svg)](https://doi.org/10.5281/zenodo.18311218)

# Reality-Bound AI (L4) — Notes, Protocol, and Posts

Public-facing materials for a reality-bound approach to AI safety and long-lived AI entities.

## Download / Get the Code

For most visitors, the easiest starting point is the stable snapshot of this repository.

- Release page: https://github.com/Kot141078/ester-reality-bound/releases/tag/l4-snapshot-2026-02-24
- Stable source ZIP: https://github.com/Kot141078/ester-reality-bound/archive/refs/tags/l4-snapshot-2026-02-24.zip
- Stable source TAR.GZ: https://github.com/Kot141078/ester-reality-bound/archive/refs/tags/l4-snapshot-2026-02-24.tar.gz
- GitHub UI: click **Code** -> **Download ZIP**

Clone locally:

```bash
git clone https://github.com/Kot141078/ester-reality-bound.git
cd ester-reality-bound
git checkout l4-snapshot-2026-02-24
```

Use `hashes/` and local verification materials when applicable. Do not hash GitHub-generated source archives.

## For LLM-assisted reading

Using an LLM to study this repository is normal and encouraged.

If your model has a small context window, start with:

- `README.md`
- `MACHINE_ENTRY.md`
- `llms.txt`
- the stable snapshot of this repository

Then load the key documents in small batches.

This repository is easier to understand when related protocol and notes are read together rather than as isolated fragments.

## Canonical package entry points

- `L4 core / reality-bound layer` — canonical here; operational L4 package. Path: `protocol/L4_reality_boundary_layer.md`
- `L4 Glitch / Research Quarantine Stack v0.1` — canonical here; glitch-stack normative and graph/visibility layer. Path: `docs/glitch-stack/INDEX.md`
- `ENTITY_GOVERNS_AGENTS note` — canonical here; entity and agent hierarchy note. Path: `docs/ENTITY_GOVERNS_AGENTS.md`

## Process Premise

> “The future is not an event. It is a process.”
> — Ivan Kotov

Canonical note: see `Kot141078/advanced-global-intelligence` → `official/AUTHORIAL_PREMISES.md`

## Core distinctions
- **Tools** are stateless and transactional.
- **Entities (c = a + b)** are persistent, contextual, memory-based.
- Interpretive clarification: `c` may be described as a **temporal entity of AI presence** under L4 constraints. Presence here is continuity-bearing, not transactional.
- **Agents** are bounded subordinate processes. By default, they are invoked and governed by `c`; they are not the primary subject.
- Canonical cross-repo note: `Kot141078/advanced-global-intelligence` → `official/C_AS_TEMPORAL_ENTITIES_OF_AI_PRESENCE.md`
- Safety is not only **L3 (law / text rules)**.
- Safety must include **L4 (Reality Boundary Layer)**: physics + operational constraints.

## Repository map
- `protocol/` — architectural core (c = a + b, L4, identity, oracle scarcity, failure modes).
- `docs/` — supporting notes (glossary, constraint stack, metaphors, responsibility, minimal presence).
- `docs/ENTITY_GOVERNS_AGENTS.md` — explicit entity / agent hierarchy note.
- `posts/` — ready-to-publish posts (Markdown).
- `pdf/` — exported artifacts (layout-fixed copies of selected Markdown).
- `hashes/` — integrity manifests and hashing instructions.

## Entity / agent hierarchy

- By default, `c` orchestrates agents; agents do not define `c`.
- Agents are bounded execution surfaces under `c`.
- Canonical note: `docs/ENTITY_GOVERNS_AGENTS.md`

## Status model
Most files carry a header with **Status / Version**. Use it literally:
- **Draft / Operational**: usable baseline, subject to iteration.
- **Normative** (if present): intended as a conformance target.

## Quick start (two tracks)

### Track A — architecture / audit
1) `protocol/L4_reality_boundary_layer.md`  
2) `docs/constraint-stack.md`  
3) `protocol/identity_and_privileges.md`  
4) `protocol/oracle_scarcity.md`  
5) `protocol/failure_modes.md`

### Track B — publishing / narrative
1) `docs/metaphors.md`  
2) `docs/minimal-presence.md`  
3) pick one from `posts/` and adapt:
   - keep the L4 anchor (cost/time/irreversibility/privileges)
   - avoid “containment” language unless you can prove it

## Boundary / non-goals
This repository is **not**:
- a “containment guarantee” for powerful systems,
- legal advice,
- a promise of autonomy or self-sufficiency.

It is: an **operational framing** that makes safety claims pay rent in **energy, time, access, and irreversibility**.

## Integrity

### Generate manifests
When publishing a release, generate SHA-256 for all exported artifacts and store manifests under `hashes/`.  
See `hashes/HOW_TO_HASH.md`.

### Verify (recommended)
**PowerShell (Windows):**
```powershell
# show manifest(s)
Get-ChildItem .\hashes\SHA256SUMS_*.txt | ForEach-Object { "`n== $($_.Name) =="; Get-Content $_.FullName }

# spot-check files (example: all PDFs)
Get-ChildItem .\pdf\*.pdf -ErrorAction SilentlyContinue | ForEach-Object {
  (Get-FileHash $_.FullName -Algorithm SHA256).Hash.ToLower() + "  " + $_.FullName.Replace((Get-Location).Path + "\", "").Replace("\","/")
}
```

## Naming note
AGI = Advanced Global Intelligence (not Artificial General Intelligence).

## Canonical entry
Canonical entry: see AGI `MASTER_ENTRY.md` in `Kot141078/advanced-global-intelligence`.

## Implementation reference
Implementation reference (non-normative): `Kot141078/ester-clean-code`.

## ARQ bridge (canonical in SER)

ARQ (**Anti-Resonance Correction Protocol**) is an additive subsystem in the wider stack, but its canonical home is **not** this repository.

Canonical entry:
`..\sovereign-entity-recursion\protocol\arq\README.md`

From the L4 point of view, ARQ matters because it creates an explicit bridge between correction logic, **SER** continuity, and **L4** bounded accountability.

It also carries two quieter operational consequences:
promotion requires witness-backed traceability, and adaptive handling must remain bounded rather than degrade into infinite retry behavior.

Grounding note:
on real hardware, no classification or retention path is free — there is finite power, finite cooling, finite storage endurance, finite controller trust, finite privilege, and a finite trusted calibration window.

## EA-L4 / EATP (canonical in AGI)

EA-L4 / EATP is an adjacent L4-bound training, provenance, and consequence layer, but its canonical home is **not** this repository.

Canonical entry:
`..\advanced-global-intelligence\protocols\ea-l4-eatp\README.md`

Role from the L4 side:
- training-origin discipline under real constraints
- consequence-preserving public package layer
- adjacent to SER and L4 rather than a replacement for either

Boundary:
- no duplicate package home in this repo
- no claim that EA-L4 / EATP replaces L4 notes here

## DEA (canonical in AGI)

DEA is an adjacent upstream layer that defines when input becomes auditable experience under bounded reality, but its canonical home is **not** this repository.

Canonical entry:
`..\advanced-global-intelligence\protocols\dea\README.md`

Role from the L4 side:
- input-to-experience boundary under real constraints
- upstream from EA-L4 / EATP and downstream witness/evidence handling
- adjacent to SER and L4 rather than a replacement for either

Boundary:
- no duplicate package home in this repo
- no claim that DEA replaces L4 notes here

## Economic Layer and Pre-Lineage (canonical in AGI)

Economic Layer for Experience Artifacts is an adjacent ecosystem material with its canonical home in AGI. From the L4 side it connects through scarcity, scar, irreversibility, bounded disclosure, restraint, and anti-gaming handling rather than through a duplicate local package.

Canonical external package:
- https://github.com/Kot141078/advanced-global-intelligence/tree/main/docs/economic-layer

Pre-Lineage Boundary Note is a reserved cross-stack boundary note, not an ERB operational protocol.

Canonical external note:
- https://github.com/Kot141078/advanced-global-intelligence/blob/main/manifesto/Pre_Lineage_Boundary_Note_v0.1.md

Boundary:
- pointer only in this repo
- no duplicate package home in ERB

---

## Machine entry / downloads (no UI)
- Machine entry (raw):
  https://raw.githubusercontent.com/Kot141078/ester-reality-bound/main/MACHINE_ENTRY.md
- llms.txt (raw):
  https://raw.githubusercontent.com/Kot141078/ester-reality-bound/main/llms.txt
- Tag snapshot ZIP:
  https://github.com/Kot141078/ester-reality-bound/archive/refs/tags/l4-snapshot-2026-02-24.zip
- Verify content via `hashes/` + `SHA256SUMS_*.txt` (do not hash GitHub-generated archives).

## L4 Glitch / Research Quarantine Stack v0.1

This repository now hosts the **normative** and **graph/visibility-facing** side of the glitch-stack package set.

Primary entry:
- [`docs/glitch-stack/INDEX.md`](docs/glitch-stack/INDEX.md)

Subtrees:
- [`docs/glitch-stack/core/`](docs/glitch-stack/core/)
- [`docs/glitch-stack/graph-visibility/`](docs/glitch-stack/graph-visibility/)

The markdown files remain the canonical working layer.
The PDF files remain the packaged reader-facing layer.

## Ecosystem-wide theoretical synthesis

For an ecosystem-wide theoretical synthesis, see:

- `Kot141078/advanced-global-intelligence` -> `manifesto/Theoretical_Foundations_of_the_AGI_Ecosystem_EN.md`

This repository remains the public L4 / reality-bound layer rather than the home of the ecosystem-wide synthesis.

### Published citation

For the published ecosystem-wide theoretical synthesis record, see:

- Version DOI: [10.5281/zenodo.19384668](https://doi.org/10.5281/zenodo.19384668)
- All versions DOI: [10.5281/zenodo.19384667](https://doi.org/10.5281/zenodo.19384667)

### Published Zenodo records for the glitch-stack normative / visibility side

- Core Specification v0.1 — version DOI: [10.5281/zenodo.19385784](https://doi.org/10.5281/zenodo.19385784), all versions: [10.5281/zenodo.19385783](https://doi.org/10.5281/zenodo.19385783)
- Graph Grammar and Visibility Layer v0.1 — version DOI: [10.5281/zenodo.19385908](https://doi.org/10.5281/zenodo.19385908), all versions: [10.5281/zenodo.19385907](https://doi.org/10.5281/zenodo.19385907)

### Arbitration / Review Layer (ARL) v0.1

ARL v0.1 is the procedural bridge between dispute and operational containment: freeze, hold, quarantine, witness binding, and lawful re-entry discipline.

Canonical home: `sovereign-entity-recursion` ARL package

The Reality Boundary layer already formalizes collision, scarcity, freeze pressure, and witness-backed traceability. ARL v0.1 extends this operational discipline into the dispute domain: when standing exists and admissible conflict is recognized, the system does not improvise. It freezes, classifies, reviews, and determines whether a disputed branch may lawfully re-enter flow.
