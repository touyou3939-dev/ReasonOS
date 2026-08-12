# ADR-0001: Replace Stage with Method in Product Investment Framework

- Status: Approved
- Date: 2026-08-03

---

# Context

Product Investment Frameworkは当初、
意思決定プロセスを複数の「Stage」で構成する設計を採用していた。

例

- Stage01 Market Selection
- Stage02 Market Analysis
- Stage03 Competition Analysis

しかしFrameworkの設計を進める中で、
Stageという概念には次の問題があることが分かった。

- Stageは固定された順序を連想させる。
- FrameworkとWorkflowの責務が曖昧になる。
- Method単体で再利用しにくい。
- 将来のAI Agentや異なるWorkflowへ適用しにくい。

---

# Decision

FrameworkはStageではなく、
再利用可能なMethodの集合として設計する。

WorkflowはFrameworkに含まれるMethodを組み合わせ、
目的に応じた意思決定プロセスを構成する。

FrameworkはMethodを提供するが、
Methodをどの順序で利用するかは定義しない。

---

# Rationale

この設計により、

- FrameworkはWorkflowへ依存しない。
- WorkflowはFrameworkを利用する。
- Methodは単独でも再利用できる。
- Workflowを複数定義できる。
- 将来AI Agentが独自のWorkflowを構成できる。

Frameworkの責務は
「意思決定方法の提供」に限定される。

Workflowの責務は
「Methodの組み合わせによる意思決定プロセスの定義」とする。

---

# Consequences

## Positive

- Frameworkの再利用性が向上する。
- Workflowを自由に設計できる。
- Method単体の改善が容易になる。
- Frameworkの責務が明確になる。
- AI Agentとの親和性が高くなる。

## Negative

- Workflowを別途設計する必要がある。
- Stageという直感的な表現は使用しないため、
初学者にはWorkflowとの違いを説明する必要がある。

---

# Alternatives Considered

## Alternative 1

Stageベースの設計を維持する。

却下。

理由

StageはWorkflowを固定化してしまい、
Methodの再利用性が低下する。

---

## Alternative 2

Frameworkの中でStageとMethodを併用する。

却下。

理由

責務が重複し、
FrameworkとWorkflowの境界が曖昧になる。

---

# Impact

本ADRにより、

Framework README

Glossary

各Framework Method

は、

StageではなくMethodを前提として設計する。

Workflowは独立した成果物として設計する。

---

# Related Documents

- Kernel/KernelArchitecture.md
- Plugins/ProductInvestment/README.md
- Plugins/ProductInvestment/Glossary.md
- Plugins/ProductInvestment/Framework/README.md