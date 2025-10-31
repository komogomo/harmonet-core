# 🧭 HarmoNet ファイル命名規則 v1.0

## 🪶 基本構文
```
[2桁章番号]-[画面名]-[機能名または部品名]_v[メジャー].[マイナー].[拡張子]
```

### 例
```
00-login-feature-overview_v1.0.md  
01-home-ui-layout_v2.1.md  
02-board-translation-function_v1.2.md  
03-common-button-component_v1.0.md  
04-system-architecture-overview_v1.1.md
```

---

## 🧩 記号ルール

| 記号 | 用途 | 説明 |
|------|------|------|
| `-（ハイフン）` | 論理的区切り（階層・カテゴリ） | フォルダ名・画面名・機能名を連結するために使用 |
| `_（アンダーバー）` | バージョン・派生識別 | `_v1.0` `_v2.1` `_with-gpt-comments` などに限定 |
| `.` | 拡張子区切り | `.md`, `.html`, `.jsx`, `.docx` など |

---

## 🧭 命名の意味体系

| 構成要素 | 意味 | 例 |
|-----------|------|----|
| `[00]` | 表示順制御。二桁で統一（01, 02, 03…） | `02-board` |
| `[画面名]` | login / home / board / common / system / designなど | `03-common` |
| `[機能名または部品名]` | feature, layout, component, translation, etc. | `03-common-button-component` |
| `_vX.X` | バージョン | `_v1.1`, `_v2.0` |
| `[拡張子]` | ファイルタイプ | `.md`, `.html`, `.jsx`, `.png` |

---

## 🧠 実際のディレクトリ例

```
HarmoNet/
└── docs/
    ├── 00-login-feature-overview_v1.0.md
    ├── 01-home-ui-structure_v2.1.md
    ├── 02-board-translation-function_v1.1.md
    ├── 03-common-header-component_v1.0.md
    ├── 03-common-footer-component_v1.0.md
    ├── 03-common-layout-guide_v1.0.md
    ├── 04-system-architecture-overview_v1.0.md
    └── 05-integration-progress-report_v2.0.md
```

---

## 💡 運用上のポイント

1. **ハイフンは“読むため”の区切り。**  
　ClaudeやGPTにとっても自然言語処理的に識別しやすい。

2. **アンダーバーは“識別用”。**  
　ファイル群を比較するときに `_v` 以降で差分が明確。

3. **バージョンは常に `_v` から始める。**  
　将来的にAIが差分検出する際にパターン化しやすい。

---

## 📘 派生ファイル命名（AIコメントなど）

| 用途 | 命名例 |
|------|--------|
| GPTコメント付 | `02-board-feature-design_with-gpt-comments_v1.0.md` |
| Claude統合版 | `02-board-feature-design_with-claude-review_v2.0.md` |
| Gemini分析付 | `02-board-feature-design_with-gemini-summary_v2.0.md` |

---

## 🎯 運用目的

この命名規則は、HarmoNetプロジェクトの設計書・UIコード・統合資料を対象とし、  
ファイルのソート安定性・AI可読性・Git運用効率を最大化するための基準である。  
すべてのAI（Claude, GPT, Gemini, Copilot）はこの規則を共通基盤として参照する。
