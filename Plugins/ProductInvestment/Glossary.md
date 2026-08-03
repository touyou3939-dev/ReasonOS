# Product Investment Plugin Glossary

- Version: 1.1
- Status: Approved

---

# Purpose

本Glossaryは、Product Investment Pluginで使用する用語を統一することを目的とする。

Framework・Knowledge・Workflow・Reviewにおいて、
一貫した意味で用語を利用できるようにする。

本Glossaryは概念を定義するものであり、
分析方法やRepository構成は定義しない。

---

# Terms

## Market

商品を投入する対象市場。

Marketは意思決定における最上位の分析対象であり、
複数のSegmentを含む場合がある。

**Example**

- 防災用品市場
- ガーデンライト市場
- 冷感寝具市場

---

## Segment

Marketを顧客・用途・価格帯・利用シーンなどで細分化した単位。

Segmentは分析および投資判断の対象となる。

**Example**

冷感寝具市場

- 敷きパッド
- タオルケット
- 肌掛け布団

---

## Framework

意思決定を支援するための再利用可能な分析方法。

Frameworkは個別の知識ではなく、
分析手順・評価方法・判断プロセスを提供する。

---

## Knowledge

意思決定に利用する知識。

Knowledgeには事実、経験、法規制、業界情報などが含まれる。

Knowledgeは分析方法を定義しない。

---

## Workflow

Frameworkを適用する順序。

Workflowは実務上の意思決定プロセスを表現する。

---

## Template

分析結果を一定の形式で記録するための雛形。

Templateは成果物の品質と再利用性を向上させる。

---

## Evidence

意思決定を支える客観的根拠。

Evidenceは投資判断、Review、ADRの基礎となる。

---

## Review

成果物の品質を評価するプロセス。

Reviewでは責務、一貫性、再利用性、保守性などを評価する。

---

## Investment Decision

市場へ投資するかどうかを判断するプロセス。

Product Investment Pluginにおける最終的な意思決定である。

---

# Naming Rules

- 一つの概念には一つの名称を使用する。
- 同じ名称に複数の意味を持たせない。
- 定義は簡潔かつ客観的に記述する。
- 分析方法はFrameworkで管理する。
- 知識はKnowledgeで管理する。
- Repository構成や実装方法は定義しない。

---

# Scope

本GlossaryはProduct Investment Pluginで利用する概念を定義する。

他Pluginでも利用可能な概念が確認された場合は、
RFCおよびArchitecture Reviewを経て共通Glossaryへの昇格を検討する。