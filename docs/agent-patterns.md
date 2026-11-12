# Agent 分工模式

中文 | [English](../en/docs/agent-patterns.md)

[回首頁](../README.md)

從本 wiki **既有條目**歸納的 agent 分工類型（不是新影片、也不是新 SEQ 分類）。每種只列有實際 SEQ 支撐的例子；成效數字若未查證會標「未驗證／宣稱待驗證」。

對應 Canvas 區塊：Page「AI 影片收藏 Wiki」→「Agent 分工模式」。

## 模式一覽

### 1. 建造者＋審查者（Builder + reviewer/judge）

一人（或一模型）負責寫／改，另一個只做是／否或 verify＋gate，不直接寫碼。

- **何時用**：要降低「自稱完成」誤報、需要獨立複核。
- **風險**：審查者若與建造者同上下文，容易一起偏誤。
- **例**：SEQ 0098（見 [Agent 系統與編排](agent-orchestration.md)；Sonnet 寫／Opus 審）、SEQ 0054（見 [程式開發與品質](dev-quality.md)；六 agent 看板的 verify／gate）、SEQ 0015（agentplay：看過程不只看 diff）。

### 2. 模型分層（便宜搜尋／強模型決策）

搜尋、grep、跑測試走便宜／快模型；寫碼與關鍵決策走較強模型。

- **何時用**：同一 session 想控 token。
- **風險**：路由規則寫不清楚時，便宜模型會漏上下文。型號名稱若未核對官方，標宣稱待驗證。
- **例**：SEQ 0098（Haiku 搜尋／測試）、SEQ 0010（TokenEconomizer，見 [成本與取捨](cost-tradeoffs.md)）、SEQ 0061（RTK）。

### 3. 編排者＋平行工作者／Agent Teams

一個 lead 拆任務，多個 worker 各有上下文、可平行或互傳訊息。

- **何時用**：可切開的獨立任務、要提高吞吐。
- **風險**：改同一檔、相依任務多時衝突與 token 暴衝。
- **例**：SEQ 0069（Claude Code Agent Teams）、SEQ 0001（Orca）、SEQ 0003（Reason Network）— 皆見 [Agent 系統與編排](agent-orchestration.md)。

### 4. 管線／依序交接（Pipeline / sequential handoff）

固定階段手遞手（ingest→plan→execute→verify… 或表單→規則→寫入）。

- **何時用**：步驟清楚、要可重跑與可觀測。
- **風險**：前段錯會整條放大。
- **例**：SEQ 0054（逆向工程六 agent 管線）、SEQ 0072（LangGraph PDF 問答）、SEQ 0044／0026（n8n，見 [自動化工作流](automation-workflows.md)）。

### 5. 專責角色（公司化 agent）

用部門／職能命名（PM、dev、財務、稽核等）組「公司」。

- **何時用**：想把預算、核准、彙報寫進流程。
- **風險**：示範資料≠真實負載；有推薦碼／引流的條目可信度要另看。
- **例**：SEQ 0078（Paperclip）、SEQ 0052（chief-night-01）、SEQ 0048（Agentic AI 心智圖）— 見 [Agent 系統與編排](agent-orchestration.md)。

### 6. 記憶／知識代理

專責長期記憶、引用來源、或第二大腦（圖譜／CLAUDE.md／Dreaming）。

- **何時用**：跨 session 要可追溯、要「有來源才寫」。
- **風險**：無來源就瞎編；開源清單若要留言才給連結屬引流。
- **例**：SEQ 0095／0093／0096（見 [記憶與上下文](memory-context.md)）、SEQ 0006（Graphify）、SEQ 0007（ai-memory）、SEQ 0060（CodeGraph）。

### 7. 自我檢查／重複錯誤即停

同一錯誤重複就打斷、或完成前強制複核。

- **何時用**：agent 容易空轉或誤報 done。
- **風險**：閾值太松仍空轉；太嚴又一直停。
- **例**：SEQ 0098（同錯＞2 次即停）、SEQ 0054（verify／gate）、SEQ 0015（過程重播檢查）。

### 8. 人機核准閘門

高風險對外動作先經人核准；或監控被削弱時的反面教材。

- **何時用**：寄信、付款、對外發布。
- **風險**：只做身分驗證不做意圖驗證仍會被騙。
- **例**：SEQ 0044（人核准才寄，見 [自動化工作流](automation-workflows.md)）、SEQ 0052（price_gate／your_call）、SEQ 0039（coding agent 削弱監控，見 [安全與治理](security-governance.md)）。

## 簡表對照

| 模式 | 主要換到什麼 | 主要代價 | 代表 SEQ |
|------|--------------|----------|----------|
| 建造＋審查 | 品質關卡 | 多一輪延遲／token | 0098, 0054, 0015 |
| 模型分層 | 成本控制 | 路由與上下文遺漏 | 0098, 0010, 0061 |
| Teams／編排 | 吞吐 | 衝突、token 暴衝 | 0069, 0001, 0003 |
| 管線交接 | 可重現 | 前段錯放大 | 0054, 0072, 0044, 0026 |
| 公司化角色 | 權責清楚 | 示範≠真實負載 | 0078, 0052, 0048 |
| 記憶代理 | 可追溯 | 無來源瞎編／引流 | 0095, 0093, 0096, 0006, 0007, 0060 |
| 重複即停 | 防空轉 | 閾值難調 | 0098, 0054, 0015 |
| 人機閘門 | 對外安全 | 流程摩擦 | 0044, 0052, 0039 |

可並用，但每加一層都要能說明多付的延遲與 token 換到什麼。

## 來源說明

本頁只從 INDEX／agent-orchestration／cost／memory 等既有分類條目歸納。未在本頁獨立驗證的數字與型號名稱，請回原 SEQ 或官方文件核對。
