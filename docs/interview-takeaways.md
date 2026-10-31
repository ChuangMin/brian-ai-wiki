# 面試可用的重點

[回首頁](../README.md)

從已收錄的影片整理、面試時可以拿來講的重點。

## AI 團隊方法論

[Orca](https://github.com/stablyai/orca)、[Reason Network](https://github.com/reason-machines/reason-network)：人負責分派、追蹤狀態、決定交接點，agent 之間有明確溝通管道。

## AI 程式碼品質控管

[agentplay](https://github.com/Entelligence-AI/agentplay)：審查不只看 diff，也看 agent 的過程；[git-ai](https://github.com/feder-cr/git-ai)：小批次提交，CI 與測試自動把關。

## 上下文工程

[Graphify](https://github.com/Graphify-Labs/graphify)、[ai-memory](https://github.com/akitaonrails/ai-memory)：給 agent 正確的程式碼結構和規範（如 AGENTS.md），從源頭少寫錯。

## RAG 演進路線：用評測決定加什麼

[影片 21](https://www.facebook.com/reel/4570321283241437)：先做 Naive RAG 並建好評測集，量到召回或精準度不足才加 rerank、hybrid、graph；agentic 與多 agent 是最後手段，每加一層都要能說明換來多少品質、付出多少延遲與成本。

## Agent 自我驗收

[video-to-game](https://github.com/lovisdotio/video-to-game)：agent 寫完遊戲後自己用鍵盤玩、錄影、對照原始影片截圖，把「跑起來看結果」變成流程的一部分，而不是只看程式碼。

## 規則優先、AI 其次

[n8n 工單流程](https://www.facebook.com/reel/3209079722631476)：能用明確規則判斷的就不丟給 AI，結果可預測、可測試；寫入用 idempotent（ON CONFLICT）處理重試，這也是控管 AI 產出流程的基本功。

## 成本治理

[TokenEconomizer](https://github.com/microsoft/TokenEconomizer)、[RTK](https://github.com/rtk-ai/rtk) 與 [Claude Code vs Blender 梗](https://www.facebook.com/reel/1867596277567322)：agent 不是萬用解，要量化成本與成效；先過濾上下文雜訊再談換模型。

## 先對齊、再寫碼

[Superpowers](https://github.com/obra/superpowers)、[Matt Pocock Skills](https://github.com/mattpocock/skills)：開工前讓 agent 拷問需求、確認設計與計畫、建立共用詞彙，再用 TDD 與子 agent 審查實作，把方法論寫成團隊共用的 skill。

## 最少必要程式

[Ponytail](https://github.com/DietrichGebert/ponytail)：review 不只問對不對，也問是不是多寫了；重用既有元件、但不省測試、驗證與安全。

## 憑證有效 ≠ 意圖正確

[影片 16](https://www.facebook.com/reel/1863665758475395)：密碼、裝置、核准人都對，決策者仍可能被 AI 仿聲或假訊息騙；agent 流程的高風險動作要做意圖驗證與帶外核准，不能只靠身分驗證。
