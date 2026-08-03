# Naming Convention

- Version: 1.1
- Status: Approved

---

# Purpose

Naming Conventionは、ReasonOS Repositoryにおける命名規則を定義する。

目的は、

- Repository全体の一貫性を維持すること
- ドキュメントを見つけやすくすること
- 保守性を向上させること

である。

---

# Scope

本規約はRepository全体へ適用する。

対象

- Directories
- Documents
- Constitution
- ADR
- RFC
- Reviews
- Plugins
- Templates

---

# Naming Principles

命名は以下の原則に従う。

- Responsibility First
- Consistency First
- Simplicity First
- Readability First

略称は必要最小限とする。

---

# Directory Naming

ディレクトリはPascalCaseを採用する。

例

```text
CandidateRegistry/
Constitution/
Governance/
Kernel/
Plugins/
Reviews/
Templates/
```

ディレクトリ名は責務を表現する。

---

# Document Naming

通常のドキュメントはPascalCaseを採用する。

例

```text
RepositoryRules.md
DocumentLifecycle.md
ReviewPolicy.md
NamingConvention.md
KernelArchitecture.md
Glossary.md
README.md
```

---

# Constitution

形式

```text
NNN_Name.md
```

例

```text
001_ReuseBeforeReinvent.md
```

番号はApproved後に採番する。

---

# ADR

形式

```text
ADR-XXXX_Title.md
```

例

```text
ADR-0001_SeparateArchitectureReviewAndPromotionEvaluation.md
```

ADR番号はカテゴリ単位で採番する。

Repository ADR

```text
ReasonOS/ADR/
```

Plugin ADR

```text
Plugins/<Plugin>/ADR/
```

---

# RFC

形式

```text
RFC-XXXX_Title.md
```

例

```text
RFC-0001_CandidateRegistry.md
```

RFC番号はカテゴリ単位で採番する。

---

# Review

レビュー文書は対象ドキュメント名を継承する。

形式

```text
<DocumentName>_Review_vX.Y.md
```

例

```text
KernelArchitecture_Review_v1.0.md

001_ReuseBeforeReinvent_Review_v1.0.md
```

---

# Plugin Methods

Framework Methodは以下の形式で命名する。

形式

```text
NN_MethodName.md
```

例

```text
01_MarketDiscovery.md
02_MarketAnalysis.md
03_CompetitionAnalysis.md
```

Method番号の意味および運用ルールは、
Frameworkの設計仕様で定義する。

---

# Extension Rule

新しい命名規則を追加する前に、
既存規則で表現できないかを検討する。

---

# Related Documents

- Governance/RepositoryRules.md
- Governance/DocumentLifecycle.md
- Plugins/ProductInvestment/Framework/README.md
