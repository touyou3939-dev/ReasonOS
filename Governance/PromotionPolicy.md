# Promotion Policy

- Version: 1.0
- Status: Approved

---

# Purpose

Promotion Policyは、ReasonOS Repositoryにおいて、
DraftまたはReview状態の成果物をApprovedへ昇格（Promotion）するための基準と手順を定義する。

Promotionは単なる完成宣言ではない。

Repository全体の品質、一貫性、保守性を維持するためのGovernance Processである。

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
- Reviews

---

# Promotion Principles

Promotionは以下の原則に従う。

## Responsibility First

成果物の責務が明確であること。

既存成果物との責務重複がないこと。

---

## Consistency First

Repository内の既存ルール・設計思想と整合していること。

---

## Evidence First

判断は根拠に基づいて行うこと。

単なる完成感ではなく、Review結果を基準とする。

---

## Review Before Promotion

正式採用前に必要なReviewを完了すること。

---

# Promotion Criteria

成果物は以下の条件を満たした場合にPromotion可能となる。

---

## 1. Responsibility

成果物の目的と責務が明確である。

以下を満たすこと。

- Purposeが定義されている
- Scopeが明確である
- 他成果物との責務境界が明確である

---

## 2. Completeness

成果物として必要な内容が完成している。

以下を含む。

- 未完成項目が存在しない
- TODOが残っていない
- 必要な関連情報が記載されている

---

## 3. Consistency

Repository全体との整合性が確認されている。

確認対象

- Repository Rules
- Document Lifecycle
- Naming Convention
- Architecture Principles

---

## 4. Review Completion

必要なReviewが完了している。

Review結果は以下のいずれかであること。

- Approved
- Approved with Minor Revision

Revision Requiredの場合はPromotionできない。

---

## 5. Lifecycle Compliance

Document Lifecycleで定義された状態遷移に従っていること。

---

# Promotion Procedure

Promotionは以下の手順で実施する。

```text
Draft

 ↓
