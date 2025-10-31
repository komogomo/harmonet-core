# Rules / 01-ALL-AI

このディレクトリは、HarmoNet開発における **AI協働運用ポリシー群** を管理する領域です。  
人間開発者および複数のAIエージェント（Lead AI, Integration AI, Review AI など）が  
共通の原則・手順・出力形式を参照できるように設計されています。

---

## 📘 目的
AI間および人間開発者との協働を円滑にし、  
設計・実装・文書作成における整合性と再現性を確保することを目的とします。

---

## 📂 ファイル一覧
| ファイル名 | 役割 |
|-------------|------|
| **AI Collaborative Development Guideline v1.1.md** | AIチーム全体の運用ガイドライン。GitHub／Drive共有構造を明記。 |
| **harmonet-doc-versioning-policy_v2.1.md** | ドキュメントのバージョン管理および命名規則の定義。 |
| **File-Modification-Checklist-v2.1.md** | ファイル更新時の確認手順およびレビュー項目。 |

---

## 🔗 関連ディレクトリ
- `/docs/common/` … HarmoNet全体の設計書・仕様書の最新版を格納  
- `/Rules/` … 各種運用ルールとAI連携方針を格納  
- `/screen/` … 実装フェーズでの設計参照用ビュー層（Google Drive共有）

---

## 🧭 管理方針
- すべての文書は **Markdown形式（.md）** で保存する。  
- ファイルのバージョン履歴は各文書内の **ChangeLog** に記録する。  
- ファイル名にはバージョン番号を付与し、リンク参照は `_latest.md` 形式を使用する。  
- `README.md` 自体にはバージョン番号を付けない（常に最新状態を維持）。

---

**Created:** 2025-10-31  
**Last Updated:** 2025-10-31  
**Maintainer:** Lead AI（HarmoNet PMO）
