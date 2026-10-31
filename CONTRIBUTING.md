# 貢獻說明

新的 Facebook Reel 請追加在既有內容後面。不要改寫既有條目的名稱、說明、星數或連結。星數是查詢當下的快照；若要更新，連查詢日期一起改。

## 條目格式

每一筆用同一組欄位，加在對應分類頁的最後面。名稱是標題，摘要緊接在名稱下面。

| 欄位 | 怎麼填 |
| --- | --- |
| 分類 | 下面十三個分類之一，對應一個 Markdown 檔 |
| 名稱 | 工具或主題名稱。有 URL 就做成連結；沒有就不要編一個 |
| 摘要 | 一行白話，放在名稱正下方 |
| 說明 | 這支影片或截圖在講什麼，沿用原意 |
| 可信度 | 選填，跟分類分開。沿用已有標籤，例如 `⚠️ 引流`、`⚠️ 推薦碼引流`、`概念動畫`、`概念介面`、`AI 生成`、`AI 生成圖`、`後製包裝`、`宣稱待驗證`、`商用・無 repo`、`付費模板`。沒有就寫 `—` |
| 星數 | GitHub star，沿用來源的寫法（`110,828`、`124.7k`、`412.7k（REA）`）。沒有 GitHub 專案填 `—` |
| 出處 | `影片 N`（連結到該支 Reel），或 `截圖（來源名）` |
| 配樂 | 選填。聽得出的類型；曲名無法辨識就寫「無法辨識曲名」，不要猜歌名 |
| 留言精華 | 選填。影片留言裡值得留下的一句，並註明那是留言 |

分類與檔案：

| 分類 | 檔案 |
| --- | --- |
| Agent 系統與編排 | `docs/agent-orchestration.md` |
| 記憶與上下文 | `docs/memory-context.md` |
| Skills／MCP／工具 | `docs/skills-mcp-tools.md` |
| 程式開發與品質 | `docs/dev-quality.md` |
| 前端與 UI 設計 | `docs/frontend-ui.md` |
| 3D／動畫與 DCC | `docs/dcc-animation.md` |
| AI 影像與影片 | `docs/ai-media.md` |
| 自動化工作流 | `docs/automation-workflows.md` |
| 金融與交易 | `docs/finance-trading.md` |
| 安全與治理 | `docs/security-governance.md` |
| 實體 AI 與硬體 | `docs/physical-ai.md` |
| 成本與取捨 | `docs/cost-tradeoffs.md` |
| 團隊與組織 | `docs/teams-org.md` |

每一則長這樣。有 GitHub repo 時，摘要下面可以加 Open Graph 預覽，網址是 `https://opengraph.githubassets.com/1/OWNER/REPO`（只取 owner 與 repo，不要把 tree 路徑算進去）。

```markdown
### [名稱](https://github.com/OWNER/REPO)

一行摘要

![名稱 的 GitHub 預覽](https://opengraph.githubassets.com/1/OWNER/REPO)

| 可信度 | 星數 | 出處 |
| --- | --- | --- |
| — | 1,234 | [影片 N](https://www.facebook.com/reel/...) |

說明。
```

`配樂` 和 `留言精華` 沒有就省略，不要為了填而發明內容。有的話寫進說明。影片 11 的 synthwave 純演奏、影片 12 的女聲 EDM／House、影片 13 的駭客風 synthwave、影片 14 的 synth-pop／chill house、OPZEN 的 Sayfalse – DARE、ALGORY 的 ayaibrahimx 原聲，都已經寫在說明裡，曲名除了來源點名的以外都不要猜。RuView 的留言精華也寫在說明裡。

## 新增一支影片時

1. 在 `README.md` 的「影片來源」表加一列：編號（接續的 `影片 N`，或下一個截圖批次）、標題、連結、收錄日期（`YYYY-MM-DD`）。沒有連結就填 `—`，待確認的事寫在表下面。
2. 把條目加進對應分類頁，名稱下面放一行摘要，出處用同一個編號。同時更新 README 分類後面的則數。
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
