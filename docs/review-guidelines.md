# Review Guidelines

This document defines review guidelines for `ktp-origin-audit-examples-v0.1`.

The purpose of review is to evaluate origin-audit records safely, conservatively, and transparently.

A review does not determine final legal authorship, ownership, infringement, or automatic royalty allocation.

It evaluates whether a trace record is clear, evidence-based, reviewable, and safe for downstream use.

---

## 1. Core Review Principle

The core principle of review is:

> Review strengthens evidence.  
> It does not automatically create verdict.

A reviewer may confirm that a trace record is well-formed, plausible, disputed, weak, strong, or ready for further review.

But a reviewer should not treat the record as final origin judgment.

---

## 2. Review Goals

The review process should determine whether a record:

- identifies the target clearly;
- lists origin candidates responsibly;
- separates evidence from judgment;
- uses relation types appropriately;
- documents uncertainty;
- avoids accusation;
- avoids premature allocation;
- marks disputes clearly;
- provides a reasonable next step.

The goal is not to “find the winner.”

The goal is to make the trace relationship reviewable.

---

## 3. Reviewer Roles

A review may be performed by:

- a human reviewer;
- a multi-wing review process;
- an institutional review body;
- an AI-assisted review system;
- a hybrid human-AI review process.

AI-assisted review may help identify patterns, inconsistencies, or missing fields.

However, AI-assisted review should not be treated as the final authority.

---

## 4. Multi-Wing Review Model

A multi-wing review process may divide responsibilities into several review roles.

```text
Trace Intelligence Record
        ↓
Semantic Review Wing
Structural Review Wing
Provenance Review Wing
Dispute Review Wing
Allocation Readiness Wing
Governance Review Wing
        ↓
Review Outcome
```

Each wing examines the same record from a different angle.

This prevents one-dimensional judgment.

---

## 5. Semantic Review

Semantic review evaluates meaning-level similarity.

Reviewers may ask:

- Does the target discuss similar ideas?
- Are similar terms used?
- Is the conceptual vocabulary related?
- Is the similarity strong or generic?
- Could the overlap come from shared public discourse?
- Is the semantic score supported by explanation?

Semantic similarity is useful.

But it is noisy.

A semantic match should not be treated as proof of origin.

---

## 6. Structural Review

Structural review evaluates architecture, sequence, and pattern.

Reviewers may ask:

- Does the target share a similar layered structure?
- Does it use a similar flow of concepts?
- Does it reproduce a specific schema or system architecture?
- Is the resemblance deep or superficial?
- Could the same structure arise independently?
- Is there structure fingerprint evidence?

Structural similarity may be stronger than surface textual similarity.

But structure alone is still not final proof.

---

## 7. Provenance Review

Provenance review evaluates visible history and traceable evidence.

Reviewers may ask:

- Is there explicit citation?
- Is there metadata?
- Is there a content hash?
- Is there watermark evidence?
- Is there chain-of-custody evidence?
- Is there a platform log?
- Is there an Origin Token?
- Are timestamps available?

Strong provenance can increase confidence.

However, missing provenance does not automatically disprove influence.

Likewise, present provenance does not automatically prove final origin.

---

## 8. Citation Review

Citation review evaluates whether an explicit citation is present and meaningful.

Reviewers may ask:

- Does the target cite the origin candidate?
- Is the citation relevant to the target’s main structure?
- Is the citation merely decorative?
- Does the target depend on the cited source?
- Does the target add independent contribution?
- Is the citation accurate?

Explicit citation is strong evidence of reference.

But citation does not automatically determine contribution weight or royalty share.

---

## 9. Implicit Absorption Review

Implicit absorption is one of the most difficult categories.

Reviewers should be especially conservative.

Ask:

- Is there no explicit citation?
- Is there structural similarity?
- Is there conceptual similarity?
- Is there evidence of prior exposure?
- Could the similarity be independent convergence?
- Could it come from shared AI governance discourse?
- Could it come from training data or common vocabulary?
- Are uncertainty notes sufficient?

Implicit absorption should usually remain:

```text
pending
under_review
or disputed
```

until stronger evidence is available.

It should rarely proceed directly to allocation-readiness review.

---

## 10. Blended Influence Review

Blended influence occurs when multiple origin candidates may have contributed to the target.

Reviewers should avoid forcing a single-origin conclusion.

Ask:

- Are multiple origin candidates plausible?
- Does each candidate have a distinct relation type?
- Are confidence scores separated by candidate?
- Are limitations documented for each candidate?
- Is the target better understood as a trace field?
- Does the record avoid crowning one source prematurely?

Blended influence is a map.

It is not a throne room.

---

## 11. Dispute Review

A disputed record requires special handling.

Reviewers should ask:

- Who or what disputes the claim?
- What is the reason for dispute?
- Is the dispute about evidence, interpretation, confidence, or relation type?
- Is the dispute status clearly marked?
- Is allocation readiness blocked?
- What next step is required?

