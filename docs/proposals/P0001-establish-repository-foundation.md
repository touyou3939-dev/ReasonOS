# P0001

Status

Accepted

---

## Purpose

Create the initial repository structure for ReasonOS.

The repository serves as the authoritative location for design artifacts,
allowing ReasonOS to evolve through explicit design decisions, version
control, and continuous documentation.

---

## Proposed Change

Establish the initial repository structure.

```text
ReasonOS/
├── README.md
└── docs/
    ├── Current Understanding.md
    ├── Open Questions.md
    ├── Development Process.md
    ├── Change Log.md
    └── Design Retrospectives.md
```

---

## Rationale

ReasonOS is intended to evolve incrementally rather than being fully
specified from the beginning.

Creating a stable repository structure provides a shared foundation for
future design work and keeps design artifacts organized.

---

## Decision

The initial repository structure is established as the foundation for
ReasonOS.

Git is adopted as the version control system.

GitHub is adopted as the authoritative repository for ReasonOS.