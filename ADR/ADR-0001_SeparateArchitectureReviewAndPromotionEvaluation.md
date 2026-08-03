# ADR-0001: Separate Architecture Review and Promotion Evaluation

- Status: Approved
- Version: 1.0
- Date: 2026-08-03

---

# Title

Architecture Review と Promotion Evaluation の責務を分離する

---

# Context

ReasonOSでは当初、Architecture Reviewの中で以下を評価することを検討していた。

- Promotability（昇格可能性）
- Reusability（再利用性）

しかし検討を進めた結果、これらはドキュメント品質ではなく、「KernelやFrameworkへ昇格させるか」という設計判断であることが明らかになった。

Architecture Reviewに含めると、レビューの責務が肥大化し、Single Responsibility Principle（SRP）に反する。

---

# Decision

Architecture Reviewは、ドキュメント品質のみを評価する。

評価項目は以下の7項目とする。

1. Purpose
2. Responsibility
3. Universality
4. Stability
5. Consistency
6. Simplicity
7. Testability

一方、

- Promotability
- Reusability

については、Promotion Evaluationとして独立した評価プロセスを設ける。

---

# Consequences

## Positive

- Architecture Reviewの責務が明確になる。
- Promotionの評価基準を独立して改善できる。
- レビュー担当者が判断に迷わなくなる。
- ReviewとADRの役割が明確になる。

## Negative

- Promotion Evaluationという新しいレビュー工程が追加される。

---

# Alternatives Considered

## Alternative A

Architecture Reviewの中でPromotionも評価する。

### Result

不採用

### Reason

レビューの責務が肥大化するため。

---

## Alternative B

Promotion Evaluationを独立したプロセスにする。

### Result

採用

### Reason

責務分離が明確になり、ReasonOS全体の設計と整合するため。

---

# Related Documents

- Templates/ArchitectureReviewTemplate.md
- Constitution/001_ReuseBeforeReinvent.md

---

# Notes

Promotion Evaluationの評価基準は別ドキュメントとして管理する。

Architecture Reviewは設計品質のみを対象とする。