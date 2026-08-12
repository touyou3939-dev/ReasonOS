# Constitution

- Version: 1.1
- Status: Approved

---

# Purpose

ConstitutionディレクトリはReasonOS全体で長期間維持する設計原則を管理する。

Constitutionは、Kernel・Plugin・Governanceを含むRepository全体の設計判断の根拠となる。

---

# Scope

Constitutionが対象とするのは、次のような長期安定性が求められる原則のみである。

- 特定の技術・製品・サービスに依存しない
- ReasonOS全体（Kernel・Plugin問わず）に適用できる
- 長期間変更されない

一時的な技術判断や個別Pluginの実装方針はConstitutionの対象外とする。

---

# Numbering Rule

Constitution番号はApproved時に採番する。Candidate段階では番号を付与しない（Governance/RepositoryRules.mdに従う）。

ファイル名は `NNN_Name.md` 形式とする。

---

# Lifecycle

Constitutionドキュメントは Governance/DocumentLifecycle.md に定義された共通Lifecycleに従う。

Draft → Review → Approved → Superseded → Archived

---

# Review

ConstitutionはGovernance/ReviewPolicy.mdにおいてArchitecture Review必須対象と定められている。

---

# Current Documents

現在管理されているConstitution Documentの一覧、およびそのStatusは RepositoryManifest.md を正本とする。

本READMEでは個別Documentの状態を保持しない。

---

# Related Documents

- Governance/RepositoryRules.md
- Governance/DocumentLifecycle.md
- Governance/ReviewPolicy.md
- RepositoryManifest.md