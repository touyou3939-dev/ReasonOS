# Document Lifecycle

- Version: 1.2
- Status: Approved

---

# Purpose

DocumentLifecycleは、ReasonOS Repositoryで管理されるドキュメントの共通Lifecycleを定義する。

目的は、

- ドキュメントの成熟度を明確にすること
- Repository全体の運用を統一すること
- 長期的な保守性を向上させること

である。

本ドキュメントは共通Lifecycleのみを定義する。

各ドキュメント種別固有のLifecycleは、
必要に応じて各カテゴリの仕様書で定義する。

---

# Scope

本LifecycleはRepository全体へ適用する。

対象例

- Constitution
- Governance
- Kernel
- Plugins
- ADR
- RFC
- Reviews
- Templates

---

# Responsibility

DocumentLifecycleは、
Document状態の定義のみを管理する。

管理対象:

- Document State Definition
- Common Lifecycle Model
- State Transition Concept

以下は管理対象外とする。

- Review基準
- Repository状態一覧
- Promotion判断

これらは各責務を持つ別Documentで管理する。

---

# Lifecycle Principles

- Lifecycleはドキュメントの状態を表す。
- 状態はRepository全体で一貫した意味を持つ。
- 必要最小限の状態のみを定義する。
- 既存の状態で表現できる場合は、新しい状態を追加しない。

---

# Common States

## Draft

作成中。

内容は変更される可能性がある。

---

## Review

レビュー中。

正式採用前の状態。

---

## Approved

正式に採用された状態。

Repository標準の成果物として扱う。

---

## Superseded

新しい成果物によって置き換えられた状態。

履歴として保持する。

---

## Archived

保守対象外。

履歴保存のみを目的とする。

---

# Reference Lifecycles

以下は代表例である。

詳細なLifecycleは各カテゴリの仕様書で定義できる。

---

## Constitution

Draft

↓

Review

↓

Approved

↓

Superseded

↓

Archived

---

## ADR

Draft

↓

Review

↓

Approved

↓

Superseded

↓

Archived

---

## RFC

Draft

↓

Discussion

↓

Accepted

↓

Closed

---

## Plugin Documents

Draft

↓

Review

↓

Approved

↓

Superseded

↓

Archived

---

# Relationship with Other Governance Documents

DocumentLifecycleは、
Repository Governance Layerの一部として機能する。

責務分担:

RepositoryManifest

- Repositoryの現在状態を記録する
- Document Statusを表示する

ReviewPolicy

- Review基準を定義する
- 状態変更の妥当性を評価する

DocumentLifecycle

- Document状態の意味を定義する

---

# Extension Rule

各カテゴリは、
共通Lifecycleを維持したまま必要に応じて固有の状態を追加できる。

ただし、

- 共通Stateを変更しない。
- 既存Stateで表現できる場合、新しいStateを追加しない。

---

# Related Documents

- Governance/ReviewPolicy.md
- RepositoryManifest.md
- Governance/RepositoryRules.md