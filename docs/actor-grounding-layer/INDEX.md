INDEX — Actor Grounding Layer v0.1

Status: Draft v0.1
Canonical home: ester-reality-bound
Author: Ivan Kotov
Location: Brussels
Year: 2026

1. Package purpose

This package exists to make the Actor Grounding Layer readable, navigable, and non-chaotic.

It separates:

the normative grounding core,
source-state qualification,
initiation gates,
degradation and fail-closed transitions,
layer relationships,
and package-facing integration/publication notes.
2. Primary documents
2.1 Core layer
Executive_Summary_Actor_Grounding_Layer_v0.1.md
Actor_Grounding_Layer_v0.1.md
Source_State_Qualification_and_Runtime_Reliance_v0.1.md
Initiation_Gates_and_Preconditions_v0.1.md
Degradation_Signals_and_Fail_Closed_Transitions_v0.1.md
Relationship_to_ARL_L4_Witness_and_Hardware_Perimeter_v0.1.md
2.2 Package-facing and integration documents
Cross_Repo_Pointers_AGL_v0.1.md
Repository_Integration_Notes_AGL_v0.1.md
Publication_and_Integrity_Notes_AGL_v0.1.md
Consistency_Pass_Notes_AGL_v0.1.md
README.md
INDEX.md
DOC_MAP.md
3. Recommended reading order
3.1 For architecture / logic
README.md
Executive_Summary_Actor_Grounding_Layer_v0.1.md
Actor_Grounding_Layer_v0.1.md
Source_State_Qualification_and_Runtime_Reliance_v0.1.md
Initiation_Gates_and_Preconditions_v0.1.md
Degradation_Signals_and_Fail_Closed_Transitions_v0.1.md
Relationship_to_ARL_L4_Witness_and_Hardware_Perimeter_v0.1.md
3.2 For package / integration / publication discipline
Cross_Repo_Pointers_AGL_v0.1.md
Repository_Integration_Notes_AGL_v0.1.md
Publication_and_Integrity_Notes_AGL_v0.1.md
Consistency_Pass_Notes_AGL_v0.1.md
DOC_MAP.md
4. Interpretation priority

If wording tension appears between documents, interpret in this order:

Actor_Grounding_Layer_v0.1.md
Source_State_Qualification_and_Runtime_Reliance_v0.1.md
Initiation_Gates_and_Preconditions_v0.1.md
Degradation_Signals_and_Fail_Closed_Transitions_v0.1.md
Relationship_to_ARL_L4_Witness_and_Hardware_Perimeter_v0.1.md
package-facing documents

This keeps the package from becoming a pile of equally weighted notes.

5. Explicit bridge

perimeter → grounding → runtime reliance / initiation → ARL / witness adjacency

6. Earth paragraph

If a warehouse keeps the grounding rule in one tab, the stop gate in another, and the relationship to formal review somewhere else, someone still needs an index or the next shift will waste an hour rediscovering the same system. This file is that index.
