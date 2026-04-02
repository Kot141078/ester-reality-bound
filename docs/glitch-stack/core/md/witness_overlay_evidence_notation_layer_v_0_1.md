# Witness Overlay / Evidence Notation Layer v0.1

**Status:** Concept Draft  
**Scope:** Evidence visibility layer for the Triad Stack (`L4 Glitch Map` -> `Research / Backward Node` -> `Cinematic Walkthrough Layer`)  
**Role:** Visual and semantic overlay for witness discipline, evidentiary status, challengeability, expiry, and non-authority markings  

---

## 1. Purpose

The graph already distinguishes:

- where execution is real,
- where research is quarantined,
- where visibility is cinematic,
- and where reality breaks.

That is not yet enough.

A mature graph must also show **what kind of evidentiary standing** each visible object has.

Without this layer, three dangerous confusions reappear:

1. **assertion is mistaken for proof**
2. **witness is mistaken for authority**
3. **aesthetic coherence is mistaken for validity**

The Witness Overlay exists to prevent those collapses.

It does not add execution power.  
It does not create authority.  
It does not “make a node true.”

It only makes visible:

- what has been observed,
- what has been signed,
- what can still be challenged,
- what has expired,
- and what remains purely cinematic or speculative.

---

## 2. Core Principle

**A node may be visible without being executable.**  
**A node may be witnessed without being authorized.**  
**A node may be signed without being final.**

Therefore the graph needs a separate evidentiary overlay.

This overlay answers:

- What happened?
- Who observed it?
- Under what witness discipline?
- Is it still challengeable?
- Has it expired?
- Does it support action, learning, audit, or only inspection?

---

## 3. Layer Position in the Stack

The Witness Overlay sits **above rendering** and **below interpretation**.

Meaning:

- it annotates visible nodes and edges,
- it does not alter the underlying graph topology,
- it does not grant runtime permissions,
- it does not modify L4 outcomes.

Formal relation:

- `Graph Grammar` defines what objects exist
- `Rendering Conventions` define how objects are drawn
- `Witness Overlay` defines what evidentiary status is attached to what is drawn

---

## 4. Evidence States

Each node or edge may carry one of the following primary evidence states.

### 4.1 `asserted`

The object is present as a claim, proposal, or narrative construct.  
No witness event has been attached.

Meaning:

- visible,
- inspectable,
- non-authoritative,
- non-executable by default.

Typical objects:

- speculative bridge,
- fresh cinematic segment,
- newly proposed research path.

### 4.2 `observed`

The object is linked to an actual event or state transition that was recorded, but not yet cryptographically sealed or fully reviewed.

Meaning:

- grounded enough for inspection,
- still open to reinterpretation,
- not yet robust evidence.

Typical objects:

- raw L4 collision record,
- intermediate witness queue entry,
- machine-side event before envelope finalization.

### 4.3 `witnessed`

The object is bound to a witness event or envelope that confirms it occurred under a defined constraint context.

Meaning:

- reality-linked,
- challengeable,
- reviewable,
- may support audit,
- does not itself imply permission or legitimacy.

Typical objects:

- `GlitchNode` with witness record,
- completed branch failure under L4,
- verified execution stop.

### 4.4 `signed`

The witness record has been sealed under a defined signing discipline.

Meaning:

- strong evidence integrity,
- suitable for cross-system transfer,
- suitable for downstream audit references,
- still not equal to command authority.

Typical objects:

- witness-backed branch outcome,
- signed challenge resolution,
- sealed evidence package.

### 4.5 `challenge_open`

A witness-backed object remains under a valid challenge window.

Meaning:

- not yet settled,
- strong caution in interpretation,
- must not be silently treated as final.

Typical objects:

- controversial branch classification,
- disputed evidence interpretation,
- witness package awaiting review.

### 4.6 `settled`

Challenge window closed or dispute resolved.

Meaning:

- evidentiary interpretation stabilized,
- safe for archival reliance,
- still separate from policy authority.

### 4.7 `expired`

Evidence no longer has current operational standing due to time, context drift, or trust expiry.

Meaning:

- remains historically visible,
- not valid for current decision support,
- not deleted,
- must be rendered as degraded.

### 4.8 `cinematic_only`

The visible object belongs only to representational walkthrough and has no evidentiary standing.

Meaning:

- illustrative only,
- pedagogical only,
- must never be mistaken for proof.

---

## 5. Evidence Roles

Beyond state, evidence may also carry **role tags**.

Examples:

- `runtime_evidence`
- `research_evidence`
- `audit_evidence`
- `learning_candidate`
- `display_only`
- `expired_reference`

These tags help distinguish why an object is being shown.

Example:

A node can be:

- `witnessed + research_evidence`
- `signed + audit_evidence`
- `asserted + display_only`
- `expired + historical_reference`

---

## 6. Visual Notation Rules

The Witness Overlay must be readable at a glance.

### 6.1 Badge Position

Every node may display a small evidence badge in a fixed corner.

Recommended position:

- top-right for nodes,
- center-top or mid-edge marker for edges.

The badge indicates evidence state.

### 6.2 Badge Shape Vocabulary

Suggested mapping:

- `asserted` -> hollow circle
- `observed` -> half-filled circle
- `witnessed` -> solid circle
- `signed` -> solid circle with ring
- `challenge_open` -> solid circle with exclamation mark
- `settled` -> solid circle with check mark
- `expired` -> faded circle with diagonal slash
- `cinematic_only` -> dotted circle

### 6.3 Opacity Grammar

- strong opacity -> current evidence relevance
- reduced opacity -> historical but not current
- ghosted opacity -> cinematic or illustrative only

### 6.4 Edge Treatment

Edges may also be witnessed.

Examples:

