# Session Log Template

Status: Template

Version: 1.0

---

# Session Information

**Session ID**

Session XXX

**Date**

YYYY-MM-DD

**Duration**

(Optional)

**Repository Version**

(Current Repository Version)

---

# Objective

今回の開発セッションで達成する目的を記述する。

---

# Target Deliverables

今回完成を目指す成果物を列挙する。

---

# Completed Deliverables

今回完成した成果物を列挙する。

例

- Governance/PromotionPolicy.md
- Reviews/GovernanceArchitectureReview-001.md

---

# Repository Changes

Repositoryへ反映された変更内容を記録する。

例

- PromotionPolicy.md promoted to Approved
- Repository Manifest updated

---

# Major Decisions

セッション中に決定した重要事項を記録する。

Decision 001

内容

Reason

決定理由

Impact

Repositoryへの影響

（必要に応じて追加）

---

# Review Summary

実施したReviewを記録する。

| Review | Result |
|---------|--------|
| Document Review | PASS |
| Architecture Review | PASS |

実施しなかった場合は「Not Applicable」とする。

---

# Open Questions

未解決事項を記録する。

解決済みであれば

None

と記載する。

---

# Risks

現在認識しているリスクを記録する。

存在しなければ

None

と記載する。

---

# Next Session

次回実施予定の内容を記録する。

例

Kernel Architecture Review

---

# Repository Status After Session

Repositoryの状態変化を簡潔に記録する。

例

Governance Layer Version 1 completed.

---

# Lessons Learned

今回得られた知見や改善点を記録する。

これはRepositoryではなく、開発プロセス改善のための情報である。

---

# References

今回参照した主要な成果物を記録する。

例

- RepositoryManifest.md
- PromotionPolicy.md
- ReviewPolicy.md

---## Session Log Output Rule

Session Logおよびその他のMarkdown成果物を提示する場合、
ユーザーがそのまま.mdファイルへコピーできる形式で提示する。

### Rules

- Markdown本文のみを提示する
- 不要な識別子や内部情報を混入しない
- 外側コードブロック内にMarkdownコードブロックを入れない
- Markdown内の図表現は、コピー互換性を優先する
- Mermaid等の表示依存形式を使用する場合は明示する

### Diagram Representation

標準形式:

    1 Session = 1 Issue = 1 Conclusion

    1 Issue
        |
        +-- N Documents
                |
                +-- N Reviews

理由:

- Git管理される.mdファイルとの互換性を維持するため
- ChatGPTからのコピー時に構造崩れを防ぐため