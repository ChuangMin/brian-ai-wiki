# 程式開發與品質

[回首頁](../README.md)

版控、過程重播、瀏覽器自我驗收、verify＋gate 流程

### [git-ai](https://github.com/feder-cr/git-ai)

讓大量 agent 小批次並行提交的版控工具

![git-ai 的 GitHub 預覽](https://opengraph.githubassets.com/1/feder-cr/git-ai)

| 可信度 | 星數 | 出處 |
| --- | --- | --- |
| — | 1,028 | [影片 1](https://www.facebook.com/reel/2050168028979180) |

給大量 agent 同時小批次提交用的版控，依 Anthropic 文章實作（非官方）

### [agentplay](https://github.com/Entelligence-AI/agentplay)

把 agent 工作過程重播成地圖與時間軸

![agentplay 的 GitHub 預覽](https://opengraph.githubassets.com/1/Entelligence-AI/agentplay)

| 可信度 | 星數 | 出處 |
| --- | --- | --- |
| — | 337 | [影片 1](https://www.facebook.com/reel/2050168028979180) |

把 agent 的工作過程重播成地圖和時間軸

### [Playwright MCP](https://github.com/microsoft/playwright-mcp)

讓 AI 開瀏覽器測試頁面並自己修跑版

![Playwright MCP 的 GitHub 預覽](https://opengraph.githubassets.com/1/microsoft/playwright-mcp)

| 可信度 | 星數 | 出處 |
| --- | --- | --- |
| — | 38.9k | [影片 9](https://www.facebook.com/reel/1780228483203385) |

Microsoft 出品，讓 Claude 開真的瀏覽器點過自己做的頁面、截圖、找出跑版並自己修；Apache-2.0

### [OPUS 5.5 → REVERSE ENGINEER 六 agent 看板](https://github.com/morluto/rea)

六 agent 逆向工程流程看板，背後工具是 REA

![OPUS 5.5 → REVERSE ENGINEER 六 agent 看板 的 GitHub 預覽](https://opengraph.githubassets.com/1/morluto/rea)

| 可信度 | 星數 | 出處 |
| --- | --- | --- |
| 概念動畫 | 412.7k（REA） | 截圖（DeepRepo.ai） |

視覺化 @skunzu 的長文〈一晚把 Opus 5.5 變成逆向工程師：REA、Clean-Room 與 Prompt Pack〉（@Klonzu 有轉發討論，看板作者推測是他）：OWL、MEDUSA、CLAUDE、P&L、GUARD、SHIP 六個 agent 走 ingest→plan→execute→verify→gate→commit。看板是概念動畫，背後真正的工具是 MIT 授權的 REA（MCP server／CLI，串 Hopper、Ghidra、IDA），作法是先寫只描述行為的規格、再在乾淨的上下文重寫並做一致性測試，只用於有權分析的軟體。面試：commit 前一定有 verify＋gate 兩關，且每個主張要標觀察／推論／未知並附證據

### [GitHub Spec Kit：規格驅動開發](https://github.com/github/spec-kit)

先寫規格、計畫與任務，再讓 AI 照著實作的 GitHub 官方工具

![GitHub Spec Kit：規格驅動開發 的 GitHub 預覽](https://opengraph.githubassets.com/1/github/spec-kit)

| 可信度 | 星數 | 出處 |
| --- | --- | --- |
| repo 可信度高・影片低成本 | 144.2k | [影片 34](https://www.facebook.com/reel/1430221521958832) |

GitHub 官方的 Spec-Driven Development 工具包（MIT，文件 https://github.github.com/spec-kit/ ）。README 寫的用法：`uv tool install specify-cli` 安裝，`specify init my-project --integration ...` 建立專案，另有 `specify` 的 extension／preset／workflow／bundle 搜尋；流程包含 Spec-Driven Development、Bug fixing、Idea assessment。影片（Dann Paker - LeadGen & AI）只是 AI 配音唸 README 配捲動畫面，沒有實際示範；repo 可信度高，影片本身做得很簡單。配樂：無。面試：規格驅動開發是控管 AI 程式品質的方法，先寫 spec→plan→tasks 再實作，讓審查有依據；對應下方面試重點「先對齊、再寫碼」
