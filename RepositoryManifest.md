# Repository Manifest

- Version: 1.0
- Status: Approved
- Last Updated: 2026-08-03

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

# Current Repository Structure

```text
ReasonOS/

├── README.md

├── CandidateRegistry/
├── Constitution/
├── Governance/
├── Kernel/
├── Plugins/

├── ADR/
├── RFC/
├── Reviews/
├── Templates/
```

---

# Repository Status

## Candidate Registry

### Approved Documents

- ConstitutionCandidates.md

---

## Constitution

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

- README.md
- Glossary.md
- Framework/README.md

---

# Repository Summary

| Item | Count |
|------|------:|
| Approved Documents | 8 |
| Draft Documents | 0 |
| Constitution | 1 |
| Governance | 5 |
| Kernel Documents | 1 |
| Plugins | 1 |
| ADR | 0 |
| RFC | 0 |

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