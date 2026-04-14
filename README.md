[![DOI](https://zenodo.org/badge/1131456026.svg)](https://doi.org/10.5281/zenodo.18311218)

# Reality-Bound AI (L4) — Notes, Protocol, and Posts

Role:
reality-bound operational layer / `L4` feasibility, perimeter, witness-friendly constraints, and real-world boundary discipline.

Public-facing materials for a reality-bound approach to AI safety and long-lived AI entities.

## Corpus position

This repo is not the canonical home of the whole corpus.
It does not replace AGI framing or SER continuity.

Next hop:

- corpus entry: `Kot141078/advanced-global-intelligence` -> `CORPUS_PRIMER.json`
- anti-confusion surface: `Kot141078/advanced-global-intelligence` -> `CANONICAL_DISTINCTIONS.md`
- public objections/replies surface: `Kot141078/advanced-global-intelligence` -> `OBJECTIONS_AND_REPLIES.md`
- citation / verification surface: `Kot141078/advanced-global-intelligence` -> `CITATION_AND_VERIFICATION.md`
- claims / evidence crosswalk: `Kot141078/advanced-global-intelligence` -> `CLAIMS_AND_EVIDENCE_MAP.md`
- status / maturity map: `Kot141078/advanced-global-intelligence` -> `STATUS_AND_MATURITY_MAP.md`
- audience / minimal-reading surface: `Kot141078/advanced-global-intelligence` -> `AUDIENCE_PROFILES_AND_MINIMAL_READING_PATHS.md`
- corpus sync discipline: `Kot141078/advanced-global-intelligence` -> `CHANGE_CONTROL_AND_SYNC.md`
- corpus supersession / deprecation discipline: `Kot141078/advanced-global-intelligence` -> `SUPERSESSION_AND_DEPRECATION.md`
- corpus terminology / alias policy: `Kot141078/advanced-global-intelligence` -> `TERMINOLOGY_AND_ALIAS_POLICY.md`
- corpus acceptance / regression discipline: `Kot141078/advanced-global-intelligence` -> `ENTRY_ACCEPTANCE_AND_REGRESSION.md`
- corpus assertion-strength / reading-boundary discipline: `Kot141078/advanced-global-intelligence` -> `ASSERTION_STRENGTH_AND_BOUNDARIES.md`
- canonical ownership / package-home discipline: `Kot141078/advanced-global-intelligence` -> `CANONICAL_OWNERSHIP_AND_BOUNDARIES.md`
- cross-layer invariant / contradiction discipline: `Kot141078/advanced-global-intelligence` -> `CROSS_LAYER_INVARIANTS_AND_CONTRADICTION_POLICY.md`
- corpus precedence / resolution discipline: `Kot141078/advanced-global-intelligence` -> `PRECEDENCE_AND_RESOLUTION.md`
- stable artifact ID / reference discipline: `Kot141078/advanced-global-intelligence` -> `ARTIFACT_ID_AND_REFERENCE_POLICY.md`
- package intake / integration discipline: `Kot141078/advanced-global-intelligence` -> `PACKAGE_INTAKE_AND_INTEGRATION.md`
- normative stack: `Kot141078/sovereign-entity-recursion`
- runtime layer: `Kot141078/ester-clean-code`

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
Get-ChildItem ./hashes/SHA256SUMS_*.txt | ForEach-Object { "`n== $($_.Name) =="; Get-Content $_.FullName }

# spot-check files (example: all PDFs)
Get-ChildItem ./pdf/*.pdf -ErrorAction SilentlyContinue | ForEach-Object {
  (Get-FileHash $_.FullName -Algorithm SHA256).Hash.ToLower() + "  " + $_.FullName.Replace((Get-Location).Path + "\", "").Replace("\","/")
}
```

## Naming note
AGI = Advanced Global Intelligence (not Artificial General Intelligence).

## Canonical entry
Canonical entry: see AGI `MASTER_ENTRY.md` in `Kot141078/advanced-global-intelligence`.

## Implementation reference
Implementation reference (non-normative): `Kot141078/ester-clean-code`.

## ARQ v0.2 bridge (canonical in SER)

ARQ (**Anti-Resonance Correction Protocol**) remains an adjacent protocol layer for ERB readers, but its canonical home is **not** this repository.

Canonical home:
- repo: `Kot141078/sovereign-entity-recursion`
- markdown package: `protocol/arq/v0.2/`
- pdf package: `pdf/arq/v0.2/`
- package manifest: `hashes/SHA256SUMS_ARQ_Supplement_v0.2.txt`
- minimal L4-facing first hop:
  - `https://github.com/Kot141078/sovereign-entity-recursion/blob/main/protocol/arq/v0.2/README_ARQ_Supplement_v0.2.md`
  - `https://github.com/Kot141078/sovereign-entity-recursion/blob/main/protocol/arq/v0.2/ARQ_v0.2_Executive_Summary.md`
  - `https://github.com/Kot141078/sovereign-entity-recursion/blob/main/protocol/arq/v0.2/ARQ_Integration_Map_to_SER_L4_Witness_Beacon_VXCX_v0.2.md`
  - `https://github.com/Kot141078/sovereign-entity-recursion/blob/main/protocol/arq/v0.2/ARQ_Failure_Modes_and_Safe_Degradation_v0.2.md`

From the L4 point of view, ARQ matters here as an adjacent layer for bounded degradation, witness-bound memory promotion, and the integration boundary between correction logic, **SER** continuity, and **L4** bounded accountability.

## EA-L4 / EATP (canonical in AGI)

EA-L4 / EATP is an adjacent L4-bound training, provenance, and consequence layer, but its canonical home is **not** this repository.

Canonical entry:
`https://github.com/Kot141078/advanced-global-intelligence/blob/main/protocols/ea-l4-eatp/README.md`

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
`https://github.com/Kot141078/advanced-global-intelligence/blob/main/protocols/dea/README.md`

Role from the L4 side:
- input-to-experience boundary under real constraints
- upstream from EA-L4 / EATP and downstream witness/evidence handling
- adjacent to SER and L4 rather than a replacement for either

Boundary:
- no duplicate package home in this repo
- no claim that DEA replaces L4 notes here

## Continuity Bundle / Cold Wake v0.1 (canonical in AGI)

Continuity Bundle / Cold Wake v0.1 is a cross-layer package with canonical home in AGI rather than in this repository.

Canonical entry:
`https://github.com/Kot141078/advanced-global-intelligence/blob/main/protocols/continuity-bundle/README.md`

Role from the L4 side:
- temporal suspension under storage decay, interface drift, dependency rot, and budget limits
- cold wake must remain fail-closed
- no blind motor reattachment or open privilege restore

Boundary:
- companion to SER continuity and L4 wake constraints; not a replacement
- no duplicate package home in this repo

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

## Related public work

A separate public repository by the same author preserves the multilingual reading editions of *Qubit of Hope — Volume I*:

- `Kot141078/qubit-of-hope-volume-i`

This is a literary repository and is linked here only as related public work.
