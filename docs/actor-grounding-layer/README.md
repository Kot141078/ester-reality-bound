# Actor Grounding Layer (AGL) v0.1
## Package README

**Status:** Draft package v0.1  
**Canonical home:** `ester-reality-bound`  
**Author:** Ivan Kotov  
**Location:** Brussels  
**Year:** 2026

---

## Purpose

This package defines the **Actor Grounding Layer (AGL)** for long-lived systems operating under real constraints.

AGL exists to answer a question that sits **before review** and often **before action**:

> Is the actor, source, perceptual path, or delegated origin sufficiently grounded in real present execution state for the system to rely on it at all?

Without that layer, a system may:
- admit procedurally coherent disputes,
- validate evidence cleanly,
- and even emit witness-bound outcomes,

while still depending on an initiation surface that is too degraded, detached, stale, simulated, overloaded, or operationally ungrounded to support runtime reliance.

AGL is therefore not a decorative refinement.
It is the precondition layer that prevents systems from acting on abstraction while still sounding coherent.

---

## What this package does

AGL v0.1 defines:

- source-state qualification,
- runtime-reliance discipline,
- initiation gates and preconditions,
- degradation signals and fail-closed transitions,
- and the boundary relationship between:
  - physical perimeter,
  - grounding,
  - procedural review,
  - and witness traceability.

In practical terms, this package asks:
- who or what is initiating,
- in what condition,
- through what channel,
- under what local grounding,
- and whether that initiation may lawfully support runtime progression.

---

## What this package is not

AGL is **not**:
- a replacement for ARL,
- a replacement for L4 Witness,
- a replacement for the hardware perimeter,
- a universal theory of consciousness,
- a social scoring system,
- or a post-hoc analytics layer pretending to be control.

AGL does not decide disputes after they exist.
It decides whether some signals, actors, or initiation paths are grounded enough to be relied on **before** or **while** action binds.

---

## Package contents

### Primary documents
- `Executive_Summary_Actor_Grounding_Layer_v0.1.md`
- `Actor_Grounding_Layer_v0.1.md`

### Normative support documents
- `Source_State_Qualification_and_Runtime_Reliance_v0.1.md`
- `Initiation_Gates_and_Preconditions_v0.1.md`
- `Degradation_Signals_and_Fail_Closed_Transitions_v0.1.md`
- `Relationship_to_ARL_L4_Witness_and_Hardware_Perimeter_v0.1.md`

### Package-facing documents
- `README.md`
- `INDEX.md`
- `DOC_MAP.md`

---

## Reading order

Recommended reading order:

1. `Executive_Summary_Actor_Grounding_Layer_v0.1.md`
2. `Actor_Grounding_Layer_v0.1.md`
3. `Source_State_Qualification_and_Runtime_Reliance_v0.1.md`
4. `Initiation_Gates_and_Preconditions_v0.1.md`
5. `Degradation_Signals_and_Fail_Closed_Transitions_v0.1.md`
6. `Relationship_to_ARL_L4_Witness_and_Hardware_Perimeter_v0.1.md`
7. `INDEX.md`
8. `DOC_MAP.md`

---

## Architectural position

AGL sits between:
- **L4 Hardware Perimeter** and present execution reality,
- **runtime initiation surfaces**,
- **ARL procedural review**,
- and **L4 Witness traceability**.

In short:
- the hardware perimeter asks whether the node and room are physically fit to host sensitive action,
- AGL asks whether the source or actor is grounded enough to support runtime reliance,
- ARL asks how conflict is procedurally admitted and resolved,
- L4 Witness asks what can later be proven about what actually happened.

AGL is therefore an upstream gate, not a downstream explanation.

---

## Canonical role of this repository

The canonical home of AGL v0.1 is **`ester-reality-bound`**.

That placement is deliberate.
AGL is closer to:
- reality contact,
- source-state quality,
- operator/sensor grounding,
- present execution state,
- and physical preconditions,

than to procedural dispute doctrine alone.

ARL should consume AGL.
It should not swallow it.

---

## Required bridges

**Explicit bridge:**  
**L4 Hardware Perimeter / present execution state ↔ AGL grounding gate ↔ ARL procedural review ↔ L4 Witness traceability**

**Hidden bridge #1:**  
AGL is the upstream precondition that keeps ARL from reviewing conflicts whose initiation surface was already detached from real present state. In that sense, AGL protects ARL from beginning too late.

**Hidden bridge #2:**  
L4 Witness can prove what happened, but proof does not grant lawful initiation by itself. AGL separates *auditability after the fact* from *grounding before action*, which keeps traceability from masquerading as permission.

---

## Earth paragraph

On a real warehouse floor, you do not wait for a full incident review to notice that the forklift operator is exhausted, the barcode scanner is failing, the pallet tag is stale, and the loading lane is half blocked. You stop the move before it becomes a dispute. Hardware perimeter is the floor and the doors. ARL is the formal review after conflict is admitted. Witness is the ledger. AGL is the moment someone says: this source is not grounded enough to move the load.
