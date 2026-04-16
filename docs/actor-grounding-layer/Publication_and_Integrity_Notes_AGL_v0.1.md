Publication and Integrity Notes — AGL v0.1
Publication-facing and integrity-facing notes for the AGL package

Package: Actor Grounding Layer v0.1
Short name: AGL v0.1
Canonical home: ester-reality-bound
Author: Ivan Kotov
Location: Brussels
Year: 2026

1. Purpose

This document defines the minimum publication-facing and integrity-facing requirements
for the AGL package.

It answers four practical questions:

which artifacts must exist for the package to be publication-ready,
how the integrity contour of the package should be represented,
what minimum evidence is required to treat the package as a stable public object,
and which publication shortcuts must be avoided.

This document is publication-facing.
It does not replace the normative content of the package.

2. Publication principle

AGL v0.1 should not remain only a working text cluster.

To become a stable object in the public corpus, it must exist in a form that is:

readable by humans,
stable across time,
checkable without private trust,
citable as a package,
and discoverable from the canonical repository path.

Publication therefore means:

the package has a readable surface,
the package has an integrity surface,
and the package can be checked as an object rather than merely described.
3. Minimum Markdown package

Before any PDF or hash layer is created, the package MUST already contain the full canonical Markdown layer.

Minimum required Markdown artifacts:

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

If this Markdown layer is incomplete, the package is not publication-ready.

4. PDF contour
4.1 Purpose of the PDF layer

The PDF layer exists to provide:

a stable reading surface,
a printable review surface,
a frozen human-facing representation,
and a publication-ready citation object.
4.2 Recommended PDF set

The following PDFs are recommended for AGL v0.1:

Executive_Summary_Actor_Grounding_Layer_v0.1.pdf
Actor_Grounding_Layer_v0.1.pdf
Source_State_Qualification_and_Runtime_Reliance_v0.1.pdf
Initiation_Gates_and_Preconditions_v0.1.pdf
Degradation_Signals_and_Fail_Closed_Transitions_v0.1.pdf
Relationship_to_ARL_L4_Witness_and_Hardware_Perimeter_v0.1.pdf

Optional but useful PDFs:

DOC_MAP.pdf
Cross_Repo_Pointers_AGL_v0.1.pdf
Repository_Integration_Notes_AGL_v0.1.pdf
Publication_and_Integrity_Notes_AGL_v0.1.pdf
Consistency_Pass_Notes_AGL_v0.1.pdf
4.3 PDF rule

The PDF layer must not silently diverge from the Markdown source.
If typography or layout is improved, content must remain materially unchanged.

5. Integrity contour
5.1 Purpose

The integrity contour exists so that the package can be verified without narrative trust.

5.2 Minimum integrity artifact

Recommended package-level integrity file:

SHA256SUMS_actor_grounding_layer_v0.1.txt

This manifest should contain SHA-256 hashes for:

all canonical Markdown files,
all canonical PDFs that exist in the package publication surface.
5.3 Naming discipline

Use a stable explicit name.
Avoid vague names such as:

hashes.txt
checksums.txt
sha.txt
6. Publication-ready conditions

AGL v0.1 may be treated as publication-ready only if all of the following are true:

the full canonical Markdown package exists,
the canonical repository path is defined,
the package is discoverable from the default branch,
the core PDF layer exists,
the package-level SHA-256 manifest exists,
the package does not rely on oral explanation for interpretation,
the package has a visible package facade (README, INDEX, DOC_MAP),
the package has at least one stable human-facing entry object (Executive Summary PDF).
7. Anti-shortcut rules

The following publication shortcuts should be explicitly avoided.

7.1 PDF-only publication

Publishing only PDFs without the source Markdown weakens future maintenance.

7.2 Markdown-only publication

Leaving the package only as Markdown weakens the frozen public surface.

7.3 Hashless publication

Publishing without a package-level hash manifest invites silent drift.

7.4 Branch-only publication

If the package exists only in a non-default branch or via direct file link,
it is not properly discoverable.

7.5 Cross-repo duplication

If AGL is restated as competing normative summaries in multiple repositories,
publication creates ambiguity rather than clarity.

8. Publication sequence (recommended)
8.1 Stage 1 — Complete text package

Assemble and verify the Markdown layer.

8.2 Stage 2 — Generate PDFs

Render the canonical human-facing PDF set.

8.3 Stage 3 — Generate SHA-256 manifest

Hash all canonical Markdown and existing package PDFs.

8.4 Stage 4 — Surface package discoverability

Ensure the package is visible from the canonical repository entry path.

8.5 Stage 5 — Add cross-repo pointers

Only after the canonical package is stable should adjacent repositories receive short bridge pointers.

9. Explicit bridge

L4 Hardware Perimeter ↔ Actor Grounding Layer ↔ ARL / runtime reliance

10. Hidden bridges
pre-admissibility / standing discipline
L4 Witness traceability without substituting for grounding
11. Earth paragraph

A real warehouse operator does not call a new control layer “official” because the papers exist on a table. It becomes official when the binder is visible, the core pages are frozen into stable reading form, and the ledger can prove later that the object was not quietly replaced. Publication and integrity do the same job here.
