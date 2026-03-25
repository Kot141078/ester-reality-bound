[![DOI](https://zenodo.org/badge/1131456026.svg)](https://doi.org/10.5281/zenodo.18311218)

# Reality-Bound AI (L4) — Notes, Protocol, and Posts

Public-facing materials for a reality-bound approach to AI safety and long-lived AI entities.

## Process Premise

> “The future is not an event. It is a process.”
> — Ivan Kotov

Canonical note: see `Kot141078/advanced-global-intelligence` → `official/AUTHORIAL_PREMISES.md`

## Core distinctions
- **Tools** are stateless and transactional.
- **Entities (c = a + b)** are persistent, contextual, memory-based.
- **Agents** are bounded subordinate processes. By default, they are invoked and governed by `c`; they are not the primary subject.
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

---

## Machine entry / downloads (no UI)
- Machine entry (raw):
  https://raw.githubusercontent.com/Kot141078/ester-reality-bound/main/MACHINE_ENTRY.md
- llms.txt (raw):
  https://raw.githubusercontent.com/Kot141078/ester-reality-bound/main/llms.txt
- Tag snapshot ZIP:
  https://github.com/Kot141078/ester-reality-bound/archive/refs/tags/l4-snapshot-2026-02-24.zip
- Verify content via `hashes/` + `SHA256SUMS_*.txt` (do not hash GitHub-generated archives).
