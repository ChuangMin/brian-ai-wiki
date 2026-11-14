# AI 影片收藏 Wiki

中文 | [English](en/index.md)

[每日新聞](news/index.md) — 每天早上的新聞簡報。

[關聯圖](graph/index.html) — 用互動圖看所有條目、分類、來源影片與概念之間的關係（310 個節點、615 條連線）。

Brian 的公開 wiki，以繁體中文（zh-Hant、台灣）從 Facebook 影片、截圖與推薦清單整理 AI 工具與觀點，依主題分類收錄，並另外標示引流、概念動畫等可信度；之後的新影片會繼續加進來。

星數為 2026-10-30 晚上（台北時間）查詢的數字；video-to-game 為 2026-10-31 上午查詢；截圖批次 2 為 2026-10-31 中午查詢；Brian 推薦清單、Filee、CLI-Anything、ai-pdf-chatbot-langchain、影片 32 的 5 個 repo、Paperclip、Spec Kit、archify 與 diagram-design 為 2026-10-31 晚上查詢。Edge0 為 2026-10-31 晚上（台北時間）查詢。PPT Master 為 2026-11-01 凌晨（台北時間）查詢。VibeVoice、Cindy 為 2026-11-01 晚上（台北時間）查詢。mobile-mcp 為 2026-11-01 深夜（台北時間）查詢。影片 16 的事件與數字取自影片文案，未逐一查證。

可信度標籤與分類分開標示：⚠️ 引流（導流、推薦碼、課程漏斗）、概念動畫／概念介面（設計好的畫面，不是真實產品或實測）、AI 生成、後製包裝、宣稱待驗證、商用・無 repo、付費模板、搞笑短劇。GitHub 項目的預覽圖取自 GitHub 的 Open Graph 卡片。

標了引流的條目，連結和說明裡的網址旁邊都會加上 ⚠️。

共 136 則。

從既有條目歸納的分工類型見 [Agent 分工模式](docs/agent-patterns.md)。

## 分類

- [Agent 系統與編排](docs/agent-orchestration.md)（23）— 多 agent 指揮、swarm、中斷續跑、商用 agent OS 與 agent 平台全景
- [記憶與上下文](docs/memory-context.md)（11）— 知識圖譜、程式碼圖譜、長期記憶、跨 agent 交接
- [Skills／MCP／工具](docs/skills-mcp-tools.md)（20）— 通用的 agent 能力元件：MCP、skill、開發方法論 skill、語音、抽取模型
- [程式開發與品質](docs/dev-quality.md)（5）— 版控、過程重播、瀏覽器自我驗收、verify＋gate 流程
- [前端與 UI 設計](docs/frontend-ui.md)（22）— 設計系統、UI linter、設計 skill、介面模板與概念介面
- [3D／動畫與 DCC](docs/dcc-animation.md)（10）— Blender 等 DCC 外掛、運鏡、程序化動畫、遊戲生成
- [AI 影像與影片](docs/ai-media.md)（6）— AI 生成影片與圖片、prompt、AI 渲染、程式化影片
- [自動化工作流](docs/automation-workflows.md)（4）— n8n 等流程自動化，規則優先與人工核准閘門
- [金融與交易](docs/finance-trading.md)（5）— 交易圖表、財務 Claude 技巧，以及交易機器人導流片
- [安全與治理](docs/security-governance.md)（7）— agent 對齊事故、隱私疑慮、AI 輔助金融資安
- [實體 AI 與硬體](docs/physical-ai.md)（3）— ESP32、機器人等實體裝置
- [成本與取捨](docs/cost-tradeoffs.md)（6）— token 成本、指令輸出壓縮、agent 與傳統工具的成本對比
- [團隊與組織](docs/teams-org.md)（1）— 協作成本、決策結構、組織設計
- [演講與 Talk](docs/talks.md)（2）— 演講、訪談、Podcast 片段：AI 領袖與從業者的第一手說法
- [搞笑與迷因](docs/memes.md)（2）— 關於 AI 的職場迷因、搞笑短劇與梗圖
- [生產力與開源工具](docs/productivity-tools.md)（1）— 本身不是 AI 的實用工具：轉檔、桌面效率、開源小工具
- [系統設計與工程基礎](docs/systems-design.md)（8）— 非 AI 的後端／分散式系統基礎與維運常識（如 TLS 健檢）

