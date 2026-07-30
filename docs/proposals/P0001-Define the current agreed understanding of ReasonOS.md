# P0001

Status

Accepted

---

## Purpose

Define the current agreed understanding of ReasonOS.

Establish Current Understanding as the single source of truth for the design of the system.

---

## Proposed Change

Create `docs/Current Understanding.md` with the following structure.

### Purpose

- This document defines the current agreed understanding of ReasonOS.
- It is the single source of truth for the design of the system.
- When discussion and this document conflict, this document takes precedence until it is intentionally updated.

### Core Principles

#### Principle 1

Current Understanding is the single source of truth.

#### Principle 2

Concepts represent responsibilities.

A concept should exist only when it owns a unique responsibility.

#### Principle 3

Open Questions are preserved until resolved.

Unknowns are valuable design assets and should never be discarded simply because they are inconvenient.

#### Principle 4

Design evolves through explicit discussion.

Every accepted design change should originate from discussion and be intentionally incorporated.

#### Principle 5

Every accepted change is recorded.

ReasonOS should always preserve the history of how its understanding evolved.

### Scope

Current Understanding contains only agreed knowledge.

Ideas, hypotheses, and unresolved discussions belong elsewhere.

---

## Rationale

Current Understanding contains only design decisions that have already been agreed upon.

Concepts that are still under design, including Quality Function, World Model, Observation, Command, and Reasoning Engine, are intentionally excluded.

Current Understanding is the latest design specification, not a collection of ideas.

---

## Decision

Create `docs/Current Understanding.md` as the authoritative design document for ReasonOS.