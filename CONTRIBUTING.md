# 貢獻說明

新的 Facebook Reel 請追加在既有內容後面。不要改寫既有條目的名稱、說明、星數或連結。星數是查詢當下的快照；若要更新，連查詢日期一起改。

## 條目格式

每一筆用同一組欄位。分類決定放在哪一頁，其餘四欄寫進該頁的表格，新列加在表格最下方：

| 欄位 | 怎麼填 |
| --- | --- |
| 分類 | 下面六個分類之一，對應一個 Markdown 檔 |
| 名稱 | 工具或主題名稱，連結到該筆的 URL |
| 說明 | 這支影片在講什麼，沿用原意，不另加評價 |
| 星數 | GitHub star，千分位逗號（例如 `110,828`）。沒有 GitHub 專案填 `—` |
| 出處 | `影片 N`，連結到該支 Reel |

分類與檔案：

| 分類 | 檔案 |
| --- | --- |
| Agent 系統 | `docs/agent-systems.md` |
| 記憶與上下文 | `docs/memory-context.md` |
| 工具與研究 | `docs/tools-research.md` |
| 建構與創作 | `docs/build-create.md` |
| 成本與觀點 | `docs/cost-perspective.md` |
| 動畫與視覺 | `docs/animation-visual.md` |

表格每一列長這樣（欄序固定）：

```markdown
| [名稱](https://example.com) | 說明 | 1,234 | [影片 7](https://www.facebook.com/reel/...) |
```

## 新增一支影片時

1. 在 `README.md` 的「影片來源」表加一列：編號（接續的 `影片 N`）、標題、Reel 網址、收錄日期（`YYYY-MM-DD`）。
2. 把從該片整理出的條目加進對應分類頁，出處用同一個編號。
3. 若有適合面試引用的一句話，加到 `docs/interview-takeaways.md`，點出對應的工具名稱。
4. 條目帶有 GitHub 星數時，在 `README.md` 的星數說明註明查詢日期與時區（台北時間）。
