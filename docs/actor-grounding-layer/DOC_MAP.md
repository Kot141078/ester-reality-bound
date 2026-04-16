# DOC_MAP — Actor Grounding Layer v0.1
## Canonical document map for the AGL package

**Status:** Draft v0.1  
**Canonical home:** `ester-reality-bound`  
**Author:** Ivan Kotov  
**Location:** Brussels  
**Year:** 2026

---

## 1. Purpose

This file classifies the documents in the Actor Grounding Layer package by role.

Its purpose is to prevent three recurring failures:
- not knowing which file is doctrinal,
- not knowing which file is support,
- and not knowing where AGL ends and ARL / Witness / Hardware Perimeter begin.

---

## 2. Document classes

### 2.1 Core doctrine
These define the main normative meaning of AGL:

- `Executive_Summary_Actor_Grounding_Layer_v0.1.md`
- `Actor_Grounding_Layer_v0.1.md`

### 2.2 Normative support documents
These define the mechanics and implications of the layer:

- `Source_State_Qualification_and_Runtime_Reliance_v0.1.md`
- `Initiation_Gates_and_Preconditions_v0.1.md`
- `Degradation_Signals_and_Fail_Closed_Transitions_v0.1.md`
- `Relationship_to_ARL_L4_Witness_and_Hardware_Perimeter_v0.1.md`

### 2.3 Package-facing documents
These support navigation and package coherence:

- `README.md`
- `INDEX.md`
- `DOC_MAP.md`

---

## 3. What is canonical here and what is not

### 3.1 Canonical here
Canonical here means:
- the public bounded meaning of Actor Grounding Layer v0.1,
- the internal reading order of the AGL package,
- and the role separation between grounding, review, witness, and perimeter.

### 3.2 Not canonical here
Not canonical here:
- the ARL dispute constitution,
- the full L4 Witness evidence standard,
- the full hardware perimeter specification,
- or the ECC implementation pack.

Those remain adjacent but distinct packages.

---

## 4. Recommended reading paths

### 4.1 Architecture / doctrine path
- `README.md`
- `Executive_Summary_Actor_Grounding_Layer_v0.1.md`
- `Actor_Grounding_Layer_v0.1.md`
- `Relationship_to_ARL_L4_Witness_and_Hardware_Perimeter_v0.1.md`

### 4.2 Mechanism path
- `Source_State_Qualification_and_Runtime_Reliance_v0.1.md`
- `Initiation_Gates_and_Preconditions_v0.1.md`
- `Degradation_Signals_and_Fail_Closed_Transitions_v0.1.md`

### 4.3 Boundary / interpretation path
- `Relationship_to_ARL_L4_Witness_and_Hardware_Perimeter_v0.1.md`
- `DOC_MAP.md`
- `INDEX.md`

---

## 5. Interpretation discipline

If a future reader encounters tension between:
- orientation text,
- summary text,
- and normative rule text,

the interpretation order is:

1. `Actor_Grounding_Layer_v0.1.md`
2. `Source_State_Qualification_and_Runtime_Reliance_v0.1.md`
3. `Initiation_Gates_and_Preconditions_v0.1.md`
4. `Degradation_Signals_and_Fail_Closed_Transitions_v0.1.md`
5. `Relationship_to_ARL_L4_Witness_and_Hardware_Perimeter_v0.1.md`
6. package-facing documents

This keeps package-facing clarity from becoming silent doctrine drift.

---

## 6. Canonical package logic

AGL is the layer that keeps a system from confusing:
- visible signal with grounded source,
- provenance with present-state fitness,
- auditability with permission,
- and reviewability with lawful runtime reliance.

That is its whole reason to exist.

---

## 7. Required bridges

**Explicit bridge:**  
**Present execution state / Hardware Perimeter ↔ Actor Grounding Layer ↔ ARL procedural conflict ↔ L4 Witness traceability**

**Hidden bridge #1:**  
AGL is the missing upstream condition that lets ARL stay honest. Without it, ARL can become procedurally elegant while still operating on initiation that was already detached from reality.

**Hidden bridge #2:**  
AGL also protects witness logic from inflation. A signed trace can prove that something happened. It cannot, by itself, prove that the source should have been trusted strongly enough to let it start. That distinction belongs here.

---

## 8. Earth paragraph

In a serious workshop, the lockout tag, the fatigue of the operator, the live state of the machine, the incident review file, and the maintenance log are not thrown into one drawer called “safety.” They are different objects with different jobs. AGL is the part that decides whether the hand on the switch is grounded enough for the switch to matter at all.
