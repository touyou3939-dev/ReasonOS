# Repository Rules

- Version: 1.0
- Status: Draft

---

# Purpose

Repository Rulesは、ReasonOS Repository全体の運用ルールを定義する。

目的は、

- Repository構造の一貫性を保つこと
- 成果物の責務を明確にすること
- ドキュメントの配置ルールを統一すること

である。

---

# Scope

本ルールはRepository全体へ適用する。

対象

- Constitution
- Governance
- Kernel
- Plugins
- ADR
- RFC
- Reviews
- Templates

---

# Repository Principles

Repositoryは責務単位で構成する。

新しいフォルダ・ドキュメントを追加する前に、

既存の責務で表現できないかを検討する。

---

# Scope Rule

ADR・RFC・Reviewは、

最も影響範囲（Scope）が近い場所へ保存する。

## Repository Scope

ReasonOS全体へ影響するもの

保存場所

ReasonOS/

- ADR/
- RFC/
- Reviews/

---

## Plugin Scope

Plugin固有のもの

保存場所

Plugins/<Plugin>/

- ADR/
- RFC/
- Reviews/

---

# Constitution Rule

Constitution番号はApproved時に採番する。

Candidateには番号を付与しない。

---

# Review Rule

以下はArchitecture Reviewを必須とする。

- Constitution
- Kernel
- Plugin README
- Plugin Framework
- Glossary

その他は必要に応じてReviewを実施する。

---

# Lifecycle

各ドキュメントはDocument Lifecycleに従って管理する。

Lifecycleの詳細は別ドキュメントで定義する。

---

# Future Extension

Repository RuleはMechanismである。

Evidenceに基づいて継続的に改善する。