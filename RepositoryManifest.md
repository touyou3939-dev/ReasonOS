# Repository Manifest

- Version: 1.3
- Status: Draft
- Last Updated: 2026-08-12

---

# Purpose

Repository ManifestはReasonOS Repositoryの現在の公式状態（Current State）を記録する。

目的は以下の通りである。

- Repository全体の現在地を把握する。
- Repository構造を一貫して管理する。
- 新しい開発セッションに共通コンテキストを提供する。
- Repositoryの唯一の正本（Single Source of Truth）への入口となる。

Repository Manifestは設計仕様ではない。

Repositoryの現在状態を表現するインデックスである。

---

# Repository Principles

Repository ManifestはRepositoryの現在状態のみを管理する。

以下は管理対象外とする。

- 設計仕様
- 開発計画
- タスク管理
- Current Focus
- Next Recommended Action

これらはそれぞれ責務を持つ成果物で管理する。

---

# Responsibility Boundary

RepositoryManifestはRepositoryの現在状態を記録する。

管理対象:

- Repository Structure
- Document Status
- Current Repository State

以下は管理対象外とする。

- Lifecycle定義
- Reviewルール
- 設計仕様

これらは各責務を持つ別Documentで管理する。

---

# Current Repository Structure

    ReasonOS/

    ├── README.md

    ├── CandidateRegistry/
    ├── Constitution/
    ├── Governance/
    ├── Kernel/
    ├── Plugins/
    ├── Sessions/

    ├── ADR/
    ├── RFC/
    ├── Reviews/
    ├── Templates/

Sessions/ はDevelopment Session記録を格納する。Conversation Context相当であり、正本文書ではないため、Document Status集計の対象外とする。

---

# Repository Status

## Candidate Registry

### Approved Documents

- ConstitutionCandidates.md

---

## Constitution

### Draft


### Approved

- 001_ReuseBeforeReinvent.md
- README.md

---

## Governance

### Approved

- RepositoryRules.md
- DocumentLifecycle.md
- ReviewPolicy.md
- NamingConvention.md
- PromotionPolicy.md

---

## Kernel

### Approved

- KernelArchitecture.md

---

## Plugins

### ProductInvestment

#### Approved

- README.md
- Glossary.md
- Framework/README.md

---

## ADR

### Draft

- ADR-0002_ReasonOSDevelopmentStrategy.md（本Sessionで本文起票。Architecture Review未実施のため次Sessionへ持ち越し）

### Approved


---

# Repository Summary

集計基準: 「Approved Documents」はカテゴリ別の実承認文書数の単純合計とする。Plugins配下の個別文書数は「Plugins配下承認文書数」として別行に記載し、「Plugins」行は製品数を表す。

| Item | Count |
|------|------:|
| Approved Documents | 12 |
| Draft Documents | 1 |
| Constitution | 2 |
| Governance | 5 |
| Kernel Documents | 1 |
| Plugins（製品数） | 1 |
| Plugins配下承認文書数 | 3 |
| ADR | 1 (Draft) |
| RFC | 0 |

Note: v1.2からの変更点は以下の通り。

- Approved Documents集計基準を「カテゴリ内訳の単純合計（Plugins=1扱い）」から「実文書数の積み上げ」に変更（10→12）。
- Current Repository StructureにSessions/を追加。
- ADR-0002_ReasonOSDevelopmentStrategy.mdの本文を起票し、Status: Draftとして登録（Draft Documents 0→1、ADR 0→1）。

Note: README.mdのRepository Structureセクション（Constitution/, Kernel/, ADR/, RFC/, Templates/, Reviews/, ProductInvestment/という旧構造の記載）が、本Manifestの記述と一致していない既知の乖離が残存している。本Updateではスコープ外とし、Next Session Issueとして記録する。

---

# Authoritative Sources

Repository ManifestはRepositoryの入口である。

Repositoryの正式な情報は各成果物を正本とする。

| Information | Authoritative Source |
|-------------|----------------------|
| Repository Structure | RepositoryRules.md |
| Document Lifecycle | DocumentLifecycle.md |
| Review Rules | ReviewPolicy.md |
| Naming Convention | NamingConvention.md |
| Architecture | KernelArchitecture.md |
| Constitution | Constitution/ |
| Candidates | CandidateRegistry/ |

Repository Manifestは各成果物へのインデックスであり、
正本を置き換えるものではない。

---

# Manifest Maintenance

Repository ManifestはVersion 1では手動管理とする。

将来的にはReasonOS DevKitにより自動生成する。

Manifestの更新は以下に従う。

- Repositoryの状態変更はContent Updateとする。
- Manifestの責務変更はStructure Changeとする。

Change ClassificationはReviewPolicy.mdに従う。

---

# Related Documents

- README.md
- Governance/RepositoryRules.md
- Governance/DocumentLifecycle.md
- Governance/ReviewPolicy.md
