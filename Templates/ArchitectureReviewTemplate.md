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
- [ ] 責務が曖昧でない

### Review Comments

---

## 2. Responsibility

### Objective

責務は一つに限定されているか。

### Checklist

- [ ] Single Responsibilityになっている
- [ ] 他のドキュメントと責務が重複しない
- [ ] Responsibilityが適切に分離されている

### Review Comments

---

## 3. Universality

### Objective

複数Pluginで利用できるか。

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
- [ ] Amazon固有になっていない
- [ ] 10年後も利用できる可能性が高い

### Review Comments

---

## 5. Consistency

### Objective

他のConstitution・Kernel・Pluginと矛盾しないか。

### Checklist

- [ ] 他Principleと矛盾しない
- [ ] Kernel設計と整合する
- [ ] Plugin設計と整合する

### Review Comments

---

## 6. Simplicity

### Objective

必要以上に複雑になっていないか。

### Checklist

- [ ] 不要な概念がない
- [ ] 説明が簡潔
- [ ] 読みやすい

### Review Comments

---

## 7. Testability

### Objective

実際のPluginで検証可能か。

### Checklist

- [ ] Product Pluginで試せる
- [ ] 実務で確認できる
- [ ] 成功・失敗を判断できる

### Review Comments

---

## 8. Evolution

### Objective

将来改善できる設計になっているか。

### Checklist

- [ ] RFCで改善可能
- [ ] ADRへ記録できる
- [ ] Coreへの昇格条件が考慮されている

### Review Comments

---

# Review Summary

## Strengths

-

## Concerns

-

## Improvement Suggestions

-

---

# Final Decision

| Item | Result |
|------|--------|
| Purpose | ☐ Pass ☐ Review ☐ Fail |
| Responsibility | ☐ Pass ☐ Review ☐ Fail |
| Universality | ☐ Pass ☐ Review ☐ Fail |
| Stability | ☐ Pass ☐ Review ☐ Fail |
| Consistency | ☐ Pass ☐ Review ☐ Fail |
| Simplicity | ☐ Pass ☐ Review ☐ Fail |
| Testability | ☐ Pass ☐ Review ☐ Fail |
| Evolution | ☐ Pass ☐ Review ☐ Fail |

---

# Overall Result

- [ ] Approved
- [ ] Needs Revision
- [ ] Rejected

---

# Next Action

-