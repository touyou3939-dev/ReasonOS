# Repository Manifest

- Version: 1.6
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

    ├── docs/  (Legacy Archive)

Sessions/ はDevelopment Session記録を格納する。Conversation Context相当であり、正本文書ではないため、Document Status集計の対象外とする。

docs/ は、正式なRFC/ADR運用（Idea→RFC→Plugin Implementation→Architecture Review→ADR）確立以前に蓄積された議論記録（ChatGPTとの議論等）を格納するLegacy Archiveである。個別文書内のStatus表記（例: Accepted）はArchive内の合意状態を示すものであり、ReasonOSの正式なDocument Status（Approved/Draft）体系とは別のものとして扱う。Document Status集計の対象外とする。docs/内の内容をReasonOSの正式な設計として採用する場合は、既存のChange Control（責務確認→Why/How/What分類→RFC要否判断→Review要否判断→ADR化検討）を経る必要がある。

---

# Repository Status

## Candidate Registry

### Approved Documents

- ConstitutionCandidates.md

---

## Constitution

### Draft

- README.md

### Approved

- 001_ReuseBeforeReinvent.md

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

- Glossary.md
- Framework/README.md
- ADR/ADR-0001_Replace Stage with Method in Product Investment Framework.md

#### Draft

- README.md

---

## ADR

### Draft


### Approved

- ADR-0001_SeparateArchitectureReviewAndPromotionEvaluation.md
- ADR-0002_ReasonOSDevelopmentStrategy.md（Session 009でArchitecture Review実施、Approved with Minor Revisionを反映しv1.1でApproved昇格）

---

## Docs (Legacy Archive)

Document Status集計の対象外。正式なRFC/ADR運用確立以前の議論記録を保持する領域として、参考記録扱いとする。

- docs/proposals/P0001-Define the current agreed understanding of ReasonOS.md（Archive内Status: Accepted）

---

# Repository Summary

集計基準: 「Approved Documents」はカテゴリ別の実承認文書数の単純合計とする。Plugins配下の個別文書数は「Plugins配下承認文書数」として別行に記載し、「Plugins」行は製品数を表す。docs/（Legacy Archive）はいずれの集計にも含めない。

| Item | Count |
|------|------:|
| Approved Documents | 13 |
| Draft Documents | 2 |
| Constitution | 1 |
| Governance | 5 |
| Kernel Documents | 1 |
| Plugins（製品数） | 1 |
| Plugins配下承認文書数 | 3 |
| ADR | 2 (Approved) |
| RFC | 0 |

Note: v1.5からの変更点は以下の通り。

- Sessions/Development_Session_010.mdのNext Session Issue優先順位1・2への対応として、README.mdのRepository Structureセクション（Constitution/, Kernel/, ADR/, RFC/, Templates/, Reviews/, ProductInvestment/という旧構造の記載）を、本Manifestの現行構造と整合する内容へ修正した。
- docs/フォルダの正式な扱いを決定した。正式なRFC/ADR運用確立以前の議論記録（ChatGPTとの議論等）を格納するLegacy Archiveと位置づけ、Current Repository StructureおよびRepository Statusへ新規登録した。Document Status集計の対象外とし、正式採用には既存のChange Controlを経る必要があることを明記した。
- 上記反映により、README.mdとRepositoryManifest.mdのRepository Structure記載間の既知の乖離（v1.4 Note記載）を解消した。

Note: v1.4からの変更点は以下の通り。

- Reviews/Constitution/001_ReuseBeforeReinvent_Review_v1.0.md（Overall Result: Approved with Minor Revision、Next Action: Status Approvedへ昇格）に基づき、Constitution/001_ReuseBeforeReinvent.mdのStatusをDraftからApprovedへ昇格した（Version 1.0のまま据え置き）。
- Constitution/README.md・Plugins/ProductInvestment/README.mdについては該当するArchitecture Reviewの実施記録が確認できなかったため、実ヘッダー通りDraftとして扱うこととし、Manifest上の集計をApprovedからDraftへ是正した。
- Plugins/ADR/ADR-0001_Replace Stage with Method in Product Investment Framework.md（本文見出しはADR-0002だった）を、Governance/NamingConvention.mdの規定する`Plugins/<Plugin>/ADR/`形式に合わせてPlugins/ProductInvestment/ADR/へ移動し、本文見出しをADR-0001へ修正のうえ、Manifestへ新規登録した。
- 上記反映により、Approved Documents 14→13、Draft Documents 0→2、Constitution Approved 2→1・Draft 0→1、Plugins配下承認文書数は3のまま（ProductInvestment/README.mdが除外され、代わりにADR-0001が新規登録された）。

Note: Session 010にて、Constitution/README.mdのNumbering Rule（「Constitution番号はApproved時に採番する」）と、001_ReuseBeforeReinvent.mdがDraft段階から既に「001」の番号を保持していた実態との不整合を新たに発見した。本Updateではスコープ外とし、Next Session Issueとして記録する。

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
