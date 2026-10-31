# 自動化工作流

[回首頁](../README.md)

n8n 等流程自動化，規則優先與人工核准閘門

### [n8n 客服工單自動化流程](https://www.facebook.com/reel/3209079722631476)

表單到 SQL 工單的規則式客服自動化流程

| 可信度 | 星數 | 出處 |
| --- | --- | --- |
| 概念動畫 | — | [影片 7](https://www.facebook.com/reel/3209079722631476) |

表單送出→Webhook→驗證資料→用規則（非 AI）判斷 urgent／payment failed 為高優先→寫入 SQL 工單（INSERT … ON CONFLICT 防重試重複）→寄通知信→回 HTTP 200。影片是 AE 風格模擬動畫，不是真的 n8n 畫面（CODER.X）

![霓虹綠終端風工作流 UI：節點依序亮起打勾、右側面板顯示 JSON、底部 log 逐行出現；可用 CSS keyframes + 依序 setTimeout 切換 active class 重現](../assets/gifs/v07-n8n-workflow-ui-motion.gif)

霓虹綠終端風工作流 UI：節點依序亮起打勾、右側面板顯示 JSON、底部 log 逐行出現；可用 CSS keyframes + 依序 setTimeout 切換 active class 重現

### [n8n Email Agent：Gmail→AI Agent→HubSpot／Docs／Sheets](https://n8n.io/workflows/7680-automate-gmail-lead-follow-up-with-openai-gpt-4o-hubspot-slack-and-google-sheets/) ⚠️

Gmail 觸發、AI 查 CRM 後擬信的 n8n 範本

| 可信度 | 星數 | 出處 |
| --- | --- | --- |
| ⚠️ 引流 | — | 截圖（Maruf AI Automation Expert） |

MD Abdullah Al Maruf（孟加拉 n8n／Make 接案者）的「留言 Email Agent 拿模板」導流片：Gmail 觸發→AI Agent 查 HubSpot、Google Docs、Sheets→寄出或存草稿。n8n 官方免費範本就有同款（本連結 #7680）；#8967 則是先依 HubSpot 資料擬回覆、再到 Slack 讓人核准才寄出。面試：AI 只擬草稿、人核准後才寄送，就是對外動作的品質閘門
