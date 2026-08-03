# Promotion Policy

- Version: 1.0
- Status: Approved

---

# Purpose

Promotion Policyは、ReasonOS Repositoryにおいて、成果物をDraftまたはReview状態からApprovedへ昇格（Promotion）するための基準と手順を定義する。

Promotionは単なる完成宣言ではない。

Repository全体の品質、一貫性、保守性を維持するためのGovernance Processである。

---

# Scope

本ポリシーはRepository全体へ適用する。

対象:

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

Repository内の既存ルールおよび設計思想と整合していること。

---

## Evidence First

Promotion判断は根拠に基づいて行う。

完成感や主観的判断ではなく、Review結果を基準とする。

---

## Review Before Promotion

正式採用前に必要なReviewを完了する。

---

# Promotion Criteria

成果物は以下の条件を満たした場合にPromotion可能となる。

---

## 1. Responsibility

成果物の目的と責務が明確である。

確認項目:

- Purposeが定義されている
- Scopeが明確である
- 他成果物との責務境界が明確である

---

## 2. Completeness

成果物として必要な内容が完成している。

確認項目:

- 未完成項目が存在しない
- TODOが残っていない
- 必要な関連情報が記載されている

---

## 3. Consistency

Repository全体との整合性が確認されている。

確認対象:

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

Document Lifecycleで定義された状態遷移に従っている。

---

# Promotion Procedure

Promotionは以下の手順で実施する。

Draft
  |
  v
Review
  |
  v
Revision
  |
  v
Approval
  |
  v
Approved

具体的な手順:

1. 成果物作成
2. Self Review実施
3. 必要なArchitecture Review実施
4. 指摘事項修正
5. Review Approval取得
6. StatusをApprovedへ変更
7. Repository Manifest更新

---

# Responsibilities

## Author

責務:

- 成果物を作成する
- Review指摘へ対応する
- Promotion条件を満たす状態へ改善する

---

## Reviewer

責務:

- Responsibilityを確認する
- Architecture整合性を確認する
- Promotion可否を判断する

---

## Repository Maintainer

責務:

- Approved状態を管理する
- Repository Manifestを更新する
- Repository状態を維持する

---

# Promotion Effects

ApprovedへPromotionされた成果物は以下の扱いとなる。

- Repositoryの正式成果物となる
- Authoritative Sourceとして参照可能になる
- 他成果物から利用可能になる
- 変更時はReview Policyに従う

---

# Change After Promotion

Approved成果物も改善可能である。

ただし変更内容に応じて、以下へ分類する。

## Content Update

既存構造を維持した内容変更。

例:

- Status変更
- Version変更
- 日付更新
- 文言修正

---

## Structure Change

成果物の責務、構造、設計へ影響する変更。

例:

- 新しい責務追加
- 章構成変更
- Rule追加
- Scope変更

Structure Changeの場合はArchitecture Reviewを実施する。

---

# Relationship With Other Governance Documents

## RepositoryRules

Repository構造および変更ルールを定義する。

---

## DocumentLifecycle

成果物状態の意味と状態遷移を定義する。

---

## ReviewPolicy

Review方法および変更分類を定義する。

---

## NamingConvention

成果物命名規則を定義する。

---

# Related Documents

- Governance/RepositoryRules.md
- Governance/DocumentLifecycle.md
- Governance/ReviewPolicy.md
- Governance/NamingConvention.md
- RepositoryManifest.md