# P0010

Status

Draft

---

## Purpose

Introduce a standardized review document to preserve proposal evaluation results independently from the original proposals.

---

## Proposed Change

Create a new directory:

- `docs/reviews/`

Each proposal may have a corresponding review document.

Example:

- `docs/reviews/P0003 Review.md`
- `docs/reviews/P0004 Review.md`

Each review document records:

- Review status
- Review summary
- Findings
- Final decision
- Impact on repository artifacts

The original proposal remains unchanged as a historical record.

---

## Rationale

A Commit Proposal represents the original design proposal at the time it was written.

Editing an accepted proposal after review would overwrite historical information and make it difficult to understand the original intent.

Separating proposals from reviews preserves both:

- the original proposal
- the current evaluation

This separation aligns with the responsibility-oriented design of ReasonOS.

---

## Decision

Pending review.