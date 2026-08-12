# Architecture Review Template

- Template Version: 1.1
- Status: Approved

---

# Document Information

| Item | Value |
|------|------|
| Document | |
| Version | |
| Author | |
| Reviewer | |
| Review Date | |
| Status | Draft / Review / Approved / Frozen |

---

# Review Criteria

## 1. Purpose

### Objective

ドキュメントの目的は明確か。

### Checklist

- [ ] 目的が一文で説明できる
- [ ] ReasonOS全体との関係が明確
- [ ] 責務が明確である

### Review Comments

---

## 2. Responsibility

### Objective

責務は一つに限定されているか。

### Checklist

- [ ] Single Responsibilityになっている
- [ ] 他ドキュメントと責務が重複しない
- [ ] Responsibilityが適切に分離されている

### Review Comments

---

## 3. Universality

### Objective

ReasonOS全体で利用できる設計になっているか。

### Checklist

- [ ] Product Pluginで利用できる
- [ ] Stock Pluginでも利用できる
- [ ] 特定ドメインに依存しない

### Review Comments

---

## 4. Stability

### Objective

長期間変更されない設計になっているか。

### Checklist

- [ ] 一時的な技術に依存しない
- [ ] 特定サービス・製品に依存しない
- [ ] 長期間利用できる可能性が高い

### Review Comments

---

## 5. Consistency

### Objective

他のConstitution・Kernel・Governance（Repository Rules / Review Policy / Document Lifecycle等）の既存ルールと矛盾していないか。

### Checklist

- [ ] 既存のConstitutionと矛盾しない
- [ ] Kernelの設計思想と一致している
- [ ] Governanceの既存ルールと矛盾しない

### Review Comments

---

## 6. Simplicity

### Objective

構成・記述が必要以上に複雑になっていないか。

### Checklist

- [ ] 不要な概念を含まない
- [ ] 構成がシンプルである
- [ ] 目的達成に必要な最小限の内容である

### Review Comments

---

## 7. Testability

### Objective

原則・設計の妥当性を、実際のPlugin実装やDocument運用を通じて検証できるか。

### Checklist

- [ ] Plugin実装を通じて検証できる
- [ ] 妥当性を判断する基準が明確である
- [ ] 再レビュー時に効果を確認できる

### Review Comments

---

# Review Summary

## Strengths

---

## Concerns

---

## Improvement Suggestions

---

# Final Decision

| Item | Result |
|------|--------|
| Purpose | |
| Responsibility | |
| Universality | |
| Stability | |
| Consistency | |
| Simplicity | |
| Testability | |

---

# Overall Result

Approved / Approved with Minor Revision / Revision Required

---

# Next Action

---

# Related Documents

- Governance/ReviewPolicy.md
- Governance/DocumentLifecycle.md
- RepositoryManifest.md