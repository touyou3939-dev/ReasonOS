# Repository Manifest

- Version: 1.4
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


### Approved

- ADR-0001_SeparateArchitectureReviewAndPromotionEvaluation.md
- ADR-0002_ReasonOSDevelopmentStrategy.md（Session 009でArchitecture Review実施、Approved with Minor Revisionを反映しv1.1でApproved昇格）

---

# Repository Summary

集計基準: 「Approved Documents」はカテゴリ別の実承認文書数の単純合計とする。Plugins配下の個別文書数は「Plugins配下承認文書数」として別行に記載し、「Plugins」行は製品数を表す。

| Item | Count |
|------|------:|
| Approved Documents | 14 |
| Draft Documents | 0 |
| Constitution | 2 |
| Governance | 5 |
| Kernel Documents | 1 |
| Plugins（製品数） | 1 |
| Plugins配下承認文書数 | 3 |
| ADR | 2 (Approved) |
| RFC | 0 |

Note: v1.3からの変更点は以下の通り。

- ADR-0001_SeparateArchitectureReviewAndPromotionEvaluation.md（Status: Approved）がRepository内に既に存在していたにもかかわらず、v1.3までADRセクションへ未登録だったため追加登録した（登録漏れの是正）。
- ADR-0002_ReasonOSDevelopmentStrategy.mdのArchitecture Reviewを実施し、Approved with Minor Revisionの指摘を反映のうえv1.1へ改訂、Draft→Approvedへ昇格した。
- 上記2件の反映により、Approved Documents 12→14、Draft Documents 1→0、ADR「1 (Draft)」→「2 (Approved)」に変更。

Note: README.mdのRepository Structureセクション（Constitution/, Kernel/, ADR/, RFC/, Templates/, Reviews/, ProductInvestment/という旧構造の記載）が、本Manifestの記述と一致していない既知の乖離が残存している。引き続きNext Session Issueとして記録する。

Note: Session 009にて、Plugins/ADR/ADR-0001_Replace Stage with Method in Product Investment Framework.md（ファイル名はADR-0001だが本文見出しはADR-0002、格納先もGovernance/NamingConvention.mdが定める`Plugins/<Plugin>/ADR/`ではなく`Plugins/ADR/`直下）という命名・格納規則不整合を新たに発見した。本Updateではスコープ外とし、Next Session Issueとして記録する。

Note: Session 009にて、Constitution/001_ReuseBeforeReinvent.md・Constitution/README.md・Plugins/ProductInvestment/README.mdの3文書について、実文書ヘッダーのStatusが「Draft」であるにもかかわらず、本Manifest上は「Approved」として扱われている不整合を新たに発見した（001はArchitecture Review結果が"Approved with Minor Revision"のまま文書ヘッダーへ未反映と見られる）。本Updateではスコープ外とし、Next Session Issueとして記録する。上記3文書の集計上の扱い（Constitution: 2, Plugins配下承認文書数: 3への算入）は、次Session確認まで暫定的に現状維持する。

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