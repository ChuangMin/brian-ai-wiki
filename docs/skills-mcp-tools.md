# Skills／MCP／工具

中文 | [English](../en/docs/skills-mcp-tools.md)

[回首頁](../README.md)

通用的 agent 能力元件：MCP、skill、開發方法論 skill、語音、抽取模型

### [earshot](https://github.com/Leonxlnx/earshot)

讓 agent 在本地端處理語音的工具

![earshot 的 GitHub 預覽](https://opengraph.githubassets.com/1/Leonxlnx/earshot)

| 可信度 | 星數 | 出處 |
| --- | --- | --- |
| — | 3,290 | [影片 1](https://www.facebook.com/reel/2050168028979180) |

讓 agent 在本地處理語音

### [axuse](https://github.com/ctoldigital/axuse)

透過無障礙樹操作瀏覽器的 MCP 工具

![axuse 的 GitHub 預覽](https://opengraph.githubassets.com/1/ctoldigital/axuse)

| 可信度 | 星數 | 出處 |
| --- | --- | --- |
| — | 648 | [影片 1](https://www.facebook.com/reel/2050168028979180) |

透過無障礙樹操作瀏覽器，走 MCP

### [imozuru](https://github.com/MaryCache/imozuru)

沿引用追回原始文獻的 Claude Code skill

![imozuru 的 GitHub 預覽](https://opengraph.githubassets.com/1/MaryCache/imozuru)

| 可信度 | 星數 | 出處 |
| --- | --- | --- |
| — | 1,385 | [影片 1](https://www.facebook.com/reel/2050168028979180) |

沿引用往回追到原始文獻的 Claude Code skill

### [audio-studio-mcp](https://github.com/kanaworksai-hue/audio-studio-mcp)

在本地生成音樂與音效的 MCP 工具

![audio-studio-mcp 的 GitHub 預覽](https://opengraph.githubassets.com/1/kanaworksai-hue/audio-studio-mcp)

| 可信度 | 星數 | 出處 |
| --- | --- | --- |
| — | 541 | [影片 1](https://www.facebook.com/reel/2050168028979180) |

在本地生成音樂和音效

### [Cloudflare Clairic 抽取模型](https://blog.cloudflare.com/clairic-extraction-model/)

一次前向就抽出結構化欄位的 Cloudflare 模型

| 可信度 | 星數 | 出處 |
| --- | --- | --- |
| — | — | 截圖（Marc.AI） |

2026-10-19 Workers AI 預覽模型 @cf/cloudflare/clairic：給文字（最多 4 張圖）加欄位 schema，一次前向就回傳有型別的值，不生成 token，附信心分數、null 機率與字元位置。每百萬輸入 token $0.10、輸出不收費，預告開權重。多步數學與預測仍弱

### [Superpowers](https://github.com/obra/superpowers)

讓 coding agent 先釐清需求、寫計畫、TDD 再動手的 skill 方法論

![Superpowers 的 GitHub 預覽](https://opengraph.githubassets.com/1/obra/superpowers)

| 可信度 | 星數 | 出處 |
| --- | --- | --- |
| — | 309.7k | Brian 推薦清單 2026-10-31 |

Jesse Vincent（obra）的 agentic skills 框架：agent 一開工先 brainstorming 問清楚需求、分段給你確認設計，再寫出連新手都能照做的實作計畫，強調紅綠 TDD、YAGNI、DRY，最後用 subagent-driven-development 逐項派工並審查成果；skill 會自動觸發。支援 Claude Code、Codex、Cursor、Gemini CLI、Copilot CLI、Grok Build 等。安裝：Claude Code 用 `/plugin install superpowers@claude-plugins-official`，Cursor 用 `/add-plugin superpowers`；MIT。預設會載入官網 logo 統計版本，可用 `SUPERPOWERS_DISABLE_TELEMETRY` 關閉。面試：把「需求釐清→設計確認→計畫→TDD→子 agent 實作＋審查」固化成團隊流程，就是 AI 團隊方法論的骨架

### [Matt Pocock Skills（Skills For Real Engineers）](https://github.com/mattpocock/skills)

Matt Pocock 每天用的小型工程 skill，主打先對齊再寫碼

![Matt Pocock Skills（Skills For Real Engineers） 的 GitHub 預覽](https://opengraph.githubassets.com/1/mattpocock/skills)

| 可信度 | 星數 | 出處 |
| --- | --- | --- |
| — | 307.9k | Brian 推薦清單 2026-10-31 |

TypeScript 講師 Matt Pocock 從自己 .agents 目錄公開的 skill 集，刻意做得小、可組合、不綁流程（相對 GSD、BMAD、Spec-Kit 那種接管整個流程的做法）。招牌是 /grill-me、/grill-with-docs：開工前讓 agent 反過來拷問你需求，順便建立專案共用詞彙表（ubiquitous language）並把難解釋的決策寫成 ADR，讓 agent 用詞精簡、命名一致。安裝：Claude Code 用 `claude plugin install mattpocock-skills@claude-plugins-official`，其他 agent 用 `npx skills@latest add mattpocock/skills`；MIT。面試：AI 程式碼最常見的失敗是需求沒對齊，用 grilling＋共用詞彙＋ADR 從源頭降低重工

### [Ponytail](https://github.com/DietrichGebert/ponytail)

讓 agent 像資深工程師一樣少寫程式、先重用現有元件的 skill

![Ponytail 的 GitHub 預覽](https://opengraph.githubassets.com/1/DietrichGebert/ponytail)

| 可信度 | 星數 | 出處 |
| --- | --- | --- |
| — | 181.2k | Brian 推薦清單 2026-10-31 |

DietrichGebert 的「懶惰資深工程師」skill：只寫任務需要的程式，優先重用 repo 既有元件，但不准砍驗證、錯誤處理、安全與無障礙。附 /ponytail-review（連 diff 以外受影響的檔案一起審）、/ponytail-audit 等指令。README 自述 Ponytail 5 在 Claude Code 39 個任務的測試：程式碼 -53%、時間 -41%、成本 -26%、token -45%，高風險邏輯 98% 附測試（無 skill 為 68%），屬作者自測。安裝：Claude Code 先 `/plugin marketplace add DietrichGebert/ponytail` 再 `/plugin install ponytail@ponytail`，其他 agent 可直接放 AGENTS.md；MIT。作者提醒只從這個 repo 或 npm `@dietrichgebert/ponytail` 安裝，帶 .exe／.dll 的是假冒版。面試：AI 程式碼品質不只看對不對，還要看是不是多寫了；把「最少必要程式＋不省測試與安全」寫成 review 標準

### [CLI-Anything：讓所有軟體都有命令列](https://github.com/HKUDS/CLI-Anything)

自動幫專業軟體生出命令列，讓 AI agent 不用點畫面就能操作

![CLI-Anything：讓所有軟體都有命令列 的 GitHub 預覽](https://opengraph.githubassets.com/1/HKUDS/CLI-Anything)

| 可信度 | 星數 | 出處 |
| --- | --- | --- |
| — | 57.9k | [影片 26](https://www.facebook.com/reel/1857279712725267) |

香港大學 HKUDS 的開源專案（repo 簡介：Making ALL Software Agent-Native）：替專業軟體自動產生 CLI，讓 agent 用指令操作，而不是截圖加點擊。在 Claude Code 執行 `/cli-anything <軟體路徑或 GitHub 網址>`，走 7 個階段：分析程式碼→設計 CLI→實作→規劃測試→寫測試→寫測試文件→發佈到 PyPI。會呼叫真的軟體（LibreOffice 轉 PDF、Blender 算圖），輸出結構化 JSON，文案稱有 2,000+ 個測試；CLI-Hub（https://clianything.cc/ ）讓 agent 搜尋、安裝社群做好的 CLI（SKILL.md）。影片示範 FreeCAD 做好奇號風探測車、Blender 軌道中繼無人機、《殺戮尖塔 2》CLI；但畫面上的殺戮尖塔看起來是一代不是二代，示範畫面也是 README 裡美化過的展示。和本 wiki 的 blender-skills、Spider Walker 等 DCC 項目是同一方向：讓 agent 用可測試的介面操作 3D 軟體。Python、Apache-2.0，2026-03-08 建立、5.2k fork。影片是小礦工挖挖礦的繁中 AI 配音。配樂：無。面試：要 agent 可靠又可測試，優先給它確定性、結構化的介面（CLI＋JSON），少靠 GUI 自動化

### [archify：把想法或程式碼變成互動架構圖](https://github.com/tt-a1i/archify)

讓 AI agent 把想法、計畫或程式碼轉成可互動的圖

![archify：把想法或程式碼變成互動架構圖 的 GitHub 預覽](https://opengraph.githubassets.com/1/tt-a1i/archify)

| 可信度 | 星數 | 出處 |
| --- | --- | --- |
| — | 92.0k | Brian 推薦清單 2026-10-31 |

給 Claude Code、Codex 等 agent 用的 skill，把一個想法、計畫或整個 codebase 轉成互動式圖表。Apache-2.0，2026-04-15 建立，官網 https://archify.si 。出自 Brian 的文字推薦，無影片。配樂：不適用（無影片）。面試：讓 agent 從 codebase 自動產生架構圖，審查時可以檢查文件與程式碼是否一致

### [diagram-design：編輯級品質的圖表 skill](https://github.com/cathrynlavery/diagram-design)

讓 AI agent 畫出雜誌等級的 HTML＋SVG 圖表

![diagram-design：編輯級品質的圖表 skill 的 GitHub 預覽](https://opengraph.githubassets.com/1/cathrynlavery/diagram-design)

| 可信度 | 星數 | 出處 |
| --- | --- | --- |
| — | 63.4k | Brian 推薦清單 2026-10-31 |

給 Claude Code、Codex、Copilot、Cursor 等 agent 用的圖表 skill，產出獨立 HTML 加內嵌 SVG 的編輯級品質圖表。MIT，官網 https://diagramdesign.dev 。中文 fork patrick-xin/diagram-design-zh（https://github.com/patrick-xin/diagram-design-zh ，48 ⭐）內建中日韓文字排版。出自 Brian 的文字推薦，無影片。配樂：不適用（無影片）。面試：同 archify，讓 agent 從 codebase 產生架構圖，審查時保持文件與程式碼同步

### [PPT Master：文件或主題 → 可編輯的原生 PPTX（AI 技能包）](https://github.com/hugohe3/ppt-master)

丟 PDF／Word／文字或只給主題，AI 做出文字框、形狀、圖表都能改的真 PowerPoint，不是圖片

![hugohe3/ppt-master 的 GitHub 預覽](https://opengraph.githubassets.com/1/hugohe3/ppt-master)

![hugohe3/ppt-master-examples 的 GitHub 預覽](https://opengraph.githubassets.com/1/hugohe3/ppt-master-examples)

| 可信度 | 星數 | 出處 |
| --- | --- | --- |
| 可信度高 | 71.6k | [影片 39](https://www.facebook.com/reel/1051071164608370) |

小礦工挖挖礦上傳的 1:28 影片，畫面是官方範例網站的錄影，沒有現場生成示範。給 Claude Code、Cursor、Codex CLI 用的技能包。功能：生成前先確認模板、比例、頁數等規格（要求快速模式才跳過）；圖表預設是可編輯的形狀，加參數可改成原生圖表；會加轉場與動畫，並把旁白稿寫進備忘稿；圖片來自 AI 生成或開放圖庫，並在投影片上標註來源；也能套用公司模板並保留原設計。官方範例站有 72 份簡報、1012 頁，涵蓋中、日、韓、德文；範例 repo：https://github.com/hugohe3/ppt-master-examples （22 ⭐）。需求：Python 3.10–3.14 加一個 AI 程式助理。作者提醒別期待第一次就完美，仍要自己再修。值得一看的 fork：academic-ppt-master（論文轉 PPTX）、ppt-master-plus。MIT，2025-12-10 建立，最近推送 2026-10-30。可信度：高，星數與 GitHub API 一致；片尾只問你最想先做哪份簡報，是輕微的留言引導，不算引流。配樂：輕快、俏皮的電子配樂（休閒遊戲風）。無 GIF 片段。面試：AI 產出要能「再編輯」，而不是一次定稿；human-in-the-loop 的設計，跟控管 AI 程式碼品質同一個道理

### [VibeVoice：微軟開源語音 AI（長音檔 ASR＋說話者分離＋即時 TTS）](https://github.com/microsoft/VibeVoice)

一次吃進最長約 1 小時錄音，直接輸出「誰講・幾秒・講什麼」的逐字稿，另有可在 Colab 跑的即時語音合成

![microsoft/VibeVoice 的 GitHub 預覽](https://opengraph.githubassets.com/1/microsoft/VibeVoice)

| 可信度 | 星數 | 出處 |
| --- | --- | --- |
| 可信度高 | 55.1k | [影片 40](https://www.facebook.com/watch/?v=2181912112534967) |

AI懶人報上傳的 59 秒影片，AI 語音國語旁白。重點：VibeVoice-ASR 不用先把長錄音切段，單次處理最長約 1 小時，同時做說話者分離與時間戳（誰講、幾秒到幾秒、講什麼），支援 50 多種語言，可給熱詞（hotwords）提高專有名詞辨識率（旁白念成 WhyVoice，正確是 VibeVoice）；另有即時 TTS，附 Colab T4 快速上手筆記本。示範片段是官方 demo 的 Jimmy Fallon 訪談 Lady Gaga，字幕標出講者 0／講者 1。以前要 ASR 加 diarization 兩個工具接起來，現在一個模型搞定。MIT 授權，2025-08-25 建立，最後推送 2026-10-08；影片顯示 54.9k 星。可信度：高，微軟官方 repo，影片內容與 README 一致；片尾只叫人追蹤，沒有導流。配樂：烏克麗麗加輕打擊樂。面試：會議紀錄、客服錄音這類需求，先問「要不要分講者、要不要時間戳」，一個端到端模型能省掉多工具串接的對齊與錯誤累積，但上線前要用自己的錄音抽樣驗準確率

![VibeVoice 官方 demo：Jimmy Fallon 訪談片段逐句標出講者 1／講者 0 與字幕](../assets/gifs/v40-vibevoice-diarization.gif)

GIF：影片 0:22.5–0:26，說話者分離示範。

### ⚠️ [Android 手機 AI agent（ADB 無線偵錯＋Claude Code MCP）｜預覽圖是替代方案 mobile-mcp，不是影片的 repo](https://www.facebook.com/reel/1628595922149351)

宣稱「某 GitHub repo＋Opus 5.5」能讓任何 Android 手機變成免手動 agent，但影片裡的 repo 查無此帳號；底層手法只是 ADB 無線連線加截圖、點擊、打字

替代方案預覽（不是影片裡的 repo）：⚠️ [mobile-next/mobile-mcp](https://github.com/mobile-next/mobile-mcp)

![替代方案 mobile-next/mobile-mcp 的 GitHub 預覽（不是影片的 repo）](https://opengraph.githubassets.com/1/mobile-next/mobile-mcp)

| 可信度 | 星數 | 出處 |
| --- | --- | --- |
| ⚠️ 引流・宣稱待驗證・可信度低 | —（替代方案 mobile-mcp：10.2k） | ⚠️ [影片 43](https://www.facebook.com/reel/1628595922149351) |

Tauhid IQ 上傳的 17 秒影片，沒有旁白。上半部是標題「dkrv-dev / Reverse Engineer Phone」的 GitHub 頁面（頁面顯示 17k 星、2.1k fork），About 寫「Turn any Android phone into an agent that uses its own apps over Wi-Fi. Say one sentence. Claude taps the rest.」，README 列出 tools/phone.py --probe、tools/agent.sh、claude mcp add phone tools/venv/bin/python tools/mcp.py；下半部是 Windows cmd.exe 的執行紀錄，加上一支真手機放在桌上加速播放，自己開 Telegram、再開到 Play 商店的 ChatGPT 頁面。英文說明文步驟：手機與筆電連同一個 Wi-Fi→開發人員選項開啟無線偵錯→把 repo 和手機「關於手機」截圖連同提示詞貼給 Claude Code→Opus「找到漏洞」（其實就是走網路的 ADB）→探測型號、版本、已安裝 App 並存還原點→寫出只有 3 個工具（看畫面、點擊、打字）的 agent→加進 Claude Code 當 MCP→按一次 Allow，說「open Telegram and install ChatGPT」。還宣稱支援 40 個品牌、300 多款機型、免 root；結尾寫「Find GitHub repo + full prompt below」卻沒給 repo。查證：⚠️ https://github.com/dkrv-dev 回 404（帳號不存在），GitHub API 搜尋也找不到這個 repo；而且 GitHub repo 名稱不能有空格，頁面很可能是做出來的假畫面或已刪除。Opus 5.5 只是說明文點名的模型，這裡不做判斷。可信度：低，repo 查無、數字無從驗證，加上「repo＋完整提示詞在下面」的導流寫法和誇張口吻。手法本身是真的也很普通：adb connect 走 Wi-Fi，再用截圖、點擊、輸入文字三個動作操作手機，就是標準做法。可用的替代方案（不是影片裡的 repo）：mobile-next/mobile-mcp（⚠️ https://github.com/mobile-next/mobile-mcp），10,198 星，Apache-2.0，MCP server，支援模擬器與實機，可接 Claude Code、Codex、Cursor。配樂：phonk／電子。面試：讓 agent 透過 ADB 完整控制裝置，權限面非常大，需要指令與 App 白名單、安裝與付款這類動作要人確認、限縮網路範圍（只在隔離網段開無線偵錯，用完就關）；另外，採用爆紅 repo 之前，先確認它真的存在、維護者是誰

![影片下半部：cmd.exe 執行紀錄加上桌上的手機自己開 Telegram 與 Play 商店](../assets/gifs/v43-android-adb-agent.gif)

GIF：影片 0:02–0:06，終端機紀錄與手機自動操作（加速播放）。
