# AI 影片收藏 Wiki 關聯圖 / Relationship graph

- 頁面 / Page: [graph/index.html](index.html) · [English](index.html?lang=en)
- 產生時間 / Generated: 2026-11-02 00:03 (UTC+8)
- 來源 commit / Source commit: `1c8a9de525fc208b4cffe1c1253211e146592e78` (ChuangMin/brian-ai-wiki, main)
- 規模 / Size: 247 nodes · 454 edges · 12 communities · 90 entries · index.html 284914 bytes

## 怎麼產生的 / How it is built

全程不呼叫 LLM、不需要任何 API key。/ No LLM calls and no API keys.

1. `md_extract.py`：讀 `README.md`、`docs/*.md`、`demos/demos.json` 的 Markdown 結構，抽出節點（首頁、分類、條目、來源影片、可信度標籤、GitHub 擁有者、Demo、15 個關鍵字概念）與連線。實線 = wiki 明寫的關係（`references`、`cites`，EXTRACTED）；虛線 = 關鍵字比對推論的 `conceptually_related_to`（INFERRED，信心 0.65）。
2. [graphify](https://pypi.org/project/graphifyy/)（`graphifyy`）的 build / cluster / report 建圖並自動分群；群組名稱用規則命名（最多節點的分類檔名＋連線最多的兩個節點）。
3. `graphify export html` 產生互動圖，再由 `wrap_page.py` 加上標題、中文說明、「回 wiki 首頁」連結和「中文 | English」切換（`?lang=en` 直接開英文）。
4. vis-network 9.1.6 從 unpkg 載入（固定版本＋SRI 雜湊），失敗時改用 jsDelivr 同一檔案。
5. 以 headless Chrome 檢查沒有 console 錯誤並截圖（`screenshot.png`）。

## 重建 / Rebuild

新增條目後，在產生端執行 / After adding entries, rerun:

```bash
/workspace/wiki-src/build_graph.sh /path/to/brian-ai-wiki --pull --package /workspace/wiki-handoff/sync-graph.tar.gz
```

這個資料夾的檔案都是產生出來的，請不要手動編輯。/ Files in this folder are generated; do not hand-edit.
