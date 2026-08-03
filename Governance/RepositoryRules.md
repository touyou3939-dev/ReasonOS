# Repository Rules

- Version: 1.1
- Status: Approved

---

# Purpose

Repository Rulesは、ReasonOS Repository全体の運用ルールを定義する。

目的は、

- Repository構造の一貫性を保つこと
- 成果物の責務を明確にすること
- ドキュメントの配置ルールを統一すること
- Repository変更プロセスを一貫して管理すること

である。

---

# Scope

本ルールはRepository全体へ適用する。

対象

- Constitution
- Governance
- Kernel
- Plugins
- ADR
- RFC
- Reviews
- Templates

---

# Repository Principles

Repositoryは責務単位で構成する。

新しいフォルダ・ドキュメントを追加する前に、

既存の責務で表現できないかを検討する。

---

# Scope Rule

ADR・RFC・Reviewは、

最も影響範囲（Scope）が近い場所へ保存する。

## Repository Scope

ReasonOS全体へ影響するもの

保存場所

ReasonOS/

- ADR/
- RFC/
- Reviews/

---

## Plugin Scope

Plugin固有のもの

保存場所

Plugins/<Plugin>/

- ADR/
- RFC/
- Reviews/

---

# Constitution Rule

Constitution番号はApproved時に採番する。

Candidateには番号を付与しない。

---

# Review Rule

以下はArchitecture Reviewを必須とする。

- Constitution
- Kernel
- Plugin README
- Plugin Framework
- Glossary

その他は必要に応じてReviewを実施する。

---

# Lifecycle

各ドキュメントはDocument Lifecycleに従って管理する。

Lifecycleの詳細は別ドキュメントで定義する。

---

# Issue Driven Development

ReasonOSの開発はIssueを中心に管理する。

Issueは解決すべき問題または改善対象を定義する単位であり、
Repository変更の目的を明確化する。

---

## Development Session

Development Sessionは、
1つのIssueを解決するための作業単位である。

原則として以下の関係を持つ。

```
1 Session = 1 Issue = 1 Conclusion
```

ただし、Issueを解決するための変更対象DocumentおよびReviewは複数存在してよい。

---

## Issue and Document Relationship

1つのIssueは複数のDocument変更を含むことができる。

例:

```
Issue

    ↓

Change Target

    ├── Document A
    │
    ├── Document B
    │
    └── Document C

    ↓

Review

    ↓

Issue Close
```

IssueとDocumentは1対1ではなく、
Issueは変更対象Documentを束ねる上位概念として扱う。

---

## Review Relationship

ReviewはDocument単位で実施する。

理由:

- Documentごとに責務が異なるため
- Version管理がDocument単位で行われるため
- 変更履歴を追跡可能にするため

したがって、

```
1 Issue

    ↓

N Documents

    ↓

N Reviews
```

となる。

---

## Issue Completion Criteria

Issueは以下を満たした場合にCloseする。

- Issueの目的が達成された
- 必要なDocument変更が完了した
- 対象DocumentのReviewが完了した
- Repository状態が更新された

---

## Relationship with Proposal

ProposalはIssueを解決するための設計案である。

ProposalはIssueそのものではなく、
Issue解決過程で必要に応じて作成される。

```
Issue

    ↓

Proposal (必要な場合)

    ↓

Implementation

    ↓

Review
```

単純な変更の場合、
Proposalを作成せずIssue内で完結してよい。

---

# Future Extension

Repository RuleはMechanismである。

Evidenceに基づいて継続的に改善する。

---

# Naming Convention

## Directories

- PascalCase
- Singular form
- Responsibility-based name

Examples

- CandidateRegistry
- Constitution
- Governance
- Kernel
- Plugins

---

## Documents

General documents

- PascalCase.md

Examples

- RepositoryRules.md
- KernelArchitecture.md

Constitution

- NNN_Name.md

Examples

- 001_ReuseBeforeReinvent.md

ADR

- ADR-0001_Title.md

RFC

- RFC-0001_Title.md