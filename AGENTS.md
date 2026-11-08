\# AGENTS.md - Project Rules \& Guidelines for AI Assistant



\## 1. Project Overview \& Goal

本專案為一個「日語文法與高級句型學習筆記庫網站」。

目的在於透過統一的規範，讓 AI 能快速新增日語文法、例句與尊他語自謙語用法，確保網站結構與學習卡片風格一致。



\## 2. Directory Structure

&#x20; ├── index.html            # 主頁面 (展示文法卡片與解析彈窗)

&#x20; ├── AGENTS.md             # 本規範文件

&#x20; ├── content              # 存放所有文法 Markdown 筆記

&#x20; │   └── grammar-mensang.md

&#x20; └── data

&#x20;     └── grammar.json      # 文法索引檔 (動態讀取用)



\## 3. UIUX Style Guidelines

\- Color Scheme 深青綠色調背景 (`#064e3b`)，卡片背景 (`#047857`)，文字 (`#ecfdf5`)，點綴亮綠色 (`#34d399`)。

\- Layout 響應式卡片網格，支援彈窗閱讀完整文法解析與例句。



\## 4. Rules for Adding New Content

新增文法筆記時必須執行：

1\. 在 `content` 資料夾建立 Markdown 檔（例如 `contentgrammar-nisaishite.md`）。

2\. 在 `datagrammar.json` 註冊該文法資料：

&#x20;  ```json

&#x20;  {

&#x20;    id grammar-nisaishite,

&#x20;    title ～に際して  にあたり,

&#x20;    level N2  N1,

&#x20;    date 2026-11-08,

&#x20;    summary 表示在進行某項重要事情、儀式或特別場合時的前置說明與注意事項。,

&#x20;    file contentgrammar-nisaishite.md

&#x20;  }

