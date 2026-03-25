# Evidence Pack (Minimal)

This folder contains reproducible templates to document an L4 room/node perimeter.
Goal: allow any reviewer to replicate the format without needing private code.

## How To Use

1. Copy templates and fill them for your node/room.
2. Produce a snapshot JSON (`perimeter_snapshot.json`).
3. For any change, add a change JSON (`perimeter_change.json`).
4. Keep everything local and share only redacted packs when needed.

## A/B Rule

- Section A is strict: minimal, testable, boring.
- Section B is optional: notes and reasoning.

## Bridges

Explicit bridge (`c = a + b`):
- `a` is accountable operator responsibility.
- `b` is evidence procedure + hashes + perimeter records.
- `c` is a checkable perimeter claim.

Hidden bridge #1 (Ashby):
- Perimeter variety requires matching control variety in the checklist and change log.

Hidden bridge #2 (Cover and Thomas):
- SHA-256 manifests compress trust into short checkable strings.

## Earth Paragraph

Perimeter evidence works like engineering maintenance logs:
Without dated snapshots and hashes, failures become stories instead of procedures.

## ARQ Reference (External Canonical)

- Canonical entry: `..\sovereign-entity-recursion\protocol\arq\README.md`
- Explicit bridge: correction logic -> SER continuity -> L4 bounded accountability
- Hidden bridges: witness-backed promotion for any retained deviation; bounded homeostasis rather than infinite retry
- Grounding: finite power, cooling, storage endurance, privilege, controller trust, and calibration trust window constrain whether any promoted event remains valid
