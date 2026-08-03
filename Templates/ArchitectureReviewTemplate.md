# Architecture Review Template

- Template Version: 1.0
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

他のConstitution・Kernel・
```