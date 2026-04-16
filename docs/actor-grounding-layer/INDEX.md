# INDEX — Actor Grounding Layer v0.1
## Canonical package index for AGL

**Status:** Draft package map v0.1  
**Canonical home:** `ester-reality-bound`  
**Author:** Ivan Kotov  
**Location:** Brussels  
**Year:** 2026

---

## 1. Package purpose

This package exists to make the **Actor Grounding Layer (AGL)** readable as a bounded public layer rather than a scattered implication inside neighboring documents.

Its role is to define how a system qualifies actors, sources, perceptual paths, and delegated origins before or while runtime reliance becomes possible.

AGL is the layer that says:
not every signal that is visible,
not every source that is syntactically valid,
and not every actor that still “looks okay”
may be allowed to bind consequence.

---

## 2. Primary documents

### 2.1 Entry
1. `Executive_Summary_Actor_Grounding_Layer_v0.1.md`

### 2.2 Normative core
2. `Actor_Grounding_Layer_v0.1.md`

---

## 3. Normative support documents

3. `Source_State_Qualification_and_Runtime_Reliance_v0.1.md`  
   Qualification classes, runtime-reliance force, and commit-time revalidation.

4. `Initiation_Gates_and_Preconditions_v0.1.md`  
   What must be true before action may start at all.

5. `Degradation_Signals_and_Fail_Closed_Transitions_v0.1.md`  
   How grounding loss narrows, freezes, or blocks progression.

6. `Relationship_to_ARL_L4_Witness_and_Hardware_Perimeter_v0.1.md`  
   Layer separation and cross-layer boundary map.

---

## 4. Package-facing documents

7. `README.md`  
8. `INDEX.md`  
9. `DOC_MAP.md`

---

## 5. Recommended reading order

### 5.1 Fast path
1. `Executive_Summary_Actor_Grounding_Layer_v0.1.md`
2. `Actor_Grounding_Layer_v0.1.md`
3. `Relationship_to_ARL_L4_Witness_and_Hardware_Perimeter_v0.1.md`

### 5.2 Full path
1. `README.md`
2. `Executive_Summary_Actor_Grounding_Layer_v0.1.md`
3. `Actor_Grounding_Layer_v0.1.md`
4. `Source_State_Qualification_and_Runtime_Reliance_v0.1.md`
5. `Initiation_Gates_and_Preconditions_v0.1.md`
6. `Degradation_Signals_and_Fail_Closed_Transitions_v0.1.md`
7. `Relationship_to_ARL_L4_Witness_and_Hardware_Perimeter_v0.1.md`
8. `DOC_MAP.md`

### 5.3 Implementation-facing reading path
1. `Actor_Grounding_Layer_v0.1.md`
2. `Initiation_Gates_and_Preconditions_v0.1.md`
3. `Source_State_Qualification_and_Runtime_Reliance_v0.1.md`
4. `Degradation_Signals_and_Fail_Closed_Transitions_v0.1.md`
5. `Relationship_to_ARL_L4_Witness_and_Hardware_Perimeter_v0.1.md`

---

## 6. Interpretation priority

If wording tension appears between files, interpret in this order:

1. `Actor_Grounding_Layer_v0.1.md`
2. `Source_State_Qualification_and_Runtime_Reliance_v0.1.md`
3. `Initiation_Gates_and_Preconditions_v0.1.md`
4. `Degradation_Signals_and_Fail_Closed_Transitions_v0.1.md`
5. `Relationship_to_ARL_L4_Witness_and_Hardware_Perimeter_v0.1.md`
6. package-facing documents

This preserves the difference between doctrine and orientation.

---

## 7. Canonical package logic

AGL v0.1 answers one bounded question:

> Before a system relies on a source strongly enough to move runtime, is that source, actor, or initiation path grounded in real present execution state sufficiently enough to support lawful progression at all?

That is the package center.
It is upstream to review.
It is upstream to witness proof.
It is upstream to confident fluent continuation.

---

## 8. Required bridges

**Explicit bridge:**  
**Hardware Perimeter ↔ AGL ↔ ARL ↔ L4 Witness**

**Hidden bridge #1:**  
AGL prevents a familiar architectural lie: treating “admissible dispute review” as if it also solved whether the originating actor or signal was grounded enough to support runtime reliance in the first place.

**Hidden bridge #2:**  
AGL also prevents a second lie: treating witness traceability as if “provable later” automatically meant “lawful to trust now.” It restores the missing distinction between proof and grounding.

---

## 9. Earth paragraph

In a hospital, the incident review board, the audit log, the room checklist, and the moment a nurse refuses to administer something because the patient identity, current state, or channel is wrong are not the same layer. They are adjacent and all necessary. AGL is that refusal moment made architectural: not yet a dispute, not yet a report, but already a boundary.
