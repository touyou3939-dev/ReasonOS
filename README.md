# ReasonOS

> A plugin-driven operating system for continuously improving decision quality.

---

# Vision

ReasonOSは、意思決定能力を継続的に進化させるためのプラットフォームである。

ReasonOS自身はドメイン知識を持たない。

商品開発、株式投資、経営戦略などの知識はPluginとして実装される。

---

# Philosophy

ReasonOSは次の考え方を採用する。

- Small Kernel
- Plugin Driven Development
- Evidence First
- Reuse Before Reinvent

これらの原則はConstitutionによって管理される。

---

# Repository Structure

```text
ReasonOS/

├── Constitution/
├── Kernel/
├── ADR/
├── RFC/
├── Templates/
├── Reviews/
└── ProductInvestment/
```

---

# Repository Guide

## Constitution

ReasonOS全体で長期間維持する設計原則を管理する。

---

## Kernel

すべてのPluginが共通で利用する最小限の基盤を提供する。

Kernelはドメイン知識を持たない。

---

## Plugins

ドメイン固有の知識・Framework・Workflowを提供する。

PluginはReasonOSを実証し、Kernelへフィードバックを行う。

---

## ADR

重要な設計判断を記録する。

---

## RFC

新しい設計・概念・改善案を提案する。

---

## Reviews

Architecture Reviewの履歴を管理する。

---

## Templates

ReasonOSで利用する標準テンプレートを管理する。

---

# Repository Rules

新しい概念を追加する前に、必ず次の順番で検討する。

1. 既存の責務で表現できないか。
2. Why / How / What のどこに属するか。
3. RFCが必要か。
4. Architecture Reviewが必要か。
5. ADRで採用するか。

Constitution番号はApproved後に採番する。

READMEはArchitecture Reviewの対象とする。

---

# Document Lifecycle

ReasonOSの各ドキュメントは、
定義されたLifecycleに従って管理する。

Lifecycleの詳細仕様は、
専用ドキュメントで管理する。

---

# Development Process

```text
Idea
    │
    ▼
RFC
    │
    ▼
Plugin Implementation
    │
    ▼
Architecture Review
    │
    ▼
ADR
    │
    ▼
Kernel Feedback
    │
    ▼
Constitution（必要に応じて）
```

ReasonOSはPluginによる実証を通じて継続的に進化する。

---

# Out of Scope

ReasonOSは以下を提供しない。

- ドメイン固有の知識
- 業務アプリケーション
- AIモデルそのもの
- 特定プラットフォーム向けの実装
- 業務固有の運用ルール

これらはPluginまたは外部システムの責務とする。

---

# References

詳細は各ディレクトリのドキュメントを参照する。

- Constitution
- Kernel
- ADR
- RFC
- Templates
- Reviews
- Plugins

---

# License

To be decided.