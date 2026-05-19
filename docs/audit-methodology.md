# Audit Methodology

This document defines a basic audit methodology for `ktp-origin-audit-examples-v0.1`.

The purpose of this methodology is to show how origin-audit examples may be created, reviewed, and interpreted safely under the Kazene Trace Protocol.

This methodology does not determine final origin, legal authorship, ownership, infringement, or automatic royalty allocation.

It provides a structured process for documenting possible trace relationships.

---

## 1. Core Methodological Principle

The core principle of KTP origin audit is:

> Audit before judgment.

An origin audit record is not a verdict.

It is a structured evidence packet that helps reviewers understand possible relationships between a target and one or more origin candidates.

The audit process should preserve uncertainty rather than hide it.

---

## 2. Audit Flow

A basic KTP origin audit follows this flow:

```text
Target observed
        ↓
Possible origin candidates identified
        ↓
Evidence collected
        ↓
Relationship type assigned
        ↓
Confidence estimated
        ↓
Uncertainty documented
        ↓
Review status assigned
        ↓
Dispute status checked
        ↓
Allocation readiness considered separately

This flow prevents similarity from being mistaken for proof.

3. Step 1: Identify the Target

The target is the item being audited.

A target may be:

an article;
a model output;
a prompt;
a concept;
a structure;
a code fragment;
an image;
a dataset;
another creative or technical artifact.

The target record should include, when available:

title;
URI;
content hash;
capture timestamp;
language;
summary.

The target should be described neutrally.

Avoid accusatory language.

4. Step 2: Identify Origin Candidates

An origin candidate is a possible source of influence.

It is not a final origin.

Origin candidates may be identified through:

explicit citation;
direct reference;
structural similarity;
conceptual influence;
semantic similarity;
implicit absorption;
derivative adaptation;
paraphrase;
translation;
blended influence;
unknown or uncertain relation.

Multiple origin candidates may be recorded.

A single target should not be forced into a single-origin model when the evidence suggests a wider field of influence.

5. Step 3: Classify the Relationship Type

Each origin candidate should include a relation_type.

Recommended relation types include:

direct_reference
explicit_citation
structural_similarity
conceptual_influence
semantic_similarity
implicit_absorption
derivative_adaptation
paraphrase
translation
blended_influence
unknown

The relation type should describe the nature of the evidence.

It should not be used as a final judgment.

6. Step 4: Collect Evidence

Evidence may include:

citation evidence;
metadata evidence;
watermark evidence;
content hashes;
structure fingerprint outputs;
semantic similarity scores;
chain-of-custody records;
human observations;
AI-assisted analysis;
platform logs;
other relevant documentation.

Evidence should be recorded as separate items whenever possible.

This makes later review easier.

7. Step 5: Estimate Confidence

Confidence scores should be treated as provisional.

A confidence score may reflect:

strength of citation;
degree of semantic similarity;
degree of structural similarity;
conceptual overlap;
quality of metadata;
availability of chain-of-custody evidence;
uncertainty level;
reviewer confidence.

Confidence should generally remain conservative.

High confidence does not mean final origin judgment.

8. Suggested Confidence Interpretation

The following ranges may be used as a practical guide:

0.00 - 0.39   weak signal
0.40 - 0.59   possible relation
0.60 - 0.74   moderate relation
0.75 - 0.89   strong candidate relation
0.90 - 1.00   very strong evidence, still not final judgment

Even scores above 0.90 should not be treated as legal proof, ownership proof, or automatic allocation approval.

Confidence is evidence.

It is not verdict.

9. Step 6: Document Uncertainty

Every audit record should document uncertainty.

Uncertainty may arise from:

missing citation;
missing metadata;
missing watermark;
incomplete chain of custody;
possible independent convergence;
shared technical vocabulary;
blended influence;
AI-generated recombination;
paraphrase;
translation;
weak or conflicting evidence.

Uncertainty should be written clearly in limitations and uncertainty_notes.

This is not a weakness of the audit.

It is a safety feature.

10. Step 7: Assign Review Status

The audit record should include a review status.

Possible states may include:

pending
under_review
reviewed
disputed
rejected
revised
accepted_as_candidate

A record with pending status should not be used for downstream allocation decisions.

A record with disputed status should remain blocked until the dispute is reviewed or resolved.

A record with reviewed status may proceed to later review stages, but still does not become a final judgment.

11. Step 8: Check Dispute Status

Dispute status should be recorded when a trace claim is challenged.

A disputed record may include:

dispute ID;
reason for dispute;
current status;
reviewer notes;
required next step.

Dispute is part of the lifecycle.

It should not be treated as system failure.

The purpose of dispute handling is to keep contested claims visible, reviewable, and blocked from premature allocation.

12. Step 9: Consider Allocation Readiness Separately

Allocation readiness must be handled separately from trace evidence.

A record may be marked:

"allocation_readiness": {
  "ready": true,
  "reason": "The record may proceed to allocation-readiness review.",
  "required_next_step": "allocation_readiness_review"
}

This does not mean automatic royalty allocation.

It only means the record may be reviewed by a later allocation-readiness process.

The distinction is essential:

Ready for allocation-readiness review
        ≠
Approved for royalty allocation
13. Audit Categories

This repository includes five basic audit categories.

13.1 Explicit Citation

A target directly cites or references an origin candidate.

This is usually a stronger trace case.

However, citation does not automatically determine contribution weight or royalty allocation.

13.2 Implicit Absorption

A target appears structurally or conceptually related to an origin candidate without explicit citation.

This is highly uncertain and requires careful review.

13.3 Blended Influence

A target appears influenced by multiple origin candidates.

The audit should preserve multiple candidates rather than force a single origin.

13.4 Disputed Trace Claim

A trace claim is challenged.

The record should remain visible but blocked from allocation progression until review.

13.5 Allocation Readiness Review

A reviewed trace record appears ready for a later allocation-readiness process.

This does not mean payment is approved.

14. Evidence Weighting Guidelines

Different evidence types have different practical strength.

A rough guide:

Explicit citation              strong evidence of reference
Chain of custody               strong provenance evidence
Metadata / watermark           useful provenance evidence
Structure fingerprint          useful structural evidence
Semantic similarity            useful but noisy evidence
Human observation              useful review evidence
AI-assisted analysis           useful but must be reviewed
Implicit absorption signal     uncertain and review-heavy

No single evidence type should automatically determine final origin.

The strongest records usually combine several evidence types.

15. Handling Implicit Absorption

Implicit absorption should be treated with special caution.

It may occur when a target resembles an origin candidate without direct citation or visible provenance.

Possible explanations include:

actual influence;
indirect exposure;
training data influence;
prior conversation influence;
shared discourse;
independent convergence;
common terminology;
coincidence.

For this reason, implicit absorption records should usually include:

moderate confidence;
clear limitations;
uncertainty notes;
review requirement;
allocation readiness set to false.
16. Handling Blended Influence

Blended influence occurs when multiple origin candidates may have shaped a target.

The audit should not reduce the case to one winner.

Instead, it should record a trace field.

Each candidate should have:

relation type;
confidence;
evidence summary;
limitations.

A blended influence record is a map, not a crown ceremony.

17. Handling Disputed Claims

A disputed claim should remain visible but marked clearly.

A disputed record should generally include:

"review_status": {
  "state": "disputed"
}

and:

"dispute_status": {
  "disputed": true,
  "status": "opened"
}

Allocation readiness should generally remain false until the dispute is resolved.

18. Handling Allocation-Readiness Cases

Allocation readiness is a downstream gate.

A record may be ready for allocation-readiness review when:

explicit evidence is present;
review has been completed;
no active dispute exists;
evidence is relevant;
uncertainty is documented;
the next step is clearly marked.

Even then, the record does not calculate allocation.

It only prepares the case for another process.

19. Safety Rules

Every origin audit should follow these safety rules:

Do not treat candidates as final origins.
Do not treat similarity as proof.
Do not treat confidence as verdict.
Do not treat citation as automatic allocation.
Do not use audit records as accusations.
Do not bypass review.
Do not trigger payment directly from an audit example.
Do not hide uncertainty.
Do not erase disputes.
Do not collapse blended influence into one origin without justification.
20. Recommended Review Questions

Reviewers may ask:

What is the target?
What origin candidates are listed?
What relation type is assigned to each candidate?
What evidence supports each relation?
What evidence is missing?
Is the confidence score conservative?
Are limitations documented?
Is uncertainty visible?
Is the record disputed?
Is allocation readiness separated from final allocation?
Does the record avoid legal or financial overclaiming?
Is further human or multi-wing review required?

These questions help keep the audit process safe.

21. Output Expectations

A good KTP origin audit record should be:

structured;
neutral;
reviewable;
conservative;
transparent;
dispute-aware;
allocation-safe;
compatible with the KTP Trace Intelligence Specification.

A poor audit record is:

accusatory;
overconfident;
single-origin obsessed;
unclear about evidence;
silent about uncertainty;
eager to allocate;
resistant to dispute.
22. Summary

KTP origin audit is a method for documenting possible trace relationships.

It is not a method for declaring final truth.

The correct posture is:

Observe carefully.
Record clearly.
Preserve uncertainty.
Invite review.
Separate evidence from allocation.

The goal is not perfect origin judgment.

The goal is trustworthy trace practice.
