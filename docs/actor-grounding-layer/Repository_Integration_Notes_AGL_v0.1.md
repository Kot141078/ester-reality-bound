# Repository Integration Notes — AGL v0.1
## Integration-facing notes for canonical placement and discoverability

**Package:** Actor Grounding Layer v0.1  
**Short name:** AGL v0.1  
**Canonical home:** `ester-reality-bound`  
**Author:** Ivan Kotov  
**Location:** Brussels  
**Year:** 2026  

---

## 1. Purpose

This document defines the intended repository-level integration strategy for the AGL package.

It answers four practical questions:

1. where the package must live canonically,
2. how it should be surfaced inside the host repository,
3. how adjacent repositories should reference it without duplicating it,
4. and what minimum conditions must be satisfied before the package can be treated as integrated.

This file is integration-facing.
It does not replace the normative core.

---

## 2. Canonical repository rule

The canonical repository home of AGL v0.1 is:

`ester-reality-bound`

AGL belongs here because it is a layer about:
- real present execution state,
- source qualification,
- perceptual and actor grounding,
- physical / operational preconditions,
- fail-closed gating before action,
- and upstream reality discipline prior to dispute review.

AGL is therefore closer to L4 / reality-bound materials than to:
- AGI framing,
- SER procedural arbitration,
- or executable implementation code.

---

## 3. Canonical placement rule

### 3.1 Required path

Recommended canonical placement:

```text
docs/
  actor-grounding-layer/

3.2 Required package contents

The following files belong to the package:

README.md
INDEX.md
DOC_MAP.md
Executive_Summary_Actor_Grounding_Layer_v0.1.md
Actor_Grounding_Layer_v0.1.md
Source_State_Qualification_and_Runtime_Reliance_v0.1.md
Initiation_Gates_and_Preconditions_v0.1.md
Degradation_Signals_and_Fail_Closed_Transitions_v0.1.md
Relationship_to_ARL_L4_Witness_and_Hardware_Perimeter_v0.1.md
Cross_Repo_Pointers_AGL_v0.1.md
Repository_Integration_Notes_AGL_v0.1.md
Publication_and_Integrity_Notes_AGL_v0.1.md
Consistency_Pass_Notes_AGL_v0.1.md
3.3 Optional but strongly recommended package subdirectories
pdf/
hashes/

The package should eventually produce:

one PDF for each canonical human-facing/core document that exists as PDF,
one SHA-256 manifest for the package.
4. Discoverability rule

A package is not discoverable merely because it exists in a branch or by direct file link.

For AGL to be treated as properly integrated, an ordinary reader entering the default branch
must be able to find it without insider knowledge.

This means discoverability must be checked from the perspective of:

a first-time human reader,
a reviewer entering through the repo homepage,
and a crawler reading the default branch only.

AGL must therefore be surfaced through visible entry documents,
not hidden as a silent subtree.

5. Required repository-level surfacing
5.1 README-level visibility

The repository README should contain a short visible pointer stating that
a canonical Actor Grounding Layer now exists in the L4 / reality-bound stack.

5.2 docs/index.md visibility

If the host repository already uses docs/index.md as a visible documentation path,
AGL should be listed there explicitly.

5.3 MACHINE_ENTRY visibility

If MACHINE_ENTRY.md already carries obvious package/path entries,
AGL may be added there in the same style, without inventing a new schema.

5.4 No hidden integration

It is not sufficient to:

place files in a branch,
expose them only through pdf/,
or rely on deep direct links.

The package must be visible from the ordinary reading path.

6. Adjacent repository reference rule

AGL should be referenced from adjacent repositories only through short canonical pointers.

6.1 advanced-global-intelligence

Role:

context layer,
framing layer,
high-level stack coherence.

Permitted reference:

a short statement that the stack now includes an upstream grounding layer,
a pointer to the canonical home in ester-reality-bound.

Not permitted:

a duplicate mini-AGL package,
a competing normative summary that drifts from ERB.
6.2 sovereign-entity-recursion

Role:

normative procedural conflict layer,
ARL standing / admissibility / review discipline.

Permitted reference:

a bridge note clarifying that AGL sits upstream of ARL review.

Not permitted:

relocating the grounding layer into SER as if SER were its canonical home.
6.3 ester-clean-code

Role:

implementation-facing bridge,
future gate / hook / runtime-target surfaces.

Permitted reference:

implementation-facing note only.

Not permitted:

turning executable code into the canonical normative source.
7. Minimal integration proof

AGL v0.1 may be considered minimally integrated only if all of the following are true:

the full Markdown package exists in the canonical path,
the repository default branch exposes at least one visible pointer to AGL,
README.md and INDEX.md inside the package are present,
package-facing map documents are present (DOC_MAP, Repository Integration Notes),
the package does not exist as competing normative copies in adjacent repositories.

Strongly recommended but not yet mandatory for minimal integration:

PDFs,
SHA-256 manifest,
cross-repo pointer files committed in visible locations,
release note or changelog mention.
8. Integration sequence (recommended)
8.1 Stage 1 — Text layer

Commit the Markdown package first.

8.2 Stage 2 — Visibility layer

Update host-repo entry surfaces:

README,
docs/index.md,
MACHINE_ENTRY if obvious.
8.3 Stage 3 — Artifact layer

Generate:

PDFs,
SHA-256 manifest,
package-level integrity references.
8.4 Stage 4 — Cross-repo bridge layer

Add short canonical pointers in:

AGI,
SER,
ECC.
9. Anti-fragmentation rule

AGL must not be integrated in a way that creates multiple quasi-canonical homes.

The canonical rule is simple:

one normative home,
many short pointers,
zero competing rulebooks.

10. Explicit bridge

L4 Hardware Perimeter ↔ Actor Grounding Layer ↔ ARL / runtime reliance

11. Hidden bridges
pre-admissibility / standing discipline
L4 Witness traceability without substituting for grounding
12. Earth paragraph

On a real warehouse floor, a grounding rule that determines whether the badge, the operator, the channel, or the live state is trustworthy cannot live partly in one binder, partly in another, and partly in people’s heads. Repository integration plays the same role here: it makes the layer visible where it belongs, instead of letting it dissolve into folklore.