A disputed record should not move toward allocation until the dispute is reviewed.

Dispute is not failure.

Dispute is part of the lifecycle.

---

## 12. Allocation Readiness Review

Allocation readiness review evaluates whether a record may proceed to a separate allocation-readiness process.

This is not the same as approving payment.

A record may be ready for allocation-readiness review when:

- evidence is documented;
- review status is `reviewed`;
- no active dispute exists;
- uncertainty is visible;
- relation type is appropriate;
- confidence is not exaggerated;
- next step is clearly stated.

The correct interpretation is:

```text
Ready for allocation-readiness review
        ≠
Approved for royalty allocation
```

Actual allocation requires a separate process.

---

## 13. Confidence Review

Confidence scores should be reviewed carefully.

Reviewers should check:

- Is the score consistent with the evidence?
- Is the score too high for uncertain cases?
- Are implicit absorption cases scored conservatively?
- Are citation-based cases supported by actual citation?
- Are structural and semantic scores explained?
- Are limitations included?

Suggested interpretation:

```text
0.00 - 0.39   weak signal
0.40 - 0.59   possible relation
0.60 - 0.74   moderate relation
0.75 - 0.89   strong candidate relation
0.90 - 1.00   very strong evidence, still not final judgment
```

Even a score above `0.90` is still evidence, not verdict.

---

## 14. Review Status Guidelines

Recommended usage:

### `pending`

Use when the record has not yet been reviewed.

### `under_review`

Use when review is currently in progress.

### `reviewed`

Use when the record has received review and may proceed to a next step.

### `disputed`

Use when the claim is actively challenged or uncertain enough to require dispute handling.

### `rejected`

Use when the record is not supported by sufficient evidence.

### `revised`

Use when the record has been updated after review.

### `accepted_as_candidate`

Use when the candidate relationship is accepted as plausible, but not final origin.

---

## 15. Red Flags

Reviewers should be cautious when a record:

- claims final origin;
- uses accusatory language;
- treats similarity as proof;
- hides uncertainty;
- lacks evidence items;
- gives high confidence without explanation;
- collapses blended influence into one source;
- marks allocation readiness as true while disputed;
- treats citation as automatic royalty approval;
- has no review notes;
- bypasses dispute handling.

A record with these issues should be revised or rejected.

---

## 16. Green Flags

A strong record usually:

- identifies the target clearly;
- lists origin candidates responsibly;
- separates evidence items;
- explains relation types;
- uses conservative confidence scores;
- includes limitations;
- includes uncertainty notes;
- marks review status clearly;
- blocks allocation when disputed;
- separates readiness review from actual allocation.

A good record is careful.

It does not rush toward judgment.

---

## 17. Recommended Review Questions

Reviewers should ask:

1. Is the target clearly identified?
2. Are origin candidates listed as candidates, not final origins?
3. Is the relation type appropriate?
4. Is evidence separated from analysis?
5. Are confidence scores justified?
6. Is uncertainty documented?
7. Are limitations visible?
8. Is the record free from accusatory language?
9. Is dispute status correct?
10. Is allocation readiness separated from allocation?
11. Does the record require further review?
12. Should the record be accepted, revised, rejected, or disputed?

---

## 18. Possible Review Outcomes

A review may produce one of the following outcomes:

### Accept as Candidate

The origin relationship is plausible enough to remain recorded.

This is not final origin judgment.

### Request Revision

The record needs clearer evidence, lower confidence, better limitations, or corrected relation type.

### Mark as Disputed

The claim is contested or uncertain enough to require dispute handling.

### Reject

The record does not contain enough evidence to support the candidate relationship.

### Escalate

The case requires governance review, dispute review, or allocation-readiness review.

---

## 19. Review Notes

Review notes should be:

- concise;
- neutral;
- evidence-based;
- non-accusatory;
- clear about uncertainty;
- clear about next steps.

Avoid language such as:

```text
This proves theft.
This is the true origin.
This must be paid immediately.
This is clearly copied.
```

Prefer language such as:

```text
This record supports a possible structural relationship.
This candidate may be relevant for further review.
The evidence is moderate but incomplete.
This claim should remain disputed until additional evidence is reviewed.
```

---

## 20. Review and Royalty Separation

Reviewers must preserve the boundary between trace evidence and royalty allocation.

A review may say:

> This record may proceed to allocation-readiness review.

It should not say:

> This record approves payment.

Royalty calculation requires separate criteria, governance, contribution weighting, tolerance bands, and dispute handling.

---

## 21. Summary

Review is a safety layer.

Its purpose is to slow down premature judgment and make trace reasoning visible.

A good review process follows this posture:

```text
Observe.
Compare.
Question.
Document.
Review.
Then decide whether further review is needed.
```

The final rule is simple:

```text
Candidate, not verdict.
Evidence, not enforcement.
Review before allocation.
```
