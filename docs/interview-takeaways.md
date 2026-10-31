# 面試可用的重點

[回首頁](../README.md)

從已收錄的影片整理、面試時可以拿來講的重點。

## AI 團隊方法論

[Orca](https://github.com/stablyai/orca)、[Reason Network](https://github.com/reason-machines/reason-network)：人負責分派、追蹤狀態、決定交接點，agent 之間有明確溝通管道。

## AI 程式碼品質控管

[agentplay](https://github.com/Entelligence-AI/agentplay)：審查不只看 diff，也看 agent 的過程；[git-ai](https://github.com/feder-cr/git-ai)：小批次提交，CI 與測試自動把關。

## 上下文工程

[Graphify](https://github.com/Graphify-Labs/graphify)、[ai-memory](https://github.com/akitaonrails/ai-memory)：給 agent 正確的程式碼結構和規範（如 AGENTS.md），從源頭少寫錯。

## Agent 自我驗收

[video-to-game](https://github.com/lovisdotio/video-to-game)：agent 寫完遊戲後自己用鍵盤玩、錄影、對照原始影片截圖，把「跑起來看結果」變成流程的一部分，而不是只看程式碼。

## 成本治理

[TokenEconomizer](https://github.com/microsoft/TokenEconomizer) 與 [Claude Code vs Blender 梗](https://www.facebook.com/reel/1867596277567322)：agent 不是萬用解，要量化成本與成效。

## 規則優先、AI 其次

[n8n 工單流程](https://www.facebook.com/reel/3209079722631476)：能用明確規則判斷的就不丟給 AI，結果可預測、可測試；寫入用 idempotent（ON CONFLICT）處理重試，這也是控管 AI 產出流程的基本功。
