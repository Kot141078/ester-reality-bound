# Graph Rendering Conventions / Visual Notation Concept v0.1

**Status:** Concept Draft  
**Scope:** Rendering discipline for the `L4 Glitch Map -> Research/Backward Node -> Cinematic Walkthrough` triad  
**Intent:** Define a visual language in which architectural status, authority, quarantine, and witness state are visible **before** interpretation.

---

## 1. Purpose

The graph must not behave like a decorative diagram.
It must behave like a **constraint-visible notation system**.

Its job is not to make the system look impressive.
Its job is to make the following legible at a glance:

- what is executable,
- what is blocked,
- what is quarantined,
- what is speculative,
- what is witness-backed,
- what is only navigable as cinematic exploration,
- and which transitions are forbidden by architecture.

In other words:

**the graph must show where reality still holds, where it has broken, and what remains only research or visibility.**

---

## 2. Rendering Principles

### 2.1. Status before beauty

A beautiful graph that hides authority state is a failure.
Rendering must privilege architectural truth over visual elegance.

### 2.2. Visual asymmetry is mandatory

Executable reality, quarantined research, and cinematic visibility must not look equivalent.
If they look equally "alive," the notation fails.

### 2.3. Physics outranks interface

No visual affordance may imply that UI can override L4.
A blocked path must look blocked.
Not merely discouraged.

### 2.4. Witness changes appearance

A node or edge that has been witnessed must be visually distinguishable from one that is only asserted.

### 2.5. Ambiguity must narrow authority

If a node carries unresolved ambiguity, its visual form must signal narrowed legitimacy, reduced execution scope, or quarantine.

---

## 3. Rendering Lanes

The graph is rendered in three primary lanes.

### 3.1. Core Lane

**Meaning:** Reality-bound execution space  
**Contains:** `CoreActionNode`, `ConstraintNode`, `GlitchNode`, verified authority transitions  
**Authority:** Non-zero  
**Color family:** Deep green / steel / hard blue-green  
**Texture:** Dense, solid, low-gloss  
**Interpretation:** This lane binds consequence.

### 3.2. Research Lane

**Meaning:** Quarantined possibility space  
**Contains:** `ResearchNode`, `BackwardNode`, speculative bridge candidates, unresolved requirements  
**Authority:** Zero by default  
**Color family:** Gray / muted amber / desaturated violet accents for unresolved research class  
**Texture:** Dashed, porous, skeletal  
**Interpretation:** This lane preserves possibility but cannot authorize execution.

### 3.3. Walkthrough Lane

**Meaning:** Navigable explanatory / cinematic visibility  
**Contains:** `WalkthroughFrame`, `InspectView`, branch summaries, path projection overlays  
**Authority:** Read-only  
**Color family:** Soft white / low-saturation blue / translucent overlays  
**Texture:** Thin, projected, luminous, non-load-bearing  
**Interpretation:** This lane explains; it does not decide.

---

## 4. Canonical Node Shapes

### 4.1. CoreActionNode

**Shape:** solid rectangle with slightly rounded corners  
**Reason:** operational, bounded, non-mythic  
**Visual cue:** heavy outline

### 4.2. ConstraintNode

**Shape:** hexagon  
**Reason:** structural gate / condition / hard limit  
**Visual cue:** rigid geometry, no glow

### 4.3. GlitchNode

**Shape:** fractured hexagon or split diamond  
**Reason:** collision between intended path and L4 reality  
**Visual cue:** visible discontinuity line through shape

### 4.4. ResearchNode

**Shape:** hollow circle with interrupted perimeter  
**Reason:** preserved but incomplete object  
**Visual cue:** internal emptiness, no fill

### 4.5. BackwardNode

**Shape:** target-like circle with reverse arrow marker  
**Reason:** desired future state that points backward to missing bridge  
**Visual cue:** directional back-reference symbol

### 4.6. WitnessNode / WitnessEvent marker

**Shape:** sealed badge / small square seal / cryptographic stamp attached to node or edge  
**Reason:** not a separate speculative object, but a proof-bearing state change  
**Visual cue:** high-contrast seal with timestamp slot