- a witnessed transition from execution to glitch,
- a signed transition from glitch to research node,
- a challenge-open edge representing disputed classification.

Use mid-edge markers, not endpoint substitution.

### 6.5 Overlay Color Discipline

Witness Overlay must not override the base graph semantic colors.

Therefore:

- base color continues to indicate lane / ontology
- evidence overlay uses micro-markings, rings, icons, and local texture
- evidence cannot recolor the branch into a false execution class

This prevents the viewer from confusing:

- “green because executable”
with
- “green because strongly witnessed.”

Those are not the same claim.

---

## 7. Challengeability Marking

Challengeability is central.

A witnessed object is not automatically final.

Therefore every evidence-bearing object should expose:

- `challengeable: yes/no`
- `challenge_deadline`
- `challenge_scope`

### 7.1 Visual Convention

Challenge-open items should visibly pulse, blink softly, or carry a warning contour.

Not to dramatize them, but to prevent quiet laundering into certainty.

### 7.2 Settled Convention

Once settled:

- remove pulse,
- preserve witness badge,
- add closure mark,
- retain historical trace of prior challenge state if needed in audit mode.

---

## 8. Expiry and Drift

Evidence is not timeless.

The graph must visually distinguish:

- evidence that still supports current reasoning,
- evidence that only supports historical understanding,
- evidence invalidated by context drift.

### 8.1 Expiry Cases

Examples:

- privilege context changed,
- hardware stack changed,
- time budget window closed,
- witness trust root rotated,
- scenario assumptions no longer hold.

### 8.2 Rendering Rule

Expired evidence remains visible but degraded:

- faded marker,
- dashed frame,
- archive tag,
- unavailable for execution overlays.

Expired evidence must never disappear silently.

Disappearance destroys audit memory.

---

## 9. Read Modes

Different users need different evidentiary densities.

### 9.1 `normal_mode`

Show only:

- key evidence markers,
- challenge-open warnings,
- cinematic-only disclaimers.

### 9.2 `audit_mode`

Show:

- evidence badges,
- witness chains,
- signer info class,
- expiry data,
- challenge windows,
- provenance links.

### 9.3 `pedagogical_mode`

Show:

- simplified evidence categories,
- no cryptographic jargon,
- explicit distinction between:
  - “this happened”
  - “this is under review”
  - “this is only a hypothetical branch.”

---

## 10. Forbidden Collapses

The Witness Overlay must explicitly block the following confusions.

### 10.1 Witness != Authority

A witnessed node may prove that something happened.  
It does not prove that it was legitimate to do.

### 10.2 Signature != Truth

A signed object proves integrity of record.  
It does not prove ontological correctness.

### 10.3 Visibility != Evidence

A cinematic segment can be beautiful, coherent, and persuasive.  
It may still be `cinematic_only`.

### 10.4 Evidence != Execution Permission

Even strongly witnessed objects may remain quarantined.

### 10.5 Expired != Deleted

Expired evidence must remain part of the memory field.

---

## 11. Minimal Data Attachment Schema

Each rendered node or edge may optionally expose:

```json
{
  "evidence_state": "witnessed",
  "evidence_roles": ["runtime_evidence", "audit_evidence"],
  "challengeable": true,
  "challenge_deadline": "2026-04-15T18:00:00Z",
  "settlement_state": "open",
  "expiry_state": "current",
  "witness_ref": "wit_01H...",
  "signed": true,
  "signing_class": "entity_bound",
  "cinematic_only": false
}
```

This schema does not grant runtime power.  
It only informs rendering and interpretation.

---

## 12. Canonical Example

A valid graph slice may read as:

- execution node in green lane
- witnessed edge to red `GlitchNode`
- signed witness badge on glitch
- challenge-open icon on classification
- transition to gray `ResearchNode`
- `ResearchNode` marked `observed + research_evidence`
- cinematic branch extending forward, but marked `cinematic_only`

This shows, in one view:

- what actually happened,
- what is research,
- what is visible only as imagination,
- and what remains under challenge.

---

## 13. Why This Matters

Without evidence notation, a graph can still become dangerous.

It can become:

- visually persuasive,
- ontologically mixed,
- and politically ambiguous.

The Witness Overlay ensures the graph remains:

- epistemically stratified,
- audit-compatible,
- and resistant to aesthetic laundering.

This is especially important in systems where:

- speculation is allowed,
- research branches are valuable,
- cinematic walkthroughs are rich,
- and execution is bounded by L4.

If all those layers are visible but not evidentially separated, the graph becomes a theater of confusion.

---

## 14. Explicit Bridge

This layer makes one principle visible:

**not every visible branch carries the same evidentiary weight.**

That is the bridge between:

- witness discipline,
- research quarantine,
- and long-lived continuity under constraint.

---

## 15. Hidden Bridges

### Hidden Bridge 1 — Information Theory

A graph that does not distinguish evidence classes increases ambiguity and lowers signal.  
Evidence notation compresses trust-relevant information into interpretable visible form.

### Hidden Bridge 2 — Cybernetics

A regulator without stratified feedback cannot maintain control.  
Witness Overlay is a visible feedback stratification layer.

---

## 16. Earth Paragraph

In engineering, a pressure gauge, a signed inspection tag, and a decorative dashboard animation are not the same thing. One tells you what is happening, one tells you who checked it, and one only makes the machine feel modern. A serious AI graph must preserve that difference. Otherwise, a system that only looks accountable will be mistaken for one that actually is.

---

## 17. Final Position

The Witness Overlay / Evidence Notation Layer is not a cosmetic addition.

It is the visible discipline by which the graph refuses to confuse:

- assertion,
- observation,
- witness,
- signature,
- settlement,
- expiry,
- and cinematic illustration.

Without it, the graph may still be beautiful.

But it will not yet be trustworthy.

