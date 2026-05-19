# Relationship to KTP Trace Intelligence Specification

This document explains how `ktp-origin-audit-examples-v0.1` relates to `ktp-trace-intelligence-spec-v0.1`.

The KTP Trace Intelligence Specification defines the record format.

This repository provides example records that demonstrate how the format may be used in practical or hypothetical origin-audit scenarios.

---

## 1. Specification and Examples

The relationship between the two repositories is simple:

```text
ktp-trace-intelligence-spec-v0.1
        ↓
Defines the Trace Intelligence Record format

ktp-origin-audit-examples-v0.1
        ↓
Demonstrates example uses of that format

The specification repository defines the structure.

This repository shows how that structure can be applied.

2. Role of the Trace Intelligence Specification

ktp-trace-intelligence-spec-v0.1 defines a minimal evidence-packet format for recording:

trace identifiers;
observers;
targets;
origin candidates;
evidence;
analysis notes;
review status;
dispute status;
allocation readiness;
governance context.

Its core principle is:

Origin candidates are not final origins.

The specification is designed to preserve trace evidence without making final judgments.

3. Role of This Repository

ktp-origin-audit-examples-v0.1 does not redefine the Trace Intelligence Record.

Instead, it provides example records for cases such as:

explicit citation;
implicit absorption;
blended influence;
disputed trace claims;
allocation-readiness review.

These examples help implementers, reviewers, and researchers understand how the specification may be used safely.

4. Conceptual Flow
KTP Trace Intelligence Specification
        ↓
Trace Intelligence Record format
        ↓
Origin Audit Examples
        ↓
Review Guidelines
        ↓
Dispute / Allocation Readiness
        ↓
Royalty OS

This repository sits in the example and practice layer.

It is not the specification core.

It is not the review authority.

It is not the allocation engine.

5. Why Examples Are Needed

A specification alone is not enough.

Trace intelligence involves difficult cases where simple rules are insufficient.

For example:

a target may explicitly cite an origin;
a target may resemble an origin without citation;
multiple origin candidates may be blended together;
a trace claim may be disputed;
a reviewed record may be ready for allocation-readiness review but not automatic allocation.

The examples in this repository show how these situations may be documented without turning evidence into verdict.

6. Shared Safety Boundary

Both repositories share the same safety boundary.

A Trace Intelligence Record or origin-audit example must not be treated as:

a legal judgment;
a final authorship claim;
a final ownership claim;
an accusation;
an automatic royalty trigger;
an enforcement action;
a platform moderation decision.

The correct interpretation is:

Evidence packet
        ≠
Final judgment

The examples preserve this boundary.

7. Example Categories and Their Purpose
Explicit Citation

Demonstrates a relatively strong trace case where a target clearly cites an origin candidate.

Even in this case, citation does not automatically determine contribution weight or royalty allocation.

Implicit Absorption

Demonstrates a difficult case where a target appears structurally or conceptually related to an origin candidate without explicit citation.

This requires caution and review.

Blended Influence

Demonstrates a case where multiple origin candidates may have influenced the target.

This avoids forcing a single-origin conclusion.

Disputed Trace Claim

Demonstrates how a trace claim can remain visible while being explicitly marked as disputed.

Dispute is treated as part of the lifecycle, not as system failure.

Allocation Readiness Review

Demonstrates a case where a reviewed record may proceed to allocation-readiness review.

This does not mean automatic royalty distribution.

8. Relationship to Review

The examples are designed to support review culture.

They may be used by:

human reviewers;
multi-wing review processes;
governance bodies;
AI-assisted audit systems;
researchers;
implementers;
protocol designers.

However, examples do not replace review.

They only demonstrate possible record patterns.

9. Relationship to Dispute

Dispute is expected in trace systems.

This repository includes a disputed trace claim example to show that uncertainty should be recorded rather than hidden.

A disputed record should remain blocked from allocation-readiness progression until the dispute is reviewed or resolved.

Trace claim
        ↓
Dispute opened
        ↓
Review required
        ↓
Revision / rejection / acceptance as candidate

This helps prevent weak or contested claims from becoming enforcement tools.

10. Relationship to Allocation Readiness

The KTP Trace Intelligence Specification includes an allocation_readiness field.

This field must be interpreted carefully.

In these examples, allocation_readiness.ready = true means:

The record may proceed to allocation-readiness review.

It does not mean:

Payment should be triggered automatically.

The distinction is essential.

Ready for allocation-readiness review
        ≠
Approved for royalty allocation

Allocation decisions require separate criteria, governance, and review.

11. Relationship to Royalty OS

This repository does not implement Royalty OS.

It only provides upstream audit examples.

The broader flow is:

Trace Intelligence Record
        ↓
Origin Audit Example
        ↓
Review / Dispute
        ↓
Allocation Readiness
        ↓
Royalty OS

Royalty OS may use reviewed trace records as one kind of input.

However, raw examples and unreviewed records should never trigger allocation directly.

12. Recommended Usage

Use this repository to:

understand how Trace Intelligence Records may look in practice;
test validators or parsers;
design review workflows;
discuss difficult origin-audit cases;
develop safer trace governance patterns;
teach the difference between evidence and judgment.

Do not use this repository to:

accuse real individuals or organizations;
make legal claims;
assign ownership;
calculate royalties;
enforce payment;
automate moderation;
bypass review.
13. Compatibility

The examples in this repository are intended to follow the structure defined by:

ktp-trace-intelligence-spec-v0.1

Future versions may add:

schema validation workflows;
additional example categories;
scenario metadata;
review outcome examples;
dispute resolution examples;
allocation-readiness profiles;
links to Structure Fingerprint and Dispute Registry specifications.
14. Summary

ktp-trace-intelligence-spec-v0.1 defines the form.

ktp-origin-audit-examples-v0.1 demonstrates the use.

The specification is the eye.

The examples are what the eye first learns to observe.

Together, they support the broader goal of the Kazene Trace Protocol:

Trustworthy trace, not perfect trace.
Evidence, not enforcement.
Candidate, not verdict.
Review before allocation.
