# Review Policy

- Version: 1.0
- Status: Draft

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

# Review Outcomes

レビュー結果は次のいずれかとする。

- Approved
- Approved with Minor Revision
- Revision Required

---

# Review Records

レビュー結果はRepositoryへ保存する。

保存場所はRepository RulesのScope Ruleに従う。

例

Repository全体

```
Reviews/
```

Plugin

```
Plugins/<Plugin>/Reviews/
```

---

# Continuous Improvement

Review PolicyはMechanismである。

運用を通じてEvidenceを蓄積し、
継続的に改善する。

---

# Related Documents

- Governance/RepositoryRules.md
- Governance/DocumentLifecycle.md
- Templates/ArchitectureReviewTemplate.md