# Agent 系統與編排

[回首頁](../README.md)

多 agent 指揮、swarm、中斷續跑、商用 agent OS 與 agent 平台全景

### [Orca](https://github.com/stablyai/orca)

在同一個工作台集中指揮多個 coding agent

![Orca 的 GitHub 預覽](https://opengraph.githubassets.com/1/stablyai/orca)

| 可信度 | 星數 | 出處 |
| --- | --- | --- |
| — | 110,828 | [影片 1](https://www.facebook.com/reel/2050168028979180) |

集中指揮多個 coding agent（Claude Code、Codex 等）的工作台

### [Ruflo](https://github.com/ruvnet/ruflo)

部署與協調多 agent swarm 的編排框架

![Ruflo 的 GitHub 預覽](https://opengraph.githubassets.com/1/ruvnet/ruflo)

| 可信度 | 星數 | 出處 |
| --- | --- | --- |
| — | 80,250 | [影片 1](https://www.facebook.com/reel/2050168028979180) |

部署多 agent swarm、協調自動化流程的框架

### [Reason Network](https://github.com/reason-machines/reason-network)

用加密 P2P 讓團隊看見彼此 agent 的進度

![Reason Network 的 GitHub 預覽](https://opengraph.githubassets.com/1/reason-machines/reason-network)

| 可信度 | 星數 | 出處 |
| --- | --- | --- |
| — | 1,336 | [影片 1](https://www.facebook.com/reel/2050168028979180) |

用加密 P2P 串起團隊的 agent，看得到各自在哪個 repo、分支做什麼

### [durable-harness](https://github.com/vercel-labs/durable-harness)

讓 agent 中斷後能從原處接著跑

![durable-harness 的 GitHub 預覽](https://opengraph.githubassets.com/1/vercel-labs/durable-harness)

| 可信度 | 星數 | 出處 |
| --- | --- | --- |
| — | 274 | [影片 1](https://www.facebook.com/reel/2050168028979180) |

讓 agent 中斷後能從原處接著跑（Vercel）

### [ZOEY OS](https://zoeyos.com/)

由總指揮 agent 分派 worker 的商用 agent 系統

| 可信度 | 星數 | 出處 |
| --- | --- | --- |
| 商用・無 repo | — | 截圖（ZOEY OS） |

商用多 agent 作業系統：跟總指揮 Zoey 一直對話，她自己建立專職 worker 分工；宣稱 5 層記憶、知識庫、1,000+ 整合、能操作你已登入的瀏覽器；沒有公開 repo

### Agentic AI 實作速查心智圖

一張圖看完 Agentic AI 平台的各個元件

| 可信度 | 星數 | 出處 |
| --- | --- | --- |
| AI 生成圖 | — | 截圖（Joyatres Technology） |

Joyatres Technology 整理的 agent 平台全景：記憶（長期／情節／語意／程序）、Human-in-the-loop（核准閘門、中斷與恢復）、工具與協定（MCP、A2A、function calling、電腦／瀏覽器操作）、Agentic RAG（查詢路由、Corrective RAG）、建構堆疊、LLMOps 與安全（LangSmith、DeepEval、NeMo Guardrails、最小權限）、廠商 SDK（Google ADK、MS Agent Framework、AWS Strands）。圖本身明顯是 AI 生成（Longle-Source、Correvlic、Kubenates、Roundation Modies 等亂碼），當檢查清單用就好，細節別照抄。面試：可拿 Evaluation、Guardrails、Observability、Approval Gates 四塊當 agent 平台品質控管的骨架

### [chief-night-01：Viktor 一夜開發 25 家牙醫診所](https://viktor.com/)

AI 員工一夜找出 25 家潛在客戶，寄信前等人核准

| 可信度 | 星數 | 出處 |
| --- | --- | --- |
| ⚠️ 推薦碼引流 | — | 截圖（DeepRepo.ai） |

出自 @Argona0x 的推文（ARGONA 浮水印）：在 Viktor（ZETA AI 的 Slack／Teams AI 員工，跑 Opus 5.5）下目標「每月找 5 萬美元新生意、只用公開資料、沒我同意不聯絡任何人」，一夜拆成 4 個排程工作，從 Google Maps 撈 Austin 240 家牙醫、去掉連鎖剩 25 家，每家附觀察與出處，寫好開場信但 0 封寄出，報價單價格留白由人填。屬推薦碼（ARGONA100）導流，但流程設計值得學。面試：證據連結的主張、claim.check 標記 invented 0、price_gate 缺值就 STOP＋ASK、your_call 由人核准才寄送
