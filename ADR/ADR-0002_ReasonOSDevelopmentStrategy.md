# ADR-0002: ReasonOS Development Strategy

- Status: Draft
- Version: 1.0
- Last Updated: 2026-08-12

---

# Context

ReasonOSはSmall Kernel、Plugin Driven Development、Evidence First、Reuse Before Reinventという4つの原則をPhilosophyとして掲げている（README.md参照）。これらの原則を実際の開発サイクルに落とし込む際、どのような順序・手順で新しい概念やドメイン知識をRepositoryへ取り込むかが定義されていなければ、原則は実運用上の拘束力を持たない。

本ADRは、README.mdに既に記載されているDevelopment Processの流れ（Idea → RFC → Plugin Implementation → Architecture Review → ADR → Kernel Feedback → Constitution）を、正式な開発戦略として採用することの決定を記録するものである。

現時点でRepository内にADR-0001に相当する文書は存在せず、Repository Statusにも登録されていない。この点は本ADRのスコープ外の問題として、別途Open Questionとして扱う。

---

# Decision

ReasonOSの開発戦略として、以下を正式に採用する。

1. 新しいアイデア（Idea）は、まずRFCとして提案する。
2. RFCで合意された概念は、Kernelそのものへ直接実装せず、まずPluginとして実装し実証する。
3. Plugin実装がKernelの責務境界に影響する可能性がある場合、Architecture Reviewを実施する。
4. Architecture Reviewを経て採用が決定した重要な設計判断は、ADRとして記録する。
5. Plugin実装を通じて得られた知見のうち、Kernelとして一般化すべきものはKernel Feedbackとしてフィードバックする。
6. Kernel Feedbackの中でも、ReasonOS全体で長期間維持すべき原則に相当するものは、必要に応じてConstitutionへ昇格する。

この開発戦略は、Governance/RepositoryRules.mdが定める「新しい概念を追加する前の検討順序（既存責務で表現できるか→Why/How/What分類→RFC要否→Architecture Review要否→ADR化）」と整合するものとして位置づける。

---

# Consequences

## Positive

- Kernelへの性急な機能追加を防ぎ、Small Kernel原則を実務レベルで担保できる。
- Plugin単位での実証（Evidence First）を経てからKernelへ反映する流れが明確になる。
- 重要な設計判断がADRとして記録されることで、将来のセッションが過去の意思決定の背景を追跡できる。

## Negative

- Idea起票からConstitution昇格までの経路が長く、開発速度が犠牲になる可能性がある。
- 各ステップ（RFC / Architecture Review / ADR / Kernel Feedback）の要否判断がGovernance/RepositoryRules.mdの定性的な基準に依存しており、判断者によるブレが生じうる。

## Follow-ups

- ADR-0001が現状Repository Status上に存在しない点の扱いを、Open Questionとして次セッション以降で確認する。
- 本ADRの内容がArchitecture Review未実施のままDraftである点を、次セッションでReviewしApproved昇格の可否を判断する。

---

# Alternatives Considered

## Kernelへの直接実装を許容する

新しい概念をPlugin経由でなくKernelへ直接実装する案。開発速度は上がるが、Small Kernel原則およびReuse Before Reinvent原則（既存責務で表現できるかの事前検討）と矛盾するため採用しなかった。

## ADRを経ずKernel Feedbackへ直接反映する

Architecture ReviewとADRのステップを省略し、Plugin実装から直接Kernel Feedbackへ進む案。重要な設計判断の記録が失われ、将来のセッションが意思決定の背景を追跡できなくなるため採用しなかった。

---

# Related Documents

- README.md（Philosophy, Development Process）
- Governance/RepositoryRules.md
- Governance/ReviewPolicy.md
- Governance/DocumentLifecycle.md
- Governance/PromotionPolicy.md
