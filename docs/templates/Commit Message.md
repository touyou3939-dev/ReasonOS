# Commit Message

## Purpose

This document defines the standard format for Git commit messages used in the ReasonOS repository.

A commit message should describe **what changed**.

The rationale for the change belongs in the corresponding Commit Proposal.

---

# Structure

A commit message consists of two parts.

## Summary

```
<scope>: <verb> <object>
```

Example

```
docs: define Open Question index
```

The summary should:

- be written in English
- use the imperative mood
- describe what the commit introduces or changes
- remain concise

---

## Description

The description is optional.

When used, it should summarize the modified artifacts.

Example

```
- update Open Questions index
- add Q0002
- refine question workflow
```

Descriptions should remain concise and avoid explaining the rationale.

The rationale belongs in the Commit Proposal.

---

# Common Scopes

Examples include:

- docs
- core
- reasoning
- knowledge
- tests
- repo

Additional scopes may be introduced as the repository evolves.

---

# Common Verbs

Examples include:

- add
- define
- refine
- update
- rename
- remove
- introduce
- reorganize
- clarify
- document

The chosen verb should clearly represent the primary action of the commit.

---

# Responsibilities

Commit messages describe:

- what changed

Commit messages do not describe:

- why the change was made
- design discussions
- review results

These belong in the Commit Proposal.