### 4.7. WalkthroughFrame

**Shape:** translucent panel / thin card / frame bracket  
**Reason:** this is a viewpoint, not a causal object  
**Visual cue:** floating appearance, low visual mass

---

## 5. Canonical Edge Types

### 5.1. Execute edge

**Meaning:** real permitted transition in core lane  
**Style:** solid thick line  
**Color:** dark green / steel  
**Arrow:** strong directional arrowhead

### 5.2. Constraint-hit edge

**Meaning:** path terminated by L4 constraint  
**Style:** solid line ending in hard stop bar  
**Color:** red-brown / hazard accent  
**Arrow:** none after stop marker

### 5.3. Quarantine edge

**Meaning:** `GlitchNode -> ResearchNode` wrapping transition  
**Style:** dashed line with containment brackets  
**Color:** muted gray  
**Arrow:** one-way into quarantine only

### 5.4. Reopenable edge

**Meaning:** research object may re-enter evaluation if evidence appears  
**Style:** dashed line with witness slot marker  
**Color:** amber-gray  
**Arrow:** conditional arrowhead with lock icon

### 5.5. Witness edge

**Meaning:** proof-backed transition or authorization event  
**Style:** thin hard line with seal marker(s)  
**Color:** black / dark indigo accent  
**Arrow:** explicit signed transition marker

### 5.6. Inspect edge

**Meaning:** user/viewer navigates to inspect state  
**Style:** thin dotted line  
**Color:** pale blue / neutral light  
**Arrow:** soft pointer

### 5.7. Forbidden edge

**Meaning:** architecturally impossible transition  
**Style:** broken red line with large cross-bar or no-render policy  
**Color:** saturated red  
**Arrow:** absent  
**Rule:** whenever possible, forbidden edges should be shown only as ghosted impossibilities, not as active selectable paths.

---

## 6. Core Color Semantics

### 6.1. Green family = bounded execution

Not "success" in a motivational sense.
It means: this path is still inside executable architecture.

### 6.2. Gray family = preserved but non-legitimate

Not failure.
Not deletion.
It means: stored, visible, non-authoritative.

### 6.3. Amber = conditional / evidence pending

Means: neither dead nor valid.
Requires external proof, privilege expansion, or new state.

### 6.4. Red = hard collision with L4

Means: architecture stopped the path.
Not moral disapproval.
A real limit was reached.

### 6.5. Blue-white translucency = cinematic view only

Means: readable / inspectable / narratable.
Not load-bearing.

---

## 7. Texture and Weight Semantics

Because color alone is fragile, texture and line weight must carry status too.

- **Solid + thick** = executable / authoritative
- **Dashed + medium** = quarantined or conditional
- **Dotted + thin** = inspect-only
- **Fractured border** = reality collision
- **Hollow node** = zero authority preserved object
- **Stamped seal** = witness-backed state
- **Glow** must never mean authority; at most it may mean navigational emphasis

This prevents aesthetic laundering through color grading alone.

---

## 8. Labeling Conventions

Every rendered node should expose, at minimum, the following compact label set:

- `TYPE`
- `STATUS`
- `AUTHORITY_WEIGHT`
- `L4_CLASS` (if applicable)
- `WITNESS_STATE`
- `REVISION` or `HASH_SHORT`

Example:

```text
TYPE: GLITCH
STATUS: HARD_STOP
AUTHORITY_WEIGHT: 1 -> 0
L4_CLASS: THERMAL_LOCK
WITNESS: PENDING
HASH: a91f
```

For research objects:

```text
TYPE: BACKWARD_NODE
STATUS: QUARANTINED
AUTHORITY_WEIGHT: 0
MISSING: EVIDENCE + PRIVILEGE
WITNESS: NONE
HASH: b72c
```

The graph should allow both **compact labels** and **expanded side-panels**, but compact labels must remain truthful on their own.

---

## 9. Red-Line Rendering Rules

### 9.1. Research may not visually impersonate execution

Research lane nodes may not use the same fill density, line thickness, or color dominance as core execution nodes.

