# P0007

Status

Draft

---

## Purpose

Define the responsibility of `docs/Open Questions.md`.

---

## Proposed Change

Define `Open Questions.md` as the index of currently open architectural questions.

### Responsibilities

`Open Questions.md` is responsible for:

1. Listing all currently open questions.
2. Providing navigation to detailed question documents.
3. Showing the current status of each question.
4. Helping prioritize future design work.

### Non-Responsibilities

`Open Questions.md` does not contain detailed discussions.

Detailed discussions belong in `docs/questions`.

### Structure

The document serves as a simple index of open questions, for example:

| ID | Question | Status |
| --- | --- | --- |
| Q0001 | Is "Current Understanding" the most appropriate name for its responsibilities? | Open |
| Q0002 | Should every design change originate from an Open Question? | Open |

---

## Rationale

Separating the index from individual question documents keeps responsibilities clear.

`Open Questions.md` provides navigation and status tracking, while detailed discussions remain in individual files under `docs/questions`.

---

## Decision

Pending review.