# 演講與 Talk

中文 | [English](../en/docs/talks.md)

[回首頁](../README.md)

演講、訪談、Podcast 片段：AI 領袖與從業者的第一手說法

### [Sam Altman：新模型連破研究難題後的失落感（Cheeky Pint）](https://www.facebook.com/reel/1167964102224005)

Sam Altman 談新模型連破研究難題，興奮之外也感到失落

| 可信度 | 星數 | 出處 |
| --- | --- | --- |
| — | — | [影片 17](https://www.facebook.com/reel/1167964102224005) |

大叔美股筆記 Uncle Investment Note 剪輯的 Podcast《Cheeky Pint》片段（浮水印 Source: Cheeky Pint，酒吧場景、兩人邊喝啤酒邊聊）。Altman 說某個週末拿到新模型，內部頻道取名「模型名 - hold my beer」，大家把學術生涯裡最難的研究問題丟給它，結果在許多領域一題接一題被解掉；他興奮到兩個晚上幾乎沒睡，但也比預期多了很多失落，像是「某件事正在結束」的感覺。他認為這對世界是對的，是沒人能也不該阻止的現實走向；主持人稱之為 wistfulness／懷舊，Altman 回「不只是懷舊」。片中沒有說是哪個模型；字幕前半段翻譯正確。真實訪談剪輯，非 AI 生成。配樂：無，只有對話。

#### 分段重點與時間軸

本則是 Facebook 上的短剪輯，不是整集節目。官方節目是 Cheeky Pint 第 39 集〈Why Sam Altman is against a single superintelligence〉（2026-10-29，主持 John Collison）：[節目頁](https://cheekypint.transistor.fm/39)。官方逐字稿在[原節目逐字稿頁](https://cheekypint.transistor.fm/39/transcript)，完整全文只收入私人檔案庫，不轉貼在公開站。

- 剪輯內容對應節目裡 Altman 談到某個週末拿到新模型的那段（官方章節表的 Math 段自 **15:47** 起，這段話出現在其後）。內部頻道取名「Model Name-Hold My Beer」，把學術生涯裡最難的研究問題丟給它，結果在許多領域一題接一題被解掉。
- 他說興奮到兩個晚上幾乎沒睡，但也比預期多了很多失落，像是「某件事正在結束」。主持人稱之為 wistfulness／懷舊，他回「不只是懷舊」。
- 片中沒有說是哪個模型。官方整集還有 PHP week、sandboxing、agent swarms 等其他章節，不在本則剪輯裡，請看官方節目頁，這裡不展開。

### [Claude Science：蠍毒神經毒素蛋白結合劑（318,484 設計、實驗室測 211 個）](https://www.anthropic.com/research/claude-scorpion-toxin-binder-design)

Anthropic 公開 Claude 設計蠍毒結合劑的實驗：211 個送測、17 個過關（約 8%），官方寫明尚未驗證能否中和毒性

| 可信度 | 星數 | 出處 |
| --- | --- | --- |
| 可信度高 | — | [影片 62](https://www.facebook.com/reel/1119597340441398) |

小礦工挖挖礦上傳的約 1:22 Facebook Reel（2026-10-23）。對照[官方文章](https://www.anthropic.com/research/claude-scorpion-toxin-binder-design)與[技術報告 PDF](https://www-cdn.anthropic.com/31ac578806cffd8b3d92d8affe6edc4c04d502e1.pdf)（2026-10-20）：Claude 依初始提示詞與 4 次追問，針對 5 種鈉通道毒素產生 318,484 個設計，自選 180 個、團隊再加 31 個，共 211 個由 Adaptyv Bio 與 Twist Bioscience 實驗室檢測，17 個達結合標準（約 8%）；Cn2 有 7 個、Ts1 為 0。報告寫最緊的 Cn2-B1 為個位數 nM 或更好；旁白並提 B2，本則未逐圖核對 B2 親和力，標未驗證。自主設計約前 24 小時，到最終名單共 64 小時。提示詞與 Citrini Research 合作。官方明確寫尚未在功能試驗或體內測試能否中和毒性，只用重組毒素測結合，不是解藥宣稱。資料公開於 [Hugging Face](https://huggingface.co/datasets/Anthropic/scorpion-toxin-binder-design)。旁白只提 SPR；報告寫兩家的主篩是 SPR，部分 Adaptyv 重複測量改用 biolayer interferometry（BLI），兩家都做了 reverse BLI（Twist 測 Cn2、Ts1、AaH II、AaH I）。片尾只問「接下來最難的是設計還是實驗」，無留言換連結。配樂：未標。GIF：0:23–0:33。

![小礦工解說實驗數據的簡報畫面](../assets/gifs/v60-claude-scorpion-binders.gif)

### 0144　Lauren Tan（poteto）：All Code Is Slop (Except Mine)（AI Engineer CODE 2026）

當 agent 重複犯錯，把修正寫進程式碼庫、API 與可執行檢查，而不是再加 AGENTS.md。倒金字塔由上而下是 codebase、靜態分析、驗證、散文、人工審查；數字為講者／團隊自述、未查核。來源：影片 100。

Lauren Tan（poteto）在 AI Engineer CODE 2026 的約 17 分 31 秒演講（1920×1080；info.json 的 timestamp 為 1794681009，即 2026-11-14 18:30:09 UTC、2026-11-15 02:30:09 Asia/Taipei；upload_date 欄為 20261114，是 UTC 日期）。YouTube 由 AI Engineer 頻道上傳，標題為 All Code Is Slop (Except Mine) — Lauren Tan, SpaceXSI。Brian 於 2026-11-16 07:49 Asia/Taipei 經 LINE 傳來 https://youtu.be/O_zcc6Xl12g?si=8TX1iOUw2cJrOI51 （canonical https://www.youtube.com/watch?v=O_zcc6Xl12g）。官方頁 https://ai.engineer/code/2026/talks/lauren-tan 。沒有要留言關鍵字換東西，故不標引流。講者是 SpaceXSI 工程師、Grok Bot 團隊成員，也是 React compiler 核心成員（公開身分 @poteto）；開場自介為 poteto，在 SpaceXSI 做 Grok Bot。核心主張是：在大幅提高產出的同時維持甚至提高品質；信任來自投資 agent 的環境，不是盲目相信。當 agent 重複犯同一個錯，要把修正寫進程式碼庫、API 設計或可執行的檢查（lint、測試、驗證），而不是再加一段 AGENTS.md 或註解。她用一座倒金字塔（the poteto pyramid）說明時間該花在哪裡，左邊有朝下的 cost 箭頭，由上（寬、較便宜）到下（窄、較貴）依序是：codebase（好的 API 設計、架構、重構）、static analysis（lint、型別、編譯器、測試、CI）、verification（形式化、執行期）、prose（規則、skills、AGENTS.md）、human review。例子包括：內部框架 Dune（未公開；講者形容為給 Electron 應用用的 Next.js 類框架，內建大量可執行約束）；把註解改成會指出根本原因的 lint 規則，並限制絕大多數註解，因為註解會過期且無法強制執行；執行期用 feature map 加上可重用 CLI；形式化用 TLA+ 檢查跨裝置通知等主要流程、用 Lean 證明部分演算法（講者說仍在實驗，不是萬靈丹）；UI 屬性測試用開源庫 Bombadil（https://github.com/antithesishq/bombadil ，準備紀錄 2026-11-16 為 1,970 星、MIT）。她引用 Cindy Sridharan 的說法（演講中的引言，本則未另行查核）：約六個月前 Cindy 寫到，因細微錯誤被合併而難以信任 agent，缺的是驗證；六個月後 Cindy 說每天約 70% 的 token 花在驗證上。講者說這與她自己的觀察相符，並認為 agent 降低了測試與驗證的成本。這是講者對引言的轉述，不是本則獨立查證。數字皆為講者／團隊自述，本則未查核，也不要把不同口徑混在一起：她個人上一個月稱送出 3,000 個 PR；團隊投影片寫 Grok Bot 團隊 10 月合併 10,926 個 PR（口頭說約 11,000），6 月至 10 月合計 23,370；另提到 10 月約 227 人至少貢獻一個 PR，穩定版大約一天切一次。撤銷率投影片標的是被還原的 commit 百分比（10 月 0.47%；6 月至 10 月依序為 0.98%、0.61%、0.47%、0.48%、0.47%），口頭則說大約 0.5% 的 PR。講者也說 Grok Bot（仍是 Electron 應用）在啟動、打字、開新對話與切換對話等面向比推出時更快，這同樣是講者說法。片尾她把 Grok Bot 當作外圈（outer loop）的例子：有連接器與例行工作可啟動 Cursor、cloud agents 與 projects，用以編排數百甚至數千個 agent；並稱每次發佈會自動開一個 Cursor project 去做應用層的檢查、再開修復 PR 且自動合併。這是講者對自家流程的說法，本則不當操作教學，GIF 也略過相關討論串畫面。pstack 是她放在 cursor/plugins 底下的 plugin（https://github.com/cursor/plugins/tree/main/pstack ），MIT，Copyright (c) 2026 Lauren Tan，版本 v0.15.42。父倉庫 cursor/plugins 於準備當日為 16,437 星，這個數字屬於整個 plugins 倉庫，不要算成 pstack 自己的星數。SkillSpector 靜態掃描（2026-11-16 07:55 台北時間，報告時間戳 2026-11-15 23:55:20 UTC，skillspector 2.12.0，--no-llm，掃描路徑為 pstack，commit bf0c7cd）：score 100、severity CRITICAL、recommendation DO_NOT_INSTALL；issues 198（HIGH 20：TM1 5、MP3 4、P6 4、RA1 3、TM2 2、SC2 1、YR4 1；MEDIUM 176，其中 AS3 skill-enumeration 169 則；LOW 2）。多數是模式噪音。這是規則與模式掃描，不是已確認的漏洞或利用證明。安裝前應自行評估。互動重現：https://wiki.singularityengine.dev/demos/poteto-trust-pyramid/ （五層可點的倒金字塔與向下的 cost 箭頭，內容取自演講例子；這不是產品，也不會連網）。配樂：現場演講與掌聲，曲名未標。GIF：0:28–0:32 標題、0:02:06–0:02:11 金字塔、0:13:34–0:13:39 團隊 PR 圖（已裁到投影片區，不含講者姓名條；https://wiki.singularityengine.dev/assets/gifs/v94-poteto-trust-pyramid.gif）。

互動 Demo：[poteto-trust-pyramid](https://wiki.singularityengine.dev/demos/poteto-trust-pyramid/)

![標題投影片 all code is slop、the poteto pyramid 與 Grok Bot 團隊 10 月 PR 圖；已裁到投影片區，不含講者姓名條](../assets/gifs/v94-poteto-trust-pyramid.gif)

#### 分段重點與時間軸

對照原片：[YouTube](https://www.youtube.com/watch?v=O_zcc6Xl12g)。時間碼依原片。下列為重點整理，不是逐字稿；完整逐字稿只放在私人檔案庫。數字為講者／團隊自述，未查核。

- **00:14** 自介為 poteto，在 SpaceXSI 做 Grok Bot。主張可以把別人看來像 slop 的程式碼，變成可依賴的產出。
- **00:42** 講者自述上月送出 3,000 個 PR 到 production（未查核）。核心是：在大幅提高產出的同時維持甚至提高品質。信任來自投資 agent 的環境，不是盲目相信。
- **02:03** 倒金字塔（the poteto pyramid）：先做 codebase 與靜態分析（較便宜、可決定論），再加驗證，最後才是 prose（規則、skills、AGENTS.md）。
- **02:55** 修正 agent 時，優先把檢查寫進程式碼，而不是再加一行 AGENTS.md。把程式碼庫比成花園：環境不好，agent 會複製壞的模式。
- **05:00** 例子：內部框架 Dune（講者形容為給 Electron 應用用的 Next.js 類框架，內建約束）。例如在產品程式裡限制易被誤用的 API；用目錄慣例切開 Electron 的 main／renderer，並禁止跨層 import。
- **08:12** 把絕大多數註解限制掉，因為會過期、也無法強制執行；改用會指向根本原因的 lint。
- **09:40** 驗證：執行期（含 feature map、可重用 CLI）、TLA+ 查主要流程、Lean 證明部分演算法（講者說仍在實驗）、UI 屬性測試用 Bombadil。
- **11:52** 轉述 Cindy Sridharan：約六個月前因細微錯誤被合併而難信任 agent，缺的是驗證；後來她說每天約 70% 的 token 花在驗證上。這是講者轉述，未另行查核。
- **13:05** pstack（PotatoStack）裡的 StateChart skill，用來從使用者觀點看狀態機。授權與掃描見本則既有說明。
- **13:36** 團隊數字（講者／投影片自述、未查核）：口頭約 11,000 個 PR（投影片寫 10,926）；約一天切一次穩定版；10 月約 227 人至少貢獻一個 PR；撤銷率口頭約 0.5%。並稱 Grok Bot 在啟動、打字、開新對話與切換對話等比推出時更快。
- **15:56** 外圈例子：Grok Bot 的連接器與例行工作可啟動 Cursor、cloud agents 與 projects；並稱發佈後會自動開 project 做應用層檢查、再開修復 PR 且自動合併。這是講者對自家流程的說法，不是操作教學。

### 0149　Matt Pocock 直播對談 Lauren Tan（poteto）：信任階梯、Michelin 廚房與內外圈 agent（Facebook 轉發）

Matt Pocock 與 Lauren Tan 約 65 分鐘的直播對談：信任階梯、Michelin 廚房隱喻，以及用外圈例行工作接上內圈協調 agent。數字為講者／主持人自述、未查核；對照 SEQ 0144。來源：影片 105。

| 可信度 | 星數 | 出處 |
| --- | --- | --- |
| 講者自述數字未查核 | — | [影片 105](https://www.facebook.com/reel/4411053492371686) |

Matt Pocock 在自己的 YouTube 頻道做的直播對談（官方標題 LIVE: Poteto (creator of pstack) on shipping 1,000's of PR's a month at SpaceX；canonical [https://www.youtube.com/watch?v=MN9dGgmLyso](https://www.youtube.com/watch?v=MN9dGgmLyso)；頻道 [Matt Pocock](https://www.youtube.com/@mattpocockuk)）。官方 info.json 的 timestamp 為 1791004092，即 2026-10-03 05:08:12 UTC、2026-10-03 13:08:12 Asia/Taipei，片長約 1 小時 5 分 36 秒（3936 秒）、1920×1080。Brian 於 2026-11-16 經聊天傳來的是 Facebook 轉發 [https://www.facebook.com/reel/4411053492371686](https://www.facebook.com/reel/4411053492371686)，上傳者為 Việt Nguyễn AI（2026-11-12 16:00:01 Asia/Taipei；約 1 小時 5 分 01 秒、1920×1080）。轉發比官方片少約 35 秒，開頭直接從講者說「Thanks for having me」接上，對得上官方約 0:36 的開場，結尾同樣收到「Let's do it. Part two.」。沒有要留言關鍵字換東西，故不標引流。這是 2026-10-03 的直播問答，不是 SEQ 0144 那一場較晚的 AI Engineer CODE 2026 演講；主題有重疊（信任、環境、pstack、Grok Bot、外圈），但主持人、時長、場次與數字口徑都不同，故另立本則，並對照 SEQ 0144。Facebook 轉發文案寫同時跑 30 多個 agent、每月 1,000 個 PR、醒來已有 20 個 PR 等，與本則畫面與對談不符，本則不以該文案為準。畫面 Logo 與 SEQ 0144 都寫 SpaceXSI；講者口頭說「Cursor which is now SpaceX AI」，本則不把後者當成正式名稱。講者自述此前在 Meta 的 React 團隊，3 月加入 Cursor；另以在 Netflix 帶團隊的經驗，提到「context not control」（給脈絡、而不是用控管去微觀管理）。主持人開場說，她約 10 天前有一場演講，並在 X 發過「上月送到 production 的 2,500 個 PR」相關內容，主持人稱該則約 300 萬次觀看；這些是主持人轉述，本則未查核，也不把它自動對成其他場次。本則對談裡，講者把數字說成 2,000 或 2,500 個 PR，並在後段澄清：這顯然不是 2,500 個功能，很多其實是 gardening（整理環境、讓團隊與 agent 都好做事）。這些數字是講者／主持人當日自述，未查核，也不要和 SEQ 0144 較晚演講裡的 3,000 個個人 PR、團隊 10,926 等口徑混在一起。核心脈絡是信任階梯：她說這段路在加入 Cursor 之前就開始了，當時（約 1、2 月）常把時間花在微觀管理單一 agent；要先把「廚房」與工具準備好，才能往上加更多 agent。她不太喜歡 software factory 這個詞容易讓人聯想到沒有品質與技藝，較想用 Michelin 廚房作比喻：從一個人做完全部備料的家庭煮手，到分工給幾位助手，再到主廚負責組織廚房、仍對成品負責。講到產出規模時，她區分內圈與外圈：內圈是朝一份意圖快照寫程式的 agent（她舉 Cursor 當時較新的 projects：雲端上的協調／幕僚型 agent，自己少動手、負責委派與監督）；外圈則是從 Slack、X、email、Linear 等外部系統把脈絡拉回來的連接器與例行工作。對照 SEQ 0144 與產品名稱，本則把她說的外圈工具寫成 Grok Bot（第三方字幕有 Graphbot、Grabbot 等誤聽）。重點是把兩圈接起來，讓 agent 能自己取用真實資料，而不是由人當中間代理人、也不是靠猜測。主持人以「一次湧進約 30 則議題」為例問協調者怎麼分派；講者說協調者可以依任務長出不同拓撲。不要把這個例子寫成「講者自報同時跑 30 多個 agent」。她也說，要走到這麼高的 PR 量，關鍵之一是倒過來問：怎樣才能讓 agent 合併自己的程式；主持人隨即把「你怎麼審查這麼多 PR」留到後面。其他做法包括：不要一看到問題就立刻派出大量修復 agent，可先讓例行工作把模式（她舉 React 的常見陷阱）追加到一份文件，隔幾天再一起看，以免只顧著執行而錯過全貌。片尾談到 pstack 與主持人自己的 skills：技能本質上是把流程寫成語言／Markdown，可以交織使用，但每個人仍要打磨自己的「刀」；建議回看自己以往的對話紀錄，把重複要介入、糾正的地方收成可重用技能。pstack 的授權與 SkillSpector 掃描見 SEQ 0144。準備當日所見，官方 YouTube 約 363,312 次觀看，Facebook 轉發約 52,200 次，兩者都只是當日快照。本則是對談錄影，幾乎都是講者在家庭工作空間出鏡、右下角有主持人小窗與燒錄英文字幕，沒有清楚的投影片可做成 GIF，故不附 GIF（金字塔圖見 SEQ 0144）。配樂：對談現場，曲名未標。

互動 Demo：[trust-ladder-loops](https://wiki.singularityengine.dev/demos/trust-ladder-loops/)

#### 分段重點與時間軸

對照官方原片：[YouTube](https://www.youtube.com/watch?v=MN9dGgmLyso)。時間碼依官方片（約 1:05:36）。Facebook 轉發少了約 35 秒開場，從講者說「Thanks for having me」接上。下列為重點整理，不是逐字稿；完整逐字稿只放在私人檔案庫。數字為講者／主持人自述，未查核。

- **00:00** 主持人 Matt Pocock 介紹；講者約在 **00:36** 說「Thanks for having me」。
- **01:08** 主持人轉述她約 10 天前的演講，以及「上月送到 production 的 2,500 個 PR」相關貼文（主持人稱約 300 萬次觀看，未查核）。本則是那場之後的直播問答，不是 SEQ 0144。
- **01:36** 信任階梯：先能信任，再擴大並行。
- **01:58** 講者說這段路在加入 Cursor 之前就開始。口頭說「Cursor which is now SpaceX AI」，正式名稱以畫面 Logo 與 SEQ 0144 的 SpaceXSI 為準。約 1、2 月時花很多時間微觀管理單一 agent。
- **11:10** Michelin 廚房隱喻：不喜歡 software factory 容易讓人忽略品質與技藝；從一個人做完全部備料的家庭煮手，到請助手分工，再到主廚負責組織廚房、仍對成品負責。
- **33:01** 談到 2,000／2,500 個 PR 從何而來：先把環境準備好，再談規模。內圈是朝一份意圖快照寫程式的 agent；外圈從 Slack、X、email、Linear 把脈絡拉回來。外圈工具寫成 Grok Bot。
- **39:10** Cursor projects 作為雲端協調／幕僚型 agent，自己少動手、負責委派子 agent。
- **41:38** 講者提到在 Netflix 帶團隊時聽過的「context not control」：給脈絡，而不是靠控管去微觀管理。
- **43:28** 主持人以一次湧進約 30 則議題為例。不要把這個例子寫成「講者自報同時跑 30 多個 agent」。Facebook 轉發文案的每月 1,000 個 PR、醒來已有 20 個 PR 等與本則不符。
- **46:01** 澄清：2,500 個 PR 顯然不是 2,500 個功能，很多是 gardening。不要和 SEQ 0144 較晚演講的數字混在一起。
- **47:24** 例行工作可先把重複模式寫進緩衝文件（她舉 React 的常見陷阱），隔幾天再看，以免只顧執行而錯過全貌。
- **59:49** pstack 與主持人的 skills 可以交織；技能本質上是把流程寫成語言。每個人仍要打磨自己的「刀」，並可從過去的對話裡，把重複要糾正的地方收成技能。pstack 掃描見 SEQ 0144。

### 0096　[Lamis Mukta（Anthropic）：從 CLAUDE.md 到 Dreaming 的 agent 記憶演進](https://www.youtube.com/watch?v=tTcxVv8HHNw)
{: #seq-0096}

Anthropic 工程師談 agent 記憶：CLAUDE.md→tool memory→skills→memory/ 目錄，再到非同步 Dreaming 整併

| 可信度 | 星數 | 出處 |
| --- | --- | --- |
| 可信度高・宣稱待驗證（說明文框架） | — | [影片 49](https://x.com/David_eficaz/status/2118745007628726684) |

David（@David_eficaz）轉貼的約 31 分鐘英文會議演講：Lamis Mukta（Member of Technical Staff, Anthropic）在 AI DevCon by Tessl 講 agent 記憶。完整時間軸見下方分段重點（依約 31 分鐘演講錄影重對；官方活動名稱為 AI Native DevCon）。演講中的量化宣稱（例如「97% fewer first pass errors」）屬宣稱待驗證。X 說明文提到「Opus 5.5」「不要 prompt、要建自 prompt 系統」等框架，演講本身未出現 Opus 5.5——說明文框架標宣稱待驗證。配樂：會議現場。無 GIF。

官方原片（標題 Learning while you sleep: Beyond memory to dreaming，AI Native DevCon，2026 年 6 月）：https://www.youtube.com/watch?v=tTcxVv8HHNw 。X 轉發為同一場演講錄影。本則主題與記憶與上下文相關，原分類頁留有短註。

#### 分段重點與時間軸

官方原片：[YouTube](https://www.youtube.com/watch?v=tTcxVv8HHNw)，標題 Learning while you sleep: Beyond memory to dreaming（AI Native DevCon，2026 年 6 月，Tessl）。時間碼依約 31 分鐘的演講錄影（與 [X 轉發](https://x.com/David_eficaz/status/2118745007628726684) 對應；官方 YouTube 片前可能還有主持人介紹）。下列為重點整理，不是逐字稿；完整逐字稿只放在私人檔案庫。演講中的量化宣稱維持待驗證。X 說明文的「Opus 5.5」等框架並未出現在演講裡。

- **00:00** 自介在 Anthropic 應用 AI 團隊。本場重點是 context engineering：模型變聰明本身不會自動複利，要靠脈絡才能在你的環境裡做事，並通往持續學習。
- **01:50** 大綱：回顧過去一年的脈絡工程、今日記憶管理、如何在 production 落地，最後談 dreaming。
- **03:27** 演進：先從 Claude Code 的 CLAUDE.md（簡單、有效，但會膨脹）開始，再到讓 agent 在 session 裡自己讀寫的 memory tools（in-band）。
- **05:29** Skills 與 progressive disclosure：先看檔案開頭幾句，需要時再載入詳細流程，避免一次塞滿 context。
- **10:20** Production 原則：versioning（可回溯、記錄依據哪個 session）；**11:06** concurrency（寫入前後比對 hash，不一致就重讀再試）；**11:32** permissioning（組織級知識宜偏唯讀，agent 自己的 scratch pad 可寫）；**12:48** portability（乾淨 API，跨產品面重用）。
- **13:45** 講者描述落地後的效果（第二次做得更好、用更少 token；屬講者說法，未查核）。既有條目提到的量化宣稱仍標待驗證；本則逐字稿沒有清楚對上「97% fewer first pass errors」這個數字。
- **15:05** In-band 記憶的限制：同一個 session 既要完成任務、又要整理記憶，難以兼顧，也較難看整個 agent 艦隊的模式。
- **17:51** Dreaming：非同步、批次、另配資源的二階過程，用一批 transcripts 檢查並更新記憶。
- **21:25** Production 架構：orchestrator 派出子 agent 分析 transcripts 與工具呼叫等 metadata，再提出記憶修改。
- **29:00** 問答：例如 dreaming 的觸發範圍，以及哪些該寫進 harness、哪些留給 agent 自治。
