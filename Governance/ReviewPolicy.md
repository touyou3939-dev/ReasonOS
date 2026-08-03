# Review Policy

- Version: 1.2
- Status: Approved

---

# Purpose

Review Policyは、ReasonOS Repositoryにおけるレビューの目的、対象、基準、および運用ルールを定義する。

レビューの目的は成果物の承認ではなく、
品質の継続的な向上である。

---

# Scope

本ポリシーはRepository全体へ適用する。

対象

- Constitution
- Governance
- Kernel
- Plugins
- ADR
- RFC
- Templates

---

# Review Principles

レビューは以下の原則に従う。

- Responsibility First
- Consistency First
- Simplicity First
- Reusability First
- Evidence First

レビューは設計者ではなく、
成果物を対象とする。

---

# Review Objectives

レビューでは次の観点を確認する。

- Purpose
- Responsibility
- Universality
- Stability
- Consistency
- Simplicity
- Testability

---

# Responsibility Boundary

ReviewPolicyは、
Document変更やPromotion判断に必要なReview評価を定義する。

管理対象:

- Review Criteria
- Review Process
- Review Outcome
- Change Classification

以下は管理対象外とする。

- Document状態の定義
- Repository現在状態
- Document Lifecycle

これらは各責務を持つ別Documentで管理する。

---

# Mandatory Reviews

以下はArchitecture Reviewを必須とする。

- Constitution
- Governance Specifications
- Kernel
- Plugin README
- Framework README
- Glossary

その他は必要に応じて実施する。

---

# Self-Application Principle

Review Policy自身もArchitecture Reviewの対象とする。

重要な運用ルールも、
他の成果物と同一の品質基準で評価する。

---

# Change Classification

Repositoryの変更は以下の2種類に分類する。

## Structure Change

成果物の責務、構造、章構成、設計に影響する変更。

Architecture Reviewを実施する。

例

- 新しい章の追加
- 責務変更
- Rule追加
- Section削除
- Repository構造変更

---

## Content Update

既存構造の範囲内で内容のみを更新する変更。

Architecture Reviewは不要とする。

例

- Status更新
- Version更新
- 日付更新
- 成果物追加
- Candidate追加
- RepositoryManifestの状態更新

---

# Review Outcomes

レビュー結果は次のいずれかとする。

- Approved
- Approved with Minor Revision
- Revision Required

---

# Review Records

レビュー結果はRepositoryへ保存する。

保存場所はRepository RulesのScope Ruleに従う。

Repository

    Reviews/

Plugin

    Plugins/<Plugin>/Reviews/

---

# Continuous Improvement

Review PolicyはMechanismである。

Evidenceに基づいて継続的に改善する。

---

# Related Documents

- Governance/RepositoryRules.md
- Governance/DocumentLifecycle.md
- RepositoryManifest.md
- Templates/ArchitectureReviewTemplate.md