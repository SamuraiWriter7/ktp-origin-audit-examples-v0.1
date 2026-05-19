# KTP Origin Audit Examples v0.1

Example origin-audit records for applying the KTP Trace Intelligence Specification to origin candidates, implicit absorption, blended influence, disputed trace claims, and allocation-readiness cases.

This repository is a companion repository to:

```text
ktp-trace-intelligence-spec-v0.1
```

While `ktp-trace-intelligence-spec-v0.1` defines the Trace Intelligence Record format, this repository demonstrates how that format can be used in practical or hypothetical audit scenarios.

It does **not** determine final origin, legal authorship, ownership, infringement, or automatic royalty allocation.

Its purpose is to provide safe examples for documenting trace relationships without turning evidence into final judgment.

---

## Core Principle

> Audit examples are not verdicts.

Each example in this repository demonstrates how to record a possible trace relationship.

It does not claim:

> “This is the true origin.”

Instead, it demonstrates:

> “This is how a possible origin candidate may be documented for review.”

The purpose of these examples is to support learning, testing, prototyping, and review culture around the Kazene Trace Protocol.

---

## Purpose

This repository provides example records for:

- explicit citation cases;
- implicit absorption cases;
- blended influence cases;
- disputed trace claims;
- allocation-readiness review cases;
- multi-origin trace scenarios;
- safe documentation of uncertain origin relationships.

The goal is to make the KTP Trace Intelligence Specification easier to understand, implement, and review.

---

## Non-Goals

This repository does not attempt to:

- prove legal authorship;
- prove copyright ownership;
- accuse any person, platform, or model;
- determine final origin status;
- calculate royalty shares;
- trigger automatic payments;
- enforce claims;
- replace review, dispute, or governance processes.

These examples are educational and structural.

They are not legal or financial determinations.

---

## Relationship to KTP Trace Intelligence Specification

This repository depends conceptually on the KTP Trace Intelligence Specification.

```text
ktp-trace-intelligence-spec-v0.1
        ↓
ktp-origin-audit-examples-v0.1
```

The specification defines the structure of a Trace Intelligence Record.

This repository shows example uses of that structure.

```text
Trace Intelligence Record
        ↓
Origin Audit Example
        ↓
Review / Dispute
        ↓
Allocation Readiness
        ↓
Royalty OS
```

In this flow, origin-audit examples act as practical test cases.

They help show how trace evidence can be recorded without making final judgments.

---

## Conceptual Position

```text
Kazene Trace Protocol
        ↓
Trace Intelligence Specification
        ↓
Origin Audit Examples
        ↓
Review Guidelines
        ↓
Dispute / Allocation Readiness
        ↓
Royalty OS
```

This repository belongs to the example and practice layer.

It is not the protocol core.

It is not the allocation layer.

It is not the enforcement layer.

It is a set of structured examples showing how the observation layer may be used.

---

## Why This Repository Exists

The Kazene Trace Protocol deals with difficult trace problems.

Some cases are simple.

For example, a target explicitly cites an origin source.

Other cases are much harder.

For example:

- an AI output resembles an earlier structure without citation;
- several origin candidates appear to be blended together;
- a trace claim is disputed;
- a work shows strong structural similarity but weak metadata evidence;
- a record may be useful for review but not ready for allocation.

These cases require careful documentation.

This repository provides examples for those difficult situations.

The goal is not to create perfect answers.

The goal is to create safe patterns for reviewable trace documentation.

---

## Example Categories

### 1. Explicit Citation

A target directly cites or references an origin candidate.

This is the simplest form of trace relationship.

The example demonstrates how citation evidence may be recorded without automatically determining allocation.

### 2. Implicit Absorption

A target appears to absorb or resemble an earlier structure without explicit citation.

This is one of the hardest KTP cases.

The example demonstrates how uncertainty, confidence, and limitations should be recorded.

### 3. Blended Influence

A target appears to be influenced by multiple origin candidates.

The example demonstrates how several possible origins can be recorded without forcing a single-origin conclusion.

### 4. Disputed Trace Claim

A trace claim is challenged, questioned, or contested.

The example demonstrates how dispute status can be represented and how judgment should remain suspended.

### 5. Allocation Readiness Review

A trace record is being evaluated for possible downstream allocation review.

The example demonstrates how allocation readiness can be documented without triggering automatic royalty distribution.

---

## Repository Structure

```text
ktp-origin-audit-examples-v0.1/
├── README.md
├── CHANGELOG.md
├── CITATION.cff
├── LICENSE
├── examples/
│   ├── explicit-citation.example.json
│   ├── implicit-absorption.example.json
│   ├── blended-influence.example.json
│   ├── disputed-trace-claim.example.json
│   └── allocation-readiness-review.example.json
├── docs/
│   ├── relationship-to-trace-intelligence-spec.md
│   ├── audit-methodology.md
│   └── review-guidelines.md
└── .github/
    └── workflows/
        └── validate-examples.yml
```

---

## Repository Components

### `examples/`

Contains example origin-audit records for different KTP trace scenarios.

- `explicit-citation.example.json`  
  Demonstrates a case where the target explicitly cites an origin candidate.

- `implicit-absorption.example.json`  
  Demonstrates a difficult case where structural or conceptual similarity appears without explicit citation.

- `blended-influence.example.json`  
  Demonstrates a case where multiple origin candidates may have influenced the target.

- `disputed-trace-claim.example.json`  
  Demonstrates a case where a trace claim is challenged and must remain blocked from allocation-readiness progression.

- `allocation-readiness-review.example.json`  
  Demonstrates a reviewed case that may proceed to allocation-readiness review, without triggering automatic royalty allocation.

