# 貢獻說明

新的 Facebook Reel 請追加在既有內容後面。不要改寫既有條目的名稱、說明、星數或連結。星數是查詢當下的快照；若要更新，連查詢日期一起改。

## 條目格式

每一筆用同一組欄位。分類決定放在哪一頁，其餘四欄寫進該頁的表格，新列加在表格最下方：

| 欄位 | 怎麼填 |
| --- | --- |
| 分類 | 下面七個分類之一，對應一個 Markdown 檔 |
| 名稱 | 工具或主題名稱，連結到該筆的 URL |
| 說明 | 這支影片在講什麼，沿用原意，不另加評價 |
| 星數 | GitHub star，千分位逗號（例如 `110,828`）。沒有 GitHub 專案填 `—`。也可用來源裡的縮寫，例如 `124.7k` |
| 出處 | `影片 N`，連結到該支 Reel |
| 配樂 | 選填。聽得出的類型；曲名無法辨識就寫「無法辨識曲名」，不要猜歌名 |
| 留言精華 | 選填。影片留言裡值得留下的一句，並註明那是留言 |

分類與檔案：

| 分類 | 檔案 |
| --- | --- |
| Agent 系統 | `docs/agent-systems.md` |
| 記憶與上下文 | `docs/memory-context.md` |
| 工具與研究 | `docs/tools-research.md` |
| 建構與創作 | `docs/build-create.md` |
| 成本與觀點 | `docs/cost-perspective.md` |
| 動畫與視覺 | `docs/animation-visual.md` |
| Skills 與外掛 | `docs/skills-plugins.md` |

表格每一列長這樣（欄序固定）：

```markdown
| [名稱](https://example.com) | 說明 | 1,234 | [影片 7](https://www.facebook.com/reel/...) |
```

`配樂` 和 `留言精華` 沒有就整欄省略，不要為了填而發明內容。有的話寫進該筆說明，或在表格下方用「配樂：…」「留言精華：…」另列。影片 11 的 synthwave 純演奏、影片 12 的女聲 EDM／House 都寫在說明裡，曲名無法辨識。

## 新增一支影片時

1. 在 `README.md` 的「影片來源」表加一列：編號（接續的 `影片 N`）、標題、Reel 網址、收錄日期（`YYYY-MM-DD`）。
2. 把從該片整理出的條目加進對應分類頁，出處用同一個編號。
3. 若有適合面試引用的一句話，加到 `docs/interview-takeaways.md`，點出對應的工具名稱。
4. 條目帶有 GitHub 星數時，在 `README.md` 的星數說明註明查詢日期與時區（台北時間）。

## 新增一個 HTML 示範

每個示範一個資料夾，不要把多個示範塞在同一個 `index.html`：

- `demos/<slug>/index.html`：可單獨打開的頁面。
- `demos/<slug>/README.md`：這個示範怎麼操作、怎麼改。

然後在 `demos/demos.json` 陣列最後加一筆。索引頁用 `fetch` 讀這份檔，不用改 `demos/index.html`。分類按鈕只出現有示範的分類。

| 欄位 | 怎麼填 |
| --- | --- |
| `id` | 與資料夾名稱相同，例如 `chart-replay` |
| `title` | 繁體中文標題 |
| `desc` | 一行說明 |
| `category` | 分類標籤。目前的示範是「金融圖表」。之後可沿用，或在真的有該類示範時再用「資料視覺化」「動畫」「3D」這類名稱 |
| `path` | 相對於 `demos/` 的路徑，資料夾請以 `/` 結尾，例如 `chart-replay/` |
| `source` | `影片 N`，對應 README 的影片來源 |
| `sourceUrl` | 該支 Reel 的網址 |
| `added` | 加入日期，`YYYY-MM-DD` |

`demos.json` 裡的順序就是同一分類裡卡片的順序。不要改既有項目的 `id` 或 `path`。索引要能讀到 JSON，請用本機伺服器或 GitHub Pages 開 `demos/index.html`，不要直接用檔案網址開。
