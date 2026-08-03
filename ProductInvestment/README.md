# Product Investment Plugin

- Version: 1.0
- Status: Draft

---

# Mission

市場・競争・顧客・投資・商品設計を体系化し、
商品投資における意思決定品質を継続的に向上させる。

本PluginはReasonOSの公式Pluginであり、
Plugin Driven Developmentに基づいてKernelの改善へフィードバックを行う。

---

# Purpose

商品開発そのものではなく、

「どの市場へ、どのような商品へ投資すべきか」

という意思決定を支援することを目的とする。

---

# Scope

本Pluginは以下を対象とする。

- 市場選定
- 市場分析
- 市場スコアリング
- 競争分析
- レビュー分析
- 顧客分析
- 工場選定
- 商品仕様策定
- 投資判断
- Launch判断

---

# Out of Scope

本Pluginでは以下は扱わない。

- Amazon広告運用
- 楽天広告運用
- 在庫管理
- 発送業務
- 会計
- CS対応
- デザイン制作

これらは別Pluginまたは外部システムの責務とする。

---

# Architecture

Product Investment Pluginは以下の構成要素で構成される。

- Framework
- Knowledge
- Workflow
- Templates
- Experiments
- ADR
- RFC

---

# Workflow

本Pluginでは次の意思決定プロセスを採用する。

1. 市場候補の抽出
2. 市場スコアリング
3. 競争分析
4. 顧客分析
5. レビュー分析
6. Factory Analysis
7. 商品仕様策定
8. 投資判断（ROI）
9. Launch判断
10. Review

Workflowは実証を通じて継続的に改善する。

---

# Deliverables

本Pluginが生成する成果物の例。

- 市場分析レポート
- 市場スコアリングシート
- Competition Report
- Review Analysis
- Factory Comparison
- Product Specification
- ROI Report
- Launch Report

---

# Relationship with ReasonOS

本PluginはReasonOS Kernelを利用する。

- Constitutionに従う
- Architecture Reviewを受ける
- RFCを通じて改善提案を行う
- ADRにより設計判断を記録する

Pluginで実証された共通概念は、
Promotion Evaluationを経てKernelへの昇格候補となる。

---

# Success Criteria

本Pluginは以下を満たすことを成功とする。

- 商品投資判断の品質が向上する
- 判断根拠を説明できる
- Workflowを再利用できる
- 新しい市場にも適用できる
- ReasonOSへ継続的にフィードバックできる