### `docs/`

Contains explanatory documents for methodology, review, and relationship to the KTP Trace Intelligence Specification.

- `relationship-to-trace-intelligence-spec.md`  
  Explains how this example repository relates to `ktp-trace-intelligence-spec-v0.1`.

- `audit-methodology.md`  
  Defines the basic audit flow and methodology for creating origin-audit records.

- `review-guidelines.md`  
  Defines review criteria for human, AI-assisted, and multi-wing review processes.

### `.github/workflows/`

Contains GitHub Actions workflow files.

- `validate-examples.yml`  
  Validates required files, example JSON structure, and KTP semantic safety rules.

### `CHANGELOG.md`

Records version history and planned changes.

### `CITATION.cff`

Provides citation metadata for referencing this repository.

### `LICENSE`

Defines the license for the repository.

---

## Start Here

Recommended reading order:

1. `README.md`
2. `docs/relationship-to-trace-intelligence-spec.md`
3. `docs/audit-methodology.md`
4. `docs/review-guidelines.md`
5. `examples/implicit-absorption.example.json`
6. `examples/blended-influence.example.json`
7. `examples/disputed-trace-claim.example.json`
8. `examples/explicit-citation.example.json`
9. `examples/allocation-readiness-review.example.json`

For the most important KTP audit cases, start with:

```text
examples/implicit-absorption.example.json
examples/blended-influence.example.json
examples/disputed-trace-claim.example.json
```

These examples represent difficult cases where origin tracing requires caution, uncertainty documentation, and review.

For easier comparison cases, see:

```text
examples/explicit-citation.example.json
examples/allocation-readiness-review.example.json
```

---

## Example Lifecycle

```text
Target observed
        ↓
Possible origin candidates identified
        ↓
Trace evidence recorded
        ↓
Uncertainty documented
        ↓
Review status assigned
        ↓
Dispute status recorded if needed
        ↓
Allocation readiness considered separately
```

This lifecycle prevents similarity from being mistaken for proof.

---

## Validation

This repository includes a GitHub Actions workflow for validating the example files:

```text
.github/workflows/validate-examples.yml
```

The workflow checks:

- required repository files;
- JSON syntax for all example records;
- required top-level fields;
- valid observer types;
- valid target types;
- valid relation types;
- valid review states;
- valid dispute statuses;
- valid allocation-readiness next steps;
- confidence scores within the `0.0` to `1.0` range;
- presence of evidence items;
- presence of analysis notes;
- presence of uncertainty notes;
- basic KTP semantic safety rules.

Validation is automatically triggered on:

- push to `main`;
- pull requests to `main`;
- manual workflow dispatch.

---

## Semantic Safety Checks

The validation workflow also performs KTP-specific safety checks.

These include:

```text
disputed = true
        → allocation_readiness.ready must be false
        → required_next_step must be dispute_resolution
```

```text
relation_type = implicit_absorption
        → confidence should remain conservative
        → allocation_readiness.ready should be false
```

```text
allocation_readiness.ready = true
        → review_status.state must be reviewed or accepted_as_candidate
        → dispute_status.disputed must be false
        → required_next_step must be allocation_readiness_review
```

These checks help preserve the core boundary:

```text
Origin audit example
        ≠
Final origin judgment
        ≠
Automatic royalty allocation
```

---

## Validation Scope

A passing workflow means that the example records are structurally valid and follow the repository’s basic KTP safety rules.

It does **not** mean that:

- a candidate is the final origin;
- a trace claim is legally valid;
- ownership has been determined;
- infringement has been proven;
- royalty allocation has been approved;
- payment should be triggered.

Validation confirms format and safety constraints.

It does not confirm truth.

---

## Local Validation

The workflow can also be run locally by copying the Python validation block from:

```text
.github/workflows/validate-examples.yml
```

and executing it from the repository root.

A future version may add a standalone test runner for local validation.

---

## Safety Boundary

Every example in this repository should follow these principles:

- candidate, not verdict;
- evidence, not enforcement;
- inference, not judgment;
- review before allocation;
- dispute as lifecycle;
- transparency over certainty;
- no direct accusation;
- no automatic royalty trigger.

An origin-audit example is not a legal claim.

It is a structured demonstration of how trace evidence may be recorded.

---

## Relationship to Review Culture

KTP Origin Audit Examples are intended to support a review culture.

A healthy trace culture requires:

- careful documentation;
- visible uncertainty;
- multiple origin candidates when appropriate;
- room for dispute;
- no premature judgment;
- separation between evidence and allocation;
- protection against false origin claims.

The examples in this repository are meant to help cultivate that culture.

---

## Relationship to Royalty OS

This repository does not implement Royalty OS.

It only provides upstream audit examples.

The broader flow is:

```text
Trace Intelligence Record
        ↓
Origin Audit Example
        ↓
Review / Dispute
        ↓
Allocation Readiness
        ↓
Royalty OS
```

Royalty OS may use reviewed trace records as one kind of input.

However, raw examples and unreviewed records should never trigger allocation directly.

---

## Status

Draft v0.1.0.

This repository is experimental and intended for discussion, prototyping, testing, and educational use within the broader Kazene Trace Protocol ecosystem.

---

## Citation

Citation metadata is provided in:

```text
CITATION.cff
```

If you use this repository, please cite it using the information provided there.

---

## License

This project is licensed under the MIT License.

See `LICENSE` for details.

---

## Changelog

See `CHANGELOG.md`.

---

## Key Statement

Origin audit is not origin judgment.

An audit example observes and documents.

It does not decide, punish, allocate, or enforce.
