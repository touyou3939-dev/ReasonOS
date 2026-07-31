# P0011

Status

Draft

---

## Purpose

Define a standard template for Review documents used in the ReasonOS repository.

---

## Proposed Change

Create:

- `docs/templates/Review.md`

The template contains the following structure.

### Status

The current review result.

Examples:

- Accepted
- Accepted with revisions
- Rejected
- Superseded

### Summary

A concise summary of the review outcome.

### Findings

Record the evaluation of each relevant part of the proposal.

Each finding should clearly indicate whether it is:

- Accepted
- Revised
- Rejected

and explain the reasoning when necessary.

### Impact

Describe the repository artifacts affected by the review.

Examples:

- Update `Current Understanding.md`
- Update `Development Process.md`
- No repository changes required

---

## Rationale

Review documents should follow a consistent structure so that proposal evaluations are easy to understand and trace.

Separating review results from proposals preserves historical records while documenting the current evaluation.

A standard template also makes the review process consistent across the repository.

---

## Decision

Pending review.