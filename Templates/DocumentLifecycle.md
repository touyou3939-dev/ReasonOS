# Document Lifecycle

- Version: 1.0
- Status: Approved

---

# Purpose

ReasonOSで管理するすべてのドキュメントは、
定義されたライフサイクルに従って管理する。

ライフサイクルを定義することで、

- 現在の状態
- 品質
- 承認状況

を明確にする。

---

# Constitution Lifecycle

Draft

↓

Architecture Review

↓

Approved

↓

Superseded

↓

Archived

---

# RFC Lifecycle

Draft

↓

Discussion

↓

Accepted

↓

Implemented

↓

Closed

Rejected は必要に応じてClosedへ遷移する。

---

# ADR Lifecycle

Draft

↓

Approved

↓

Superseded

↓

Archived

ADRは履歴であり、
削除しない。

---

# Plugin Lifecycle

Idea

↓

Prototype

↓

Experimental

↓

Stable

↓

Reference

↓

Deprecated

↓

Archived

---

# Kernel Lifecycle

Candidate

↓

Experimental

↓

Core

↓

Deprecated

↓

Archived

Kernelへ昇格する場合は
Promotion Evaluationを通過し、
ADRで承認されなければならない。

---

# Document Status Rules

Draft

執筆中。

レビュー対象ではない。

---

Review

レビュー中。

内容変更可能。

---

Approved

正式採用。

---

Superseded

新しいVersionへ置き換えられた。

削除しない。

---

Archived

利用終了。

履歴として保存する。

---

# Governance Rules

- Approved文書のみ正式仕様とする。
- Superseded文書は削除しない。
- Archived文書は履歴として保存する。
- すべての変更はADRまたはReviewで記録する。

---

# Related Documents

- Constitution
- ADR
- RFC
- Architecture Review Template