# Kernel Architecture

- Version: 1.1
- Status: Approved

---

# Purpose

ReasonOS Kernelは、すべてのPluginが共通で利用する最小限の基盤を提供する。

Kernelはドメイン知識や個別の意思決定ロジックを持たない。

Kernelの目的は、Pluginが一貫した方法で意思決定できる環境を提供することである。

---

# Design Philosophy

ReasonOSはPluginによって進化する。

Kernelは最初から完成させるものではない。

Pluginで実証された共通概念のみをKernelへ取り込む。

Kernelは常に最小構成（Keep the Core Small）を維持する。

---

# Responsibilities

Kernelは次の責務のみを持つ。

## 1. Governance

ReasonOS全体のガバナンスを提供する。

対象

- Constitution
- ADR
- RFC
- Architecture Review
- Document Lifecycle

---

## 2. Decision Process

Pluginが共通で利用する意思決定プロセスの基盤を提供する。

Decision Processの詳細仕様は、本ドキュメントでは定義しない。

---

## 3. Review Process

ReasonOSにおけるレビュー方法を提供する。

レビュー対象

- Constitution
- Kernel
- Plugin

レビュー基準は Architecture Review Template に従う。

---

## 4. Evolution Process

PluginからKernelへの進化を管理する。

Kernelへ新しい概念を追加する場合は、

- RFC
- Promotion Evaluation
- ADR

を経なければならない。

---

# Out of Scope

Kernelは以下を管理しない。

- ドメイン知識
- Framework
- Plugin固有Workflow
- Amazon固有知識
- 商品開発知識
- 株式投資知識
- 法規制知識

これらは各Pluginの責務とする。

---

# Design Principles

Kernelは以下のConstitutionに従う。

- Reuse Before Reinvent
- Plugin Driven Development
- Evidence First
- Core Must Stay Small
- Review Before Promotion

---

# Relationship

```text
Constitution
      │
      ▼
   Kernel
      │
      ▼
   Plugin
   ├── Framework
   ├── Knowledge
   ├── Workflow
   └── Templates
```

- ConstitutionはKernelを統治する。
- KernelはPlugin共通の基盤を提供する。
- PluginはFramework・Knowledge・Workflowを利用して意思決定を実装する。
- Framework・KnowledgeはKernelへ直接依存しない。

---

# Evolution

Kernelは固定ではない。

Pluginで十分に実証された共通概念のみを、

1. RFC
2. Promotion Evaluation
3. ADR

の順で評価し、Kernelへ追加する。

---

# Success Criteria

良いKernelとは、

- 小さい
- 安定している
- Pluginへ依存しない
- 再利用できる
- 長期間維持できる

ことである。

Kernelは機能数ではなく、責務の明確さによって評価される。