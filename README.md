[![DOI](https://zenodo.org/badge/1131456026.svg)](https://doi.org/10.5281/zenodo.18311218)

# Reality-Bound AI (L4) — Notes, Protocol, and Posts

Public-facing materials for a reality-bound approach to AI safety and long-lived AI entities.

## Core distinctions
- **Tools** are stateless and transactional.
- **Entities (c = a + b)** are persistent, contextual, memory-based.
- Safety is not only **L3 (law / text rules)**.
- Safety must include **L4 (Reality Boundary Layer)**: physics + operational constraints.

## Repository map
- `protocol/` — architectural core (c = a + b, L4, identity, oracle scarcity, failure modes).
- `docs/` — supporting notes (glossary, constraint stack, metaphors, responsibility, minimal presence).
- `posts/` — ready-to-publish posts (Markdown).
- `pdf/` — exported artifacts (layout-fixed copies of selected Markdown).
- `hashes/` — integrity manifests and hashing instructions.

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