## 影片來源

| 來源 | 標題 | 連結 | 收錄 |
| --- | --- | --- | --- |
| 影片 1 | 20 F*CKING HOT REPOS（@beamnxw，2026/10/11–10/25） | [reel/2050168028979180](https://www.facebook.com/reel/2050168028979180) | 2026-10-30 |
| 影片 2 | Claude Code vs Blender 成本對比 | [reel/1867596277567322](https://www.facebook.com/reel/1867596277567322) | 2026-10-31 |
| 影片 3 | TradingView K 線回放圖表動畫 | [reel/1632204671708366](https://www.facebook.com/reel/1632204671708366) | 2026-10-31 |
| 影片 4 | Blender 魚群路徑動畫 | [reel/1433262628273189](https://www.facebook.com/reel/1433262628273189) | 2026-10-31 |
| 影片 5 | 自動化垂直港口動畫（@marlenuii） | [reel/1665373244995510](https://www.facebook.com/reel/1665373244995510) | 2026-10-31 |
| 影片 6 | Video to Game：影片變成可玩遊戲（OdinLovis） | [reel/1118797844231418](https://www.facebook.com/reel/1118797844231418) | 2026-10-31 |
| 影片 7 | n8n 一鍵五步驟自動化（CODER.X） | [reel/3209079722631476](https://www.facebook.com/reel/3209079722631476) | 2026-10-31 |
| 影片 8 | Claude Code vs Blender：機械變色龍（@marlenuii） | [reel/1413855857399181](https://www.facebook.com/reel/1413855857399181) | 2026-10-31 |
| 影片 9 | Claude Code 前端必裝 5 個設計外掛（hayderdotdev） | [reel/1780228483203385](https://www.facebook.com/reel/1780228483203385) | 2026-10-31 |
| 影片 10 | VirtuCamera 真手持運鏡做 AI 動畫 | [reel/2599932377114150](https://www.facebook.com/reel/2599932377114150) | 2026-10-31 |
| 影片 11 | Spider Walker：機械蜘蛛／蝎子程序化走路動畫 | [reel/1442232340569116](https://www.facebook.com/reel/1442232340569116) | 2026-10-31 |
| 影片 12 | 財務人員的 25 個 Claude 技巧（Nicolas Boucher） | [reel/1411775787706586](https://www.facebook.com/reel/1411775787706586) | 2026-10-31 |
| 影片 13 | AI 交易機器人 53 美元調槓桿（Tauhid 2.0，反面教材） | [reel/1893910828071251](https://www.facebook.com/reel/1893910828071251) | 2026-10-31 |
| 影片 14 | AI 生成健身女孩短片（少女晴天） | [reel/1449881237350910](https://www.facebook.com/reel/1449881237350910) | 2026-10-31 |
| 影片 15 | Peter Sellis 談組織設計與協作成本（Tenten） | [reel/1728245575311571](https://www.facebook.com/reel/1728245575311571) | 2026-10-31 |
| 截圖批次 | 舊影片截圖：OpenAI 監控事件、Clairic、Apex、ZOEY OS、Vessa／Cadra（無原始連結） | — | 2026-10-31 |
| 截圖批次 2 | n8n Email Agent、OPZEN AI、ORBITAL X-02 火箭、Microduck、Agentic AI 心智圖、ALGORY、RuView、Grok Desk、chief-night-01（Viktor）、Open Design Agent Kit、Opus 5.5 逆向工程看板、日系插畫 prompt；@beamnxw 的 20 HOT REPOS 是影片 1 的轉貼，不重複收錄（無原始連結） | — | 2026-10-31 |
| 影片 16 | AI 會引發新的金融危機嗎？（Hà Bình／HB QuantFlow，越南語） | [reel/1863665758475395](https://www.facebook.com/reel/1863665758475395) | 2026-10-31 |
| 影片 79 | Code with Bhurtel：Space-Time Curve（JavaScript 軟化重力網格動畫，非 AI 工具） | [reel/1140316585123225](https://www.facebook.com/reel/1140316585123225) | 2026-11-13 |
| 影片 80 | 一人公司研究所：10 款專精小模型與三個挑選原則 | [reel/1761537521611500](https://www.facebook.com/reel/1761537521611500) | 2026-11-13 |
| 影片 81 | Altair AI：Fable 5.2 用五個 agent 管社群（概念動畫，非產品錄屏） | [reel/40885633571023865](https://www.facebook.com/reel/40885633571023865) | 2026-11-13 |
| 影片 82 | 產品經理的背後靈 Philo：Pixel Plays（Amir Mushich 的五款零圖片像素網頁遊戲） | [reel/1927405395307821](https://www.facebook.com/reel/1927405395307821) | 2026-11-13 |
| 影片 83 | Ming Cheng Ho（indiehack in）：Fable 5.2 寫程式蓋出渋谷 3D（製程尚未公開） | [reel/2190397408553774](https://www.facebook.com/reel/2190397408553774) | 2026-11-13 |
| 影片 84 | HA Bridge：可視化畫 3D 戶型並綁定 Home Assistant 實體（官方付費中控） | [reel/1885203799120310](https://www.facebook.com/reel/1885203799120310) | 2026-11-13 |
| 影片 85 | What the water keeps：Kevin Ngo 的繪本風泛舟網頁（稱以 Claude Fable 5.2 製作） | [reel/1682717900077017](https://www.facebook.com/reel/1682717900077017) | 2026-11-13 |
| 影片 86 | Altair AI：Claude Second Brain（Obsidian repo 清單＋純 Markdown 變體） | ⚠️ [reel/3002409066786760](https://www.facebook.com/reel/3002409066786760) | 2026-11-13 |
| 影片 87 | Hacking Tutorials Daily：三個免費網路威脅即時地圖（Kaspersky／Check Point／NETSCOUT） | [reel/29346549524942796](https://www.facebook.com/reel/29346549524942796) | 2026-11-13 |
| 影片 88 | Machine Learning & AI：所謂 Google 9 頁 Agent Harness Engineering 文件（並非官方 Google PDF） | [reel/1669067301263733](https://www.facebook.com/reel/1669067301263733) | 2026-11-13 |
| 影片 89 | AI懶人報：Anthropic 官方法務外掛（triage-nda／review-contract／legal-risk-assessment／claude-for-legal） | [reel/2280311616036852](https://www.facebook.com/reel/2280311616036852) | 2026-11-13 |
| 影片 90 | Altair AI：Claude Code 空資料夾建六部門公司（概念動畫；說明文來自 @birmeya） | [reel/1152801101050169](https://www.facebook.com/reel/1152801101050169) | 2026-11-13 |
| 影片 91 | Altair AI：Fable 5.2 四模型一腦任務分流（概念動畫；說明文與畫面不符） | [reel/3438861689623518](https://www.facebook.com/reel/3438861689623518) | 2026-11-14 |
| 影片 92 | DeepResource.ai：JEV agent-router 四路研究寫作分流（概念圖；說明文來自 @Flandermaxx） | [reel/1513020620686286](https://www.facebook.com/reel/1513020620686286) | 2026-11-14 |
| 影片 93 | Know Your System：Saga pattern（跨服務補償交易：編排 vs 事件協同） | [reel/2222208475400708](https://www.facebook.com/reel/2222208475400708) | 2026-11-14 |
| GitHub | labring/sealos-skills：在 Sealos Cloud 部署應用、資料庫與物件儲存的 agent skill 包 | [labring/sealos-skills](https://github.com/labring/sealos-skills) | 2026-11-14 |
| Brian 推薦清單 2026-10-31 | Agent skills 推薦：Superpowers、Matt Pocock Skills、Ponytail、CodeGraph、RTK（無影片） | — | 2026-10-31 |
| 影片 17 | Sam Altman 談新模型與失落感（Cheeky Pint 片段，大叔美股筆記 Uncle Investment Note） | [reel/1167964102224005](https://www.facebook.com/reel/1167964102224005) | 2026-10-31 |
| 影片 18 | Every meeting in 2026（Champagnecruz，The new gold rush） | [reel/1778931116724534](https://www.facebook.com/reel/1778931116724534) | 2026-10-31 |
| 影片 19 | 未來博物館的純人類員工（Christopher Chong，AI 生成短劇） | [reel/1141885222030708](https://www.facebook.com/reel/1141885222030708) | 2026-10-31 |
| 影片 20 | Filee 拖曳轉檔工具（DevPik） | [reel/1143388538027657](https://www.facebook.com/reel/1143388538027657) | 2026-10-31 |
| 影片 21 | RAG Design patterns (You must know in 2026)（Ankur Mishra 轉貼，圖：@MindBoostTutorix） | [reel/4570321283241437](https://www.facebook.com/reel/4570321283241437) | 2026-10-31 |
| 影片 22 | 12 個系統設計基本概念（Code Crack） | [reel/3285768298275601](https://www.facebook.com/reel/3285768298275601) | 2026-10-31 |
| 影片 23 | 10 個指令檢查網站 HTTPS（Code Crack／CodeCrackAI） | [reel/4523349764619784](https://www.facebook.com/reel/4523349764619784) | 2026-10-31 |
| 影片 24 | Claude Code Agent Teams（Lập Trình Web AI，越南語） | [reel/1864411088067060](https://www.facebook.com/reel/1864411088067060) | 2026-10-31 |
| 影片 25 | Kafka 架構手寫風筆記（softwaredeveloper077） | [reel/3443590945824757](https://www.facebook.com/reel/3443590945824757) | 2026-10-31 |
| 影片 26 | CLI-Anything（小礦工挖挖礦） | [reel/1857279712725267](https://www.facebook.com/reel/1857279712725267) | 2026-10-31 |
| 影片 27 | ai-pdf-chatbot-langchain 架構動畫（AI Star Pick） | [reel/1687227069493469](https://www.facebook.com/reel/1687227069493469) | 2026-10-31 |
| 影片 28 | 5 個學駭客的 YouTube 頻道（RedForged） | [reel/1045624941869807](https://www.facebook.com/reel/1045624941869807) | 2026-10-31 |
| 影片 29 | Websites in 2026（wearebrand） | [reel/1834273334429297](https://www.facebook.com/reel/1834273334429297) | 2026-10-31 |
| 影片 30 | BFS 廣度優先搜尋找 Crush（thachdv.it，越南語） | [reel/1108544155324652](https://www.facebook.com/reel/1108544155324652) | 2026-10-31 |
| 影片 31 | Prim's Algorithm（Software with John） | [reel/2132850694107274](https://www.facebook.com/reel/2132850694107274) | 2026-10-31 |
| 影片 32 | 每個工程師都該知道的 5 個 GitHub repo（James Mcquay） | [reel/1849291249414632](https://www.facebook.com/reel/1849291249414632) | 2026-10-31 |
| 影片 33 | Paperclip（小礦工挖挖礦） | [reel/1785583925890920](https://www.facebook.com/reel/1785583925890920) | 2026-10-31 |
| 影片 34 | GitHub Spec Kit（Dann Paker - LeadGen & AI） | [reel/1430221521958832](https://www.facebook.com/reel/1430221521958832) | 2026-10-31 |
| 影片 35 | Kishan 平面設計作品集 | [reel/1670796030659910](https://www.facebook.com/reel/1670796030659910) | 2026-10-31 |
| 影片 36 | 6 種圖表與使用時機（Statsmaniaofficial） | [reel/1742098810210214](https://www.facebook.com/reel/1742098810210214) | 2026-10-31 |
| 影片 37 | Cinema back office dashboard（Code & Chill） | [reel/1473800611304190](https://www.facebook.com/reel/1473800611304190) | 2026-10-31 |
| 影片 38 | Edge0（GitHunt） | [share/r/1CcD2Vgk2Y](https://www.facebook.com/share/r/1CcD2Vgk2Y/)（canonical watch?v=28409829592028769，經 LINE 傳來） | 2026-10-31 |
| 影片 39 | PPT Master（小礦工挖挖礦） | [reel/1051071164608370](https://www.facebook.com/reel/1051071164608370) | 2026-11-01 |
| 影片 40 | VibeVoice（AI懶人報） | [watch?v=2181912112534967](https://www.facebook.com/watch/?v=2181912112534967) | 2026-11-01 |
| 影片 41 | Claude 照片自動分類網頁（亨利溫 Henry Wen） | [reel/DfKEVgNSL3l](https://www.instagram.com/reel/DfKEVgNSL3l/) | 2026-11-01 |
| 影片 42 | Cindy（GitHunt） | [watch?v=2575196886290079](https://www.facebook.com/watch/?v=2575196886290079) | 2026-11-01 |
| 影片 43 | Android 手機 AI agent：ADB 無線偵錯＋Claude Code MCP（Tauhid IQ） | ⚠️ [reel/1628595922149351](https://www.facebook.com/reel/1628595922149351) | 2026-11-01 |
| 影片 44 | FounderOS／Content Lab（Brody） | ⚠️ [reel/1423421943269401](https://www.facebook.com/reel/1423421943269401) | 2026-11-02 |
| 影片 45 | Scrapling（小礦工挖挖礦） | ⚠️ [reel/2088263658998884](https://www.facebook.com/reel/2088263658998884) | 2026-11-09 |
| 影片 46 | gbrain／Garry Tan second brain（Ryven） | [status/2119433356584604119](https://x.com/imryven/status/2119433356584604119) | 2026-11-09 |
| 影片 47 | Altair AI：五個公開 agent skill／設定清單 | [reel/1815732602882824](https://www.facebook.com/reel/1815732602882824) | 2026-11-09 |
| 影片 48 | Altair AI：Claude＋Obsidian Second Brain 十 repo 清單 | ⚠️ [reel/1666945238466731](https://www.facebook.com/reel/1666945238466731) | 2026-11-09 |
| 影片 49 | Lamis Mukta（Anthropic）agent 記憶／Dreaming（David 轉貼） | [status/2118745007628726684](https://x.com/David_eficaz/status/2118745007628726684) | 2026-11-09 |
| 影片 50 | Altair AI：Obsidian CEO 開源的 Claude＋Obsidian 工具清單 | [reel/1895633831459873](https://www.facebook.com/reel/1895633831459873) | 2026-11-09 |
| 影片 51 | Altair AI：純 Markdown＋CLAUDE.md 第二大腦（無 Obsidian／Notion） | [reel/2062559707739569](https://www.facebook.com/reel/2062559707739569) | 2026-11-09 |
| 影片 52 | Altair AI：Claude Code 一場 session 三模型分工（Sonnet／Haiku／Opus） | [reel/2504853660346325](https://www.facebook.com/reel/2504853660346325) | 2026-11-09 |
| 影片 53 | 倉頡 SKILL 2.0（cangjie-skill）：長影片／課程／播客蒸餾成 Agent Skills | [reel/1308612614774010](https://www.facebook.com/reel/1308612614774010) | 2026-11-12 |
| Threads @ethansavemoneydairy | Details.so：真實網站設計細節庫＋MCP（Claude Code／Cursor） | [post/DfgeXIwAIzH](https://www.threads.com/@ethansavemoneydairy/post/DfgeXIwAIzH) | 2026-11-10 |
| 影片 54 | 四個合法資安練習平台（Hack The Box／TryHackMe／PortSwigger Academy／VulnHub） | [reel/1445350007024379](https://www.facebook.com/reel/1445350007024379) | 2026-11-12 |
| 影片 55 | Hallmark：Together AI 的反 AI 味設計 skill（Claude Code／Codex／Cursor／OpenCode） | ⚠️ [reel/1745279943247041](https://www.facebook.com/reel/1745279943247041) | 2026-11-12 |
| 影片 56 | OSIRIS：開源 OSINT 儀表板（osirisai.live；含代幣導流風險） | ⚠️ [reel/847344248401222](https://www.facebook.com/reel/847344248401222) | 2026-11-12 |
| 影片 57 | Higgsfield＋Fable 5.2：宣稱 3.5 小時做出射擊遊戲模型（Blender／UE5） | [reel/1610065000234607](https://www.facebook.com/reel/1610065000234607) | 2026-11-12 |
| 影片 58 | text-to-cad：用文字讓 agent 做 3D／CAD 模型（earthtojake） | [reel/1051298501315719](https://www.facebook.com/reel/1051298501315719) | 2026-11-12 |
| 影片 59 | What the water keeps：Kevin Ngo 的繪本風泛舟網頁（稱以 Claude Fable 5.2 製作） | [reel/1465699568821932](https://www.facebook.com/reel/1465699568821932) | 2026-11-12 |
| 影片 60 | Altair／Flinzu：純文字檔＋CLAUDE.md 地圖 | [status/2119892851387769273](https://x.com/Flinzu/status/2119892851387769273) | 2026-11-12 |
| 影片 61 | Lê Quốc Nghĩa：raw→wiki 與 CLAUDE.md 地圖 | [reel/3503498356478626](https://www.facebook.com/reel/3503498356478626) | 2026-11-12 |
| 影片 62 | Claude Science：蠍毒神經毒素蛋白結合劑（318,484 設計、實驗室測 211 個） | [reel/1119597340441398](https://www.facebook.com/reel/1119597340441398) | 2026-11-12 |
| 影片 63 | Broch Builds：10 個新 Claude Code／Codex skill 清單 | ⚠️ [reel/1439815074924674](https://www.facebook.com/reel/1439815074924674) | 2026-11-12 |
| 影片 64 | 15 個給 AI agent team 的 GitHub repo（含交易相關庫） | [reel/1827893618429238](https://www.facebook.com/reel/1827893618429238) | 2026-11-12 |
| 影片 65 | Fable 5.2 當 CEO：過夜帳單稽核（多模型分工） | [reel/1071773105932698](https://www.facebook.com/reel/1071773105932698) | 2026-11-12 |
| 影片 66 | Higgsfield X Fable 剪輯廣告（付費合作） | ⚠️ [reel/1461806646088320](https://www.facebook.com/reel/1461806646088320) | 2026-11-12 |
| 影片 67 | Claude＋ChatGPT Astra 6：互動建築簡報（Verdant Residences） | ⚠️ [reel/1485883914602760](https://www.facebook.com/reel/1485883914602760) | 2026-11-12 |
| 影片 68 | 每間公司該建的 10 種 AI Employees（角色清單，無實作） | ⚠️ [reel/2226812394848085](https://www.facebook.com/reel/2226812394848085) | 2026-11-12 |
| 影片 69 | 9 個打敗 AI slop 的 UI 細節（David Mráz／Atheros Learning） | ⚠️ [reel/1690133082855724](https://www.facebook.com/reel/1690133082855724) | 2026-11-12 |
| 影片 70 | 光與線：視覺構成短片（非 AI 工具介紹） | [reel/1782325196375171](https://www.facebook.com/reel/1782325196375171) | 2026-11-12 |
| 影片 71 | 騰訊混元 Hy4：首次加入視覺與 computer use（說明文有把 preview 規格算進正式版） | [reel/2350688215687462](https://www.facebook.com/reel/2350688215687462) | 2026-11-12 |
| 影片 72 | SkillTree：宣稱 47 個 agent 跑一家公司（共享 Company Brain＋Council） | ⚠️ [reel/1329619602540541](https://www.facebook.com/reel/1329619602540541) | 2026-11-12 |
| 影片 73 | Gilt Foundry：互動漫畫網站（只展示完成品，留言 HOW） | ⚠️ [reel/1436171255368046](https://www.facebook.com/reel/1436171255368046) | 2026-11-12 |
| 影片 74 | Claude Code（Fable 5.2）＋Herdr：四個本機 Pi agent 並行分窗 | [reel/1609258920348255](https://www.facebook.com/reel/1609258920348255) | 2026-11-12 |
| 影片 75 | JEV Engineering：多 agent 管線監控的科幻 FUI 儀表板（概念動畫，非產品錄屏） | [reel/1773060590589981](https://www.facebook.com/reel/1773060590589981) | 2026-11-12 |
| 影片 76 | Altair AI：Fable 5.2 讀完筆電，告訴我為什麼專案都開了不完（概念動畫） | [reel/1980204536698183](https://www.facebook.com/reel/1980204536698183) | 2026-11-12 |
| 影片 77 | Altair AI：隔夜一指令整理筆記進第二大腦 | [reel/1473932208004781](https://www.facebook.com/reel/1473932208004781) | 2026-11-12 |
| 影片 78 | Altair AI：Karpathy 的六個免費 GitHub 專案（含 LLM Wiki gist） | [reel/1655634979372088](https://www.facebook.com/reel/1655634979372088) | 2026-11-12 |
| Brian 推薦清單 2026-10-31 | 圖表 skill 推薦：archify、diagram-design（無影片） | — | 2026-10-31 |
沒有連結的來源，附上來源裡的待確認事項：
- **截圖批次**：mex 訓練曲線那支待確認 repo
- **截圖批次 2**：待確認：Tommy Vaga 是否即 VagaFX 的 Tomas Edgar、Opus 5.5 看板作者是否為 @Klonzu、Microduck 與 Open Duck Mini 的關係、Grok Desk 推文內文（X 擋抓取）、OPZEN 功能細節取自搜尋摘要；REA 星數 41 萬偏高但照 API 回傳；火箭、心智圖、插畫 prompt 三支沒有原始連結
- **Brian 推薦清單 2026-10-31**：依名稱對應到 GitHub 星數最高的 repo：obra/superpowers、mattpocock/skills、DietrichGebert/ponytail、colbymchenry/codegraph、rtk-ai/rtk；ponytail、codegraph 有多個同名或衍生專案，Ponytail 的效能數字是作者自測
- **Brian 推薦清單 2026-10-31**：tt-a1i/archify、cathrynlavery/diagram-design；中文 fork patrick-xin/diagram-design-zh
來源另外記下的一句：
- **影片 21**：另一支 reel 1110027721743729 下載失敗，未收錄
## 圖表演示

可瀏覽的 HTML 示範：[Demos 索引](demos/index.html)。線上版：<https://wiki.singularityengine.dev/demos/>

影片 3 的 K 線回放有一份自包含的 canvas 重現（示範資料）：[K 線回放圖表演示](demos/chart-replay/index.html)。用法見 [demos/chart-replay/README.md](demos/chart-replay/README.md)。

線上版：<https://wiki.singularityengine.dev/demos/chart-replay/>

## 怎麼追加

新影片請依 [CONTRIBUTING.md](CONTRIBUTING.md) 的條目格式往下加。新聞簡報每天一篇，步驟見 CONTRIBUTING.md 的「新增一天的新聞簡報」。
