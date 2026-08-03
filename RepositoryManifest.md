# Repository Manifest

- Version: 1.1
- Status: Approved
- Last Updated: YYYY-MM-DD

---

# Purpose

Repository Manifestは、ReasonOS Repositoryの現在の公式状態（Current State）を記録する。

目的は、

- Repository全体の現在地を把握すること
- Repository構造を一貫して管理すること
- 新しい開発セッションへ共通コンテキストを提供すること

Repository Manifestは設計仕様ではない。

Repositoryの現在状態を表現するためのインデックスである。

---

# Manifest Principles

Repository Manifestは、

Repositoryの「現在状態(Current State)」のみを管理する。

Repositoryの設計、運用ルール、開発計画は管理対象外とする。

---

# Current Repository Structure

現在のRepository構造

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

### Categories

- Constitution Candidates

---

## Constitution

### Approved

- 001_ReuseBeforeReinvent.md

---

## Governance

### Approved

- RepositoryRules.md
- DocumentLifecycle.md
- NamingConvention.md

### Draft

- ReviewPolicy.md
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
| Approved Documents | |
| Draft Documents | |
| Constitution | |
| Governance | |
| Kernel Documents | |
| Plugins | |
| ADR | |
| RFC | |

---

# Manifest Generation

Repository Manifestは将来的にRepositoryから自動生成されることを前提とする。

Version 1では手動管理とする。

---

# Related Documents

- README.md
- Governance/RepositoryRules.md
- Governance/DocumentLifecycle.md