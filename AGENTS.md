# AGENTS.md - Project Rules & Guidelines for AI Assistant

## 1. Project Overview & Goal
本專案為一個模組化、可持續擴充的「個人 AI 與程式開發筆記庫網站」。
目標在於透過一套統一的頁面架構與資料格式規範，讓 AI 閱讀本文件後，能快速新增筆記與展示頁面，確保樣式與目錄結構完全一致。

## 2. Directory Structure
  ├── index.html            # 主頁面 (包含標題、導覽列與動態文章卡片區)
  ├── AGENTS.md             # 本規範文件
  ├── content/              # 存放所有 Markdown 筆記
  │   └── first-note.md
  └── data/
      └── articles.json     # 文章索引檔 (動態讀取用)

## 3. UI/UX Style Guidelines
- **Color Scheme**: 暗色調背景 (`#0f172a`)，卡片背景 (`#1e293b`)，文字 (`#f8fafc`)，亮色點綴 (`#38bdf8`)。
- **Layout**: 響應式卡片網格（手機 1 欄，電腦 3 欄），支援點擊閱讀文章。

## 4. Rules for Adding New Content
當需要新增一篇內容時，必須執行以下兩步驟：
1. 在 `content/` 資料夾建立 Markdown 檔案，檔名全小寫用連字號（例如 `content/rag-intro.md`）。
2. 在 `data/articles.json` 註冊該文章資料：
   ```json
   {
     "id": "rag-intro",
     "title": "文章標題",
     "category": "AI",
     "date": "2026-11-08",
     "summary": "簡短摘要",
     "file": "content/rag-intro.md"
   }