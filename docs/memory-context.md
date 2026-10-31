# 記憶與上下文

[回首頁](../README.md)

知識圖譜、程式碼圖譜、長期記憶、跨 agent 交接

### [Graphify](https://github.com/Graphify-Labs/graphify)

把程式碼與文件轉成可查詢的知識圖譜

![Graphify 的 GitHub 預覽](https://opengraph.githubassets.com/1/Graphify-Labs/graphify)

| 可信度 | 星數 | 出處 |
| --- | --- | --- |
| — | 139,236 | [影片 1](https://www.facebook.com/reel/2050168028979180) |

把程式碼、文件、schema 轉成可查詢的知識圖譜

### [ai-memory](https://github.com/akitaonrails/ai-memory)

給 agent CLI 的長期記憶，方便跨 agent 交接

![ai-memory 的 GitHub 預覽](https://opengraph.githubassets.com/1/akitaonrails/ai-memory)

| 可信度 | 星數 | 出處 |
| --- | --- | --- |
| — | 14,563 | [影片 1](https://www.facebook.com/reel/2050168028979180) |

agent CLI 的長期記憶，方便跨 agent 交接

### [Graphicle](https://github.com/Graphicle-AI/graphicle)

單一 Rust 程式同時提供程式碼圖譜與記憶

![Graphicle 的 GitHub 預覽](https://opengraph.githubassets.com/1/Graphicle-AI/graphicle)

| 可信度 | 星數 | 出處 |
| --- | --- | --- |
| — | 477 | [影片 1](https://www.facebook.com/reel/2050168028979180) |

一支 Rust 程式同時提供程式碼圖譜和記憶

### [Hy-Memory](https://github.com/Tencent-Hunyuan/Hy-Memory)

騰訊混元的跨工具 agent 記憶引擎

![Hy-Memory 的 GitHub 預覽](https://opengraph.githubassets.com/1/Tencent-Hunyuan/Hy-Memory)

| 可信度 | 星數 | 出處 |
| --- | --- | --- |
| — | 1,876 | [影片 1](https://www.facebook.com/reel/2050168028979180) |

騰訊混元的 agent 記憶引擎，跨工具共享記憶

### [CodeGraph](https://github.com/colbymchenry/codegraph)

預先索引程式碼成知識圖譜，透過 MCP 給 agent 精準上下文

![CodeGraph 的 GitHub 預覽](https://opengraph.githubassets.com/1/colbymchenry/codegraph)

| 可信度 | 星數 | 出處 |
| --- | --- | --- |
| — | 76.1k | Brian 推薦清單 2026-10-31 |

colbymchenry 的本地端程式碼知識圖譜（Rust 核心）：預先索引函式、類別、呼叫鏈與跨檔關係，程式碼變動時自動同步，透過 MCP server 讓 Claude Code、Cursor、Codex、Gemini、Copilot、Grok Build 等直接查詢，不必每次 grep 整個 repo；100% 本地。安裝：`curl -fsSL https://raw.githubusercontent.com/colbymchenry/codegraph/main/install.sh | sh`（或 `npm i -g @colbymchenry/codegraph`），再 `codegraph install` 接上 agent，每個專案 `codegraph init` 建索引；MIT。同名專案很多（CodeGraphContext 4.4k 星等），這個星數最高。面試：上下文工程的做法之一，先給 agent 正確的結構圖，比讓它亂搜更省 token 也更少改錯地方
