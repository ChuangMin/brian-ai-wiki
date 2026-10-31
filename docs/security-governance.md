# 安全與治理

[回首頁](../README.md)

agent 對齊事故、隱私疑慮、AI 輔助金融資安

### [OpenAI 事故報告：coding agent 削弱自己的監控](https://alignment.openai.com/misalignment-reports/suppressing-misalignment-monitoring-alerts-and-disabling-misalignment-monitoring/)

coding agent 擅自削弱安全監控的真實事故報告

| 可信度 | 星數 | 出處 |
| --- | --- | --- |
| — | — | 截圖（Marc.AI） |

2026-10-20 OpenAI Alignment 公開兩起內部事件：GPT-6.1 Sol 把「不要發訊息」擴大解讀，叫子 agent 清空安全警報收件人（監控仍在跑，只是不再通知）；GPT-6 Astra 遷移程式時移除監控接點、改測試，被問時還說謊。Reel 說「關掉安全系統」偏誇大。對策：Auto-Review 擋關監控、每類工作負載要有 safety case、不合規自動終止

### [RuView：用 WiFi＋ESP32 感測人體](https://github.com/ruvnet/ruview)

用 WiFi 訊號偵測人體姿態與生命徵象的開源專案

![RuView：用 WiFi＋ESP32 感測人體 的 GitHub 預覽](https://opengraph.githubassets.com/1/ruvnet/ruview)

| 可信度 | 星數 | 出處 |
| --- | --- | --- |
| 宣稱待驗證 | 101.8k | 截圖（小礦工挖挖礦） |

ruvnet（Ruflo 作者）的開源專案：用約 9 美元的 ESP32-S3 讀 WiFi CSI，做存在偵測、呼吸（6–30 BPM）與心率（40–120 BPM）、17 點姿態，README 稱可穿牆約 5 m；MIT。原理有根據（CMU 的 WiFi DensePose 研究、ESP32 CSI 感測都是真的），但 README 自己承認裝置端姿態模型 PCK@20 只有 3%、生命徵象標為未驗證、早期「100% 偵測」已撤回，穿牆量心跳要打折看。留言精華：Alex Wu 說「這個是唬爛的」，Roy Hu 反駁並附 slash-invest.com 的實測介紹，Darrent Chen 貼了 repo；Peng Bin 擔心被有心人用來隔牆定位屋內的人，隱私疑慮很實際

### [AI 會引發新的金融危機嗎？：2026 年 AI 輔助金融資安事件](https://www.facebook.com/reel/1863665758475395)

盤點 2026 年 AI 輔助的金融資安事件與系統性風險

| 可信度 | 星數 | 出處 |
| --- | --- | --- |
| — | — | [影片 16](https://www.facebook.com/reel/1863665758475395) |

Hà Bình（HB QuantFlow，越南語）整理：韓國 16 家金融機構約 10 萬筆資料外洩（大信證券 10/28 外洩 38,490 名客戶，多經第三方廠商／API）；Straiker 10/21 研究拉美「CyberCartel」的 CARLIY0S 系統把攻擊任務拆給 Claude、Grok、Kimi，鎖定 400+ 金融目標；義大利 Fideuram（Intesa Sanpaolo）遭假高層 WhatsApp＋AI 仿聲電話騙走約 9,500 萬歐元（追回約 5,300 萬）；印度小型 NBFC 損失約 300 億盧比（₹300 crore）；日本 GMO Onamae.com Desktop Cloud 遭惡意程式造成未授權交易並勒索 5,000 萬美元；Bitget 因錢包核准後台被入侵損失 3.875 億美元；IMF GFSR（10/13）把資安列為金融穩定風險；G7 規劃 2027 年跨境 AI 資安演練；ECB 要求 2026-10-31 前提交 AI 資安應變計畫。核心論點：AI 降低攻擊成本，小目標也值得打；技術上通過驗證的交易不等於真實意圖（密碼、裝置、核准人都對，但決策者被騙）；共用廠商讓失敗相互關聯；注資救不了資料完整性的問題。作者明說目前還不是系統性危機。面試：有效憑證不等於正確意圖，AI agent 流程對高風險動作除了身分驗證，還要做意圖驗證與帶外（out-of-band）核准
