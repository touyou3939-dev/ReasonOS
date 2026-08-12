# Reuse Before Reinvent

- Version: 1.0
- Status: Draft

---

# Purpose

Reuse Before Reinventは、ReasonOS Repositoryにおいて新しい概念・責務・仕組みを追加する前に、既存の責務で表現できないかを検討することを求める原則である。

目的は、Repositoryの複雑化を防ぎ、Small Kernelを維持し、長期的な保守性を確保することである。

---

# Scope

本原則はRepository全体（Constitution、Governance、Kernel、Plugins、ADR、RFC、Templates、Reviews）へ適用する。

---

# Principle

新しい概念・機能・ドキュメントを追加する前に、次の順序で確認する。

1. 既存の責務（Document・Plugin・Kernel機能）で表現できないか
2. 既存の仕組みを拡張することで対応できないか
3. 新規追加が本当に必要か

既存の責務で表現できる場合、新しい概念・成果物を追加しない。

---

# Relationship with Repository Rules

本原則は、Governance/RepositoryRules.mdの以下の記述に対応する。

Repository Rulesは本原則の運用手順を定義し、本Constitutionは原則そのものの根拠を定義する。

---

# Rationale

Reuseを優先しない場合、類似した責務を持つDocument・仕組みがRepository内に重複して発生し、次の問題を招く。

- どの成果物が正本か不明瞭になる
- 保守コストが増加する
- Repository構造の一貫性が失われる

Reuse Before Reinventは、これらの問題を未然に防ぐための原則である。

---

# Related Documents

- Governance/RepositoryRules.md
- Kernel/KernelArchitecture.md
- README.md