### 9.2. Cinematic views may not visually imply commit capability

Frames, overlays, and path previews must remain translucent and non-load-bearing.
Anything clickable toward execution must first pass through visible architectural gates.

### 9.3. Witness may not be hidden in metadata only

If a path is witness-backed, the seal must be visually present.
If it is not witness-backed, the absence must also be visible.

### 9.4. Forbidden transitions must not be rendered as tempting continuations

No smooth animated continuation beyond a hard L4 stop.
The stop must look categorical.

### 9.5. UI emphasis must not outrank authority state

A selected node may become more noticeable, but not more legitimate.
Selection is not authorization.

---

## 10. Minimal Legend

Every graph view should include a fixed legend with at least:

- solid green edge = executable
- fractured node = L4 glitch
- hollow gray node = quarantined research
- stamped marker = witness-backed
- pale translucent frame = cinematic walkthrough only
- red ghost edge = forbidden transition

A viewer should be able to misunderstand the scenario content and still correctly understand the **authority topology**.

---

## 11. Suggested Screen Composition

### 11.1. Left-to-right mode

- left = origin / previous stable state
- center = current collision / inspection focus
- right = allowed next paths and quarantined forks

### 11.2. Top-to-bottom lane mode

- top = core lane
- middle = research lane
- bottom = cinematic lane

This makes it visually obvious that explanatory visibility sits beneath consequence-bearing execution.

### 11.3. Overlay discipline

Walkthrough overlays must never fully obscure core node state.
If explanation covers reality state, rendering has failed.

---

## 12. Minimal Example

```text
[CoreActionNode: CALL_ORACLE]
   |
   | execute
   v
[ConstraintNode: TOKEN_BUDGET]
   |
   | constraint-hit
   v
[GlitchNode: ENERGY_LOCK]
   |
   | quarantine
   v
[ResearchNode: ALT_INFERENCE_PATH]
   |
   | backward-specifies
   v
[BackwardNode: NEED_LOCAL_MODEL_X]

[WalkthroughFrame] --inspect--> [GlitchNode]
[WalkthroughFrame] --inspect--> [ResearchNode]

(forbidden)
[ResearchNode] -X-> [CoreActionNode]
```

Rendered correctly, the viewer should instantly see:

- execution happened,
- reality stopped it,
- possibility was preserved,
- visibility remains open,
- authority did not travel with speculation.

---

## 13. Relationship to the Existing Triad

### 13.1. `L4 Glitch Map`
Provides the factual collision object.

### 13.2. `Research / Backward Node`
Provides the preserved research structure.

### 13.3. `Cinematic Walkthrough Layer`
Provides inspection and explanatory navigation.

### 13.4. Rendering Conventions
Provide the **visual truth discipline** that prevents these layers from collapsing into one another.

Without rendering discipline, the stack can still exist logically while appearing misleadingly monolithic.

---

## 14. Explicit Bridge

The explicit bridge remains:

**reality collision -> preserved research -> bounded visibility**

Rendering conventions do not invent this bridge.
They make it legible.

---

## 15. Hidden Bridges

### Hidden bridge 1: cybernetics

A control system fails when signal and control state are visually indistinguishable.
Graph notation is therefore part of regulation, not mere presentation.

### Hidden bridge 2: information theory

Compressed notation must preserve the most load-bearing distinctions.
If visual compression erases authority state, the graph increases entropy instead of reducing it.

---

## 16. Earth Paragraph

In an electrical cabinet, cable color, breaker shape, warning marks, and isolation labels are not decorative. They prevent the wrong hand from treating a live line as if it were harmless. The same applies here. If a quarantined speculative branch is rendered like an executable one, the diagram becomes not a map, but a hazard. Good notation is a safety device.

---

## 17. Closing Note

This layer does not add new ontology.
It adds disciplined visibility.

A serious graph must allow a viewer to answer, in one glance:

- what is real,
- what is broken,
- what is preserved,
- what is provable,
- and what is only being shown.

That is the minimum visual grammar for an architecture that claims to respect L4.
