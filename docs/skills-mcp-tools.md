# Skills／MCP／工具

[回首頁](../README.md)

通用的 agent 能力元件：MCP、skill、開發方法論 skill、語音、抽取模型

### [earshot](https://github.com/Leonxlnx/earshot)

讓 agent 在本地端處理語音的工具

![earshot 的 GitHub 預覽](https://opengraph.githubassets.com/1/Leonxlnx/earshot)

| 可信度 | 星數 | 出處 |
| --- | --- | --- |
| — | 3,290 | [影片 1](https://www.facebook.com/reel/2050168028979180) |

讓 agent 在本地處理語音

### [axuse](https://github.com/ctoldigital/axuse)

透過無障礙樹操作瀏覽器的 MCP 工具

![axuse 的 GitHub 預覽](https://opengraph.githubassets.com/1/ctoldigital/axuse)

| 可信度 | 星數 | 出處 |
| --- | --- | --- |
| — | 648 | [影片 1](https://www.facebook.com/reel/2050168028979180) |

透過無障礙樹操作瀏覽器，走 MCP

### [imozuru](https://github.com/MaryCache/imozuru)

沿引用追回原始文獻的 Claude Code skill

![imozuru 的 GitHub 預覽](https://opengraph.githubassets.com/1/MaryCache/imozuru)

| 可信度 | 星數 | 出處 |
| --- | --- | --- |
| — | 1,385 | [影片 1](https://www.facebook.com/reel/2050168028979180) |

沿引用往回追到原始文獻的 Claude Code skill

### [audio-studio-mcp](https://github.com/kanaworksai-hue/audio-studio-mcp)

在本地生成音樂與音效的 MCP 工具

![audio-studio-mcp 的 GitHub 預覽](https://opengraph.githubassets.com/1/kanaworksai-hue/audio-studio-mcp)

| 可信度 | 星數 | 出處 |
| --- | --- | --- |
| — | 541 | [影片 1](https://www.facebook.com/reel/2050168028979180) |

在本地生成音樂和音效

### [Cloudflare Clairic 抽取模型](https://blog.cloudflare.com/clairic-extraction-model/)

一次前向就抽出結構化欄位的 Cloudflare 模型

| 可信度 | 星數 | 出處 |
| --- | --- | --- |
| — | — | 截圖（Marc.AI） |

2026-10-19 Workers AI 預覽模型 @cf/cloudflare/clairic：給文字（最多 4 張圖）加欄位 schema，一次前向就回傳有型別的值，不生成 token，附信心分數、null 機率與字元位置。每百萬輸入 token $0.10、輸出不收費，預告開權重。多步數學與預測仍弱

### [Superpowers](https://github.com/obra/superpowers)

讓 coding agent 先釐清需求、寫計畫、TDD 再動手的 skill 方法論

![Superpowers 的 GitHub 預覽](https://opengraph.githubassets.com/1/obra/superpowers)

| 可信度 | 星數 | 出處 |
| --- | --- | --- |
| — | 309.7k | Brian 推薦清單 2026-10-31 |

Jesse Vincent（obra）的 agentic skills 框架：agent 一開工先 brainstorming 問清楚需求、分段給你確認設計，再寫出連新手都能照做的實作計畫，強調紅綠 TDD、YAGNI、DRY，最後用 subagent-driven-development 逐項派工並審查成果；skill 會自動觸發。支援 Claude Code、Codex、Cursor、Gemini CLI、Copilot CLI、Grok Build 等。安裝：Claude Code 用 `/plugin install superpowers@claude-plugins-official`，Cursor 用 `/add-plugin superpowers`；MIT。預設會載入官網 logo 統計版本，可用 `SUPERPOWERS_DISABLE_TELEMETRY` 關閉。面試：把「需求釐清→設計確認→計畫→TDD→子 agent 實作＋審查」固化成團隊流程，就是 AI 團隊方法論的骨架

### [Matt Pocock Skills（Skills For Real Engineers）](https://github.com/mattpocock/skills)

Matt Pocock 每天用的小型工程 skill，主打先對齊再寫碼

![Matt Pocock Skills（Skills For Real Engineers） 的 GitHub 預覽](https://opengraph.githubassets.com/1/mattpocock/skills)

| 可信度 | 星數 | 出處 |
| --- | --- | --- |
| — | 307.9k | Brian 推薦清單 2026-10-31 |

TypeScript 講師 Matt Pocock 從自己 .agents 目錄公開的 skill 集，刻意做得小、可組合、不綁流程（相對 GSD、BMAD、Spec-Kit 那種接管整個流程的做法）。招牌是 /grill-me、/grill-with-docs：開工前讓 agent 反過來拷問你需求，順便建立專案共用詞彙表（ubiquitous language）並把難解釋的決策寫成 ADR，讓 agent 用詞精簡、命名一致。安裝：Claude Code 用 `claude plugin install mattpocock-skills@claude-plugins-official`，其他 agent 用 `npx skills@latest add mattpocock/skills`；MIT。面試：AI 程式碼最常見的失敗是需求沒對齊，用 grilling＋共用詞彙＋ADR 從源頭降低重工

### [Ponytail](https://github.com/DietrichGebert/ponytail)

讓 agent 像資深工程師一樣少寫程式、先重用現有元件的 skill

![Ponytail 的 GitHub 預覽](https://opengraph.githubassets.com/1/DietrichGebert/ponytail)

| 可信度 | 星數 | 出處 |
| --- | --- | --- |
| — | 181.2k | Brian 推薦清單 2026-10-31 |

DietrichGebert 的「懶惰資深工程師」skill：只寫任務需要的程式，優先重用 repo 既有元件，但不准砍驗證、錯誤處理、安全與無障礙。附 /ponytail-review（連 diff 以外受影響的檔案一起審）、/ponytail-audit 等指令。README 自述 Ponytail 5 在 Claude Code 39 個任務的測試：程式碼 -53%、時間 -41%、成本 -26%、token -45%，高風險邏輯 98% 附測試（無 skill 為 68%），屬作者自測。安裝：Claude Code 先 `/plugin marketplace add DietrichGebert/ponytail` 再 `/plugin install ponytail@ponytail`，其他 agent 可直接放 AGENTS.md；MIT。作者提醒只從這個 repo 或 npm `@dietrichgebert/ponytail` 安裝，帶 .exe／.dll 的是假冒版。面試：AI 程式碼品質不只看對不對，還要看是不是多寫了；把「最少必要程式＋不省測試與安全」寫成 review 標準
