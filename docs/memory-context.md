# 記憶與上下文

中文 | [English](../en/docs/memory-context.md)

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

colbymchenry 的本地端程式碼知識圖譜（Rust 核心）：預先索引函式、類別、呼叫鏈與跨檔關係，程式碼變動時自動同步，透過 MCP server 讓 Claude Code、Cursor、Codex、Gemini、Copilot、Grok Build 等直接查詢，不必每次 grep 整個 repo；100% 本地。安裝：`curl -fsSL https://raw.githubusercontent.com/colbymchenry/codegraph/main/install.sh | sh`（或 `npm i -g @colbymchenry/codegraph`），再 `codegraph install` 接上 agent，每個專案 `codegraph init` 建索引；MIT。同名專案很多（CodeGraphContext 4.4k 星等），這個星數最高。

### [RAG Design Patterns：7 種 RAG 架構圖解](https://www.facebook.com/reel/4570321283241437)

一張圖看懂 7 種 RAG 架構：從基本檢索到多 agent 協作

| 可信度 | 星數 | 出處 |
| --- | --- | --- |
| — | — | [影片 21](https://www.facebook.com/reel/4570321283241437) |

Ankur Mishra 轉貼、@MindBoost-Tutorix（YouTube）／@MindBoostTutorix（X）製作的靜態圖表「RAG Design patterns (You must know in 2026)」。① Naive RAG（圖上誤寫成 Native RAG）：文件切塊→嵌入→向量庫，查詢嵌入後取回上下文送 LLM，適合起步與單純問答；② Retrieve-and-Rerank：取回後加 reranker 重排，適合召回夠但前幾名不準時；③ Multimodal RAG：圖片、影音一起切塊嵌入，交給多模態 LLM，適合資料不只文字時；④ Graph RAG：抽實體→LLM 建圖→圖資料庫→圖檢索，適合要跨文件推關係的問題；⑤ Hybrid RAG：向量＋關鍵字＋圖檢索合併成混合上下文，適合有專有名詞、代碼等精確匹配需求時；⑥ Agentic RAG（Router）：由 agent 決定要不要查、查哪裡，可反覆查向量庫，適合問題類型多變時；⑦ Multi-Agent RAG：總指揮 agent 分派給子 agent（程式工具、網路搜尋、向量引擎 A／B、Slack／Gmail），適合要跨多個來源與工具的任務。圖的小問題：「Native」是錯字、Hybrid 的關鍵字搜尋沒接到任何索引、Router 那格沒畫資料匯入。人工繪製，非 AI 生成。配樂：無旁白，通用的免版稅輕快 synth-pop。

### [ai-pdf-chatbot-langchain：LangGraph PDF 問答範本](https://github.com/mayooear/ai-pdf-chatbot-langchain)

用 LangGraph + Next.js 做 PDF 問答的全端範本

![ai-pdf-chatbot-langchain：LangGraph PDF 問答範本 的 GitHub 預覽](https://opengraph.githubassets.com/1/mayooear/ai-pdf-chatbot-langchain)

| 可信度 | 星數 | 出處 |
| --- | --- | --- |
| — | 16.6k | [影片 27](https://www.facebook.com/reel/1687227069493469) |

mayooear 的 monorepo 範本（也是 O'Reilly《Learning LangChain》的配套範例）：Next.js 前端＋Node／TypeScript 的 LangGraph agent，graph 節點分為匯入、檢索路由、回應；Supabase 向量庫、OpenAI LLM、token 串流、每個對話串各自保留歷史、LangSmith 追蹤。可對照影片 21 的 RAG 架構：大致是 Naive RAG 加上 Router 式的檢索判斷。維護狀態：MIT，GitHub 上已封存（archived），最後一次 commit 是 2026-03-28（台北時間），README 寫明不再維護、僅供參考。影片（AI Star Pick）是架構動畫，不是錄屏。配樂：無旁白無音樂，只有 UI 音效。

![Stack / Workflow / Delivery 三區塊依序點亮，邊框描邊動畫、節點流程圖逐步連線、底部字幕切換；可用 SVG stroke 描邊 + 分段 reveal 重現](../assets/gifs/v27-pdf-chatbot-motion-graphic.gif)

Stack / Workflow / Delivery 三區塊依序點亮，邊框描邊動畫、節點流程圖逐步連線、底部字幕切換；可用 SVG stroke 描邊 + 分段 reveal 重現

### [gbrain：YC CEO Garry Tan 開源的 agent 第二大腦](https://github.com/garrytan/gbrain)

Garry Tan 開源的 OpenClaw／Hermes agent 大腦，強調每筆事實保留來源

![garrytan/gbrain 的 GitHub 預覽](https://opengraph.githubassets.com/1/garrytan/gbrain)

| 可信度 | 星數 | 出處 |
| --- | --- | --- |
| 概念動畫・可信度高 | 31.9k | [影片 46](https://x.com/imryven/status/2119433356584604119) |

Ryven（@imryven）上傳的 27 秒 X 影片，畫面是 GBRAIN／GARRY TAN 字樣與發光節點網路的動態設計（非真實錄屏），沒有在畫面上打出完整 URL；說明文寫「YC CEO 開源自己的 second brain」並點名 gbrain (by garrytan)。查證：https://github.com/garrytan/gbrain 存在，MIT，簡介「Garry's Opinionated OpenClaw/Hermes Agent Brain」，GitHub API 2026-11-09 為 31.9k 星／4.7k fork，未封存、最近推送 2026-11-09（台北時間）。配樂：未標。GIF 片段：0:00–0:02.5（https://wiki.singularityengine.dev/assets/gifs/v46-gbrain-network.gif）。SkillSpector 掃描待補（本批不 clone）。

![gbrain 節點網路](../assets/gifs/v46-gbrain-network.gif)

GIF：影片 0:00–0:02.5，gbrain 節點網路動態設計。

### ⚠️ [Altair AI：Claude Second Brain（Obsidian repo 清單＋純 Markdown 變體）](https://github.com/kepano/obsidian-skills) ⚠️

Altair AI 多支動態片與概念動畫：Obsidian repo 清單、純 .md＋CLAUDE.md 地圖、隔夜一指令整理筆記，以及 Prakhar Saxena 同家族概念片（三種回答結果、people 名片欄位；畫面皆非真實運作軟體）

![kepano/obsidian-skills 的 GitHub 預覽](https://opengraph.githubassets.com/1/kepano/obsidian-skills)

![AgriciDaniel/claude-obsidian 的 GitHub 預覽](https://opengraph.githubassets.com/1/AgriciDaniel/claude-obsidian)

![Astro-Han/karpathy-llm-wiki 的 GitHub 預覽](https://opengraph.githubassets.com/1/Astro-Han/karpathy-llm-wiki)

![undefined-ui/second-brain-os 的 GitHub 預覽](https://opengraph.githubassets.com/1/undefined-ui/second-brain-os)

![vouchdev/vouch 的 GitHub 預覽](https://opengraph.githubassets.com/1/vouchdev/vouch)

| 可信度 | 星數 | 出處 |
| --- | --- | --- |
| ⚠️ 引流・概念動畫・可信度中 | — | ⚠️ [影片 48](https://www.facebook.com/reel/1666945238466731) ⚠️；[影片 51](https://www.facebook.com/reel/2062559707739569)；[X @Flinzu](https://x.com/Flinzu/status/2119892851387769273)；[影片 61](https://www.facebook.com/reel/3503498356478626)；[影片 77](https://www.facebook.com/reel/1473932208004781)；[影片 86](https://www.facebook.com/reel/3002409066786760) |

Altair AI 動態設計短片（非真實錄屏）。【影片 48】22 秒「10 AI REPOS」看板，畫面字太小多半無法辨識；說明文點名並描述流程（sources→raw→ingest→link→check→wiki→ask）。依說明文核對 GitHub（只取名稱清楚對得上的）：kepano/obsidian-skills（51.2k，與影片 47 同一 repo）；AgriciDaniel/claude-obsidian（16.3k，MIT，最近推送 2026-10-25）；Astro-Han/karpathy-llm-wiki（2.7k，MIT，Karpathy 風格 LLM wiki，最近推送 2026-07-23）；undefined-ui/second-brain-os（1.5k，MIT，最近推送 2026-11-03）；vouchdev/vouch（66，MIT，「no source means error／你核准才寫入」與文案相符）。其餘名稱（obsidian-second-brain、second-brain、llm-wiki、ai-second-brain、LLM_Wiki_SecondBrain 等）有多個同名或對不上，標為未確認、不猜測 owner。片尾要留言編號，屬引流。【影片 51】25 秒變體：不用 Obsidian／Notion／資料庫，改以純 .md 檔＋根目錄一份 CLAUDE.md 當索引地圖；三個資料夾 notes／people／projects／；規則是回答必須引用來源檔，否則回 NOT FOUND。畫面是動畫模擬儀表板，沒有真實操作步驟，也未展示 CLAUDE.md 內容；畫面上「247 files／0 hallucinations」只是模擬 UI 計數（未驗證）；「OPUS 5.5」標籤同 SEQ 0096，屬宣稱待驗證。本支無留言換連結。【X @Flinzu／影片 60】25 秒概念動畫（無實際運作軟體）。稱一堆純文字檔繞一份地圖：notes／people／projects，以及 MEMORY／LEARNINGS／decisions；先載入地圖；回答要引用檔案；Claude 不會編造你沒寫下的理由。說明文指向 @Bober_smart 的指南 https://x.com/Bober_smart/status/2078784709253841039。畫面「OPUS 5.5」標籤同 SEQ 0096，屬宣稱待驗證。無留言換連結。【影片 61】Lê Quốc Nghĩa 上傳的 Facebook Reel，同樣是概念動畫（無實際運作軟體）：raw/→wiki/，根目錄 CLAUDE.md 當地圖；說明文附完整設置提示詞。動畫出現讀取 people 檔、weekly-review skill、remember、／doctor 提示詞健檢。本支無留言換連結。【影片 77】Altair AI 上傳的約 30 秒直式 Facebook Reel（2026-11-06；Brian 於 2026-11-12 21:28 Asia/Taipei 在對話直接傳來 [這則分享連結](https://www.facebook.com/share/v/1A4xaosai3/)）。說明文自稱為 concept demo（概念示範），不是真實運作軟體。一句指令「I'm going to bed. Sort my notes into the brain」；管線角色 Intake／Split／Mapper／Dedupe／Learnings／Citer／Honest（畫面另有 Namer、Pinner、Morning 等卡片）。資料夾 notes／people／projects／decisions（帶日期的決策紀錄）。Mapper 寫 CLAUDE.md 地圖，下次 session 開始時載入。說明文列五則當天就能用的作法：一題一檔、用內容命名；用 CLAUDE.md 當資料夾地圖；回答要引用來源檔；允許說 not in the files；只釘兩個檔（例如 memory 與 decisions log）。說明文也寫 /brain-mode、/map、/pin 是這則概念裡的自訂捷徑，不是 Claude Code 內建指令，可用 skills／自訂指令自做（畫面可見 /brain-mode）。結尾數字 143 files、37 cited answers、0 guesses（畫面另寫 3 folders · 1 CLAUDE.md；與列出的四個資料夾名稱不完全一致）為概念示範計數、未驗證。說明文問 Comment 1, 2 or 3（排序、地圖或引用何者最省時間），只是互動提問、沒有換連結，不另標引流；既有 ⚠️ 仍因影片 48 留言編號而保留。片尾 Follow Altair AI 為普通追蹤呼籲。無私人資訊。【影片 86】Prakhar Saxena 上傳的約 25 秒 Facebook Reel（2026-11-09；536×670；Brian 於 2026-11-13 在對話傳來 [這則 Reel](https://www.facebook.com/reel/3002409066786760)）。說明文同樣是純文字檔繞一份地圖、不靠 App；片尾要「save it」，只是普通收藏呼籲，不是留言換連結，不另標引流；既有 ⚠️ 仍因影片 48 留言編號而保留。畫面是與影片 51、Flinzu／影片 60 同一家族的概念儀表板動畫（OPUS 5.5、247 files、CLAUDE.md 當地圖、CITED／NOT FOUND），不是真實運作軟體；中間視覺是漩渦（說明文稱 storm），有別於 Flinzu 的軌道與影片 51 的「+ ONE INDEX FILE」加 Altair 追蹤橫幅。既有 GIF 已涵蓋這類畫面，本支不另做 GIF。「OPUS 5.5」標籤同 SEQ 0096，屬宣稱待驗證。相對既有來源，本則補上或寫得更清楚的有：三種回答結果——sourced（打開並點名一個檔）、never stored（告訴你沒存過，而不是硬補）、new（新建一個檔，地圖加一行）；people 名片欄位為角色、負責什麼、怎麼聯絡；根目錄放長期記憶、lessons，以及「為什麼這樣決定」的 decision log（與 Flinzu 已寫的 MEMORY／LEARNINGS／decisions 相同，說明文強調的是 why）。說明文附一段可貼進空資料夾的 5 步提示詞（先顯示布局再建立）：建 notes／people／projects；在根目錄加 memory、lessons 與 decision log；寫一份地圖並讓 memory 與 decisions 保持在焦點；一題一檔、以內容小寫連字號命名；只從地圖指出的檔作答並點名，沒有就明說。Flinzu 的 X 說明文在本則存檔裡被截斷，沒有對得到完整 paste 提示詞，故不宣稱兩者逐字相同；整體設定與 Flinzu／影片 51 是同一套。無私人資訊。配樂：未標。GIF（影片 51）：0:03–0:06。GIF（影片 77）：0:24–0:29。SkillSpector 掃描待補（本批不 clone）

![純 .md 第二大腦模擬儀表板](../assets/gifs/v51-altair-plain-md-second-brain.gif)

![隔夜一指令整理筆記進第二大腦的概念示範收尾](../assets/gifs/v74-altair-overnight-brain-sort.gif)

此則的影片 48 為引流：標題與影片 48 連結旁保留 ⚠️；影片 51／60／61／77／86 與 Bober_smart 指南無留言換連結，不加 ⚠️。

### [Lamis Mukta（Anthropic）：從 CLAUDE.md 到 Dreaming 的 agent 記憶演進](https://x.com/David_eficaz/status/2118745007628726684)

Anthropic 工程師談 agent 記憶：CLAUDE.md→tool memory→skills→memory/ 目錄，再到非同步 Dreaming 整併

| 可信度 | 星數 | 出處 |
| --- | --- | --- |
| 可信度高・宣稱待驗證（說明文框架） | — | [影片 49](https://x.com/David_eficaz/status/2118745007628726684) |

David（@David_eficaz）轉貼的約 31 分鐘英文會議演講：Lamis Mukta（Member of Technical Staff, Anthropic）在 AI DevCon by Tessl 講 agent 記憶。重點時間碼：記憶演進 CLAUDE.md→tool memory→skills→由 agent 管理的 memory/ 目錄（03:16）；skills 的 progressive disclosure（05:30）；編輯記憶檔前後用 hashing 做 concurrency control（10:05）；記憶權限——組織知識唯讀 vs scratchpad 可讀寫（11:45）；in-band 記憶更新的限制（14:59）；Dreaming：非同步、out-of-band 批次從 transcript 整併記憶（17:49）；Dreaming 架構——orchestrator＋子 agent 找重複錯誤（21:27）。演講中的量化宣稱（例如「97% fewer first pass errors」）屬宣稱待驗證。X 說明文提到「Opus 5.5」「不要 prompt、要建自 prompt 系統」等框架，演講本身未出現 Opus 5.5——說明文框架標宣稱待驗證。配樂：會議現場。無 GIF。

### [Altair AI：Obsidian CEO 開源的 Claude＋Obsidian 工具清單](https://github.com/kepano/defuddle)

動態看板整理 kepano／Obsidian 官方開源的 Claude＋Obsidian 工具：skills、Defuddle、Clipper、Help、Importer

![kepano/defuddle 的 GitHub 預覽](https://opengraph.githubassets.com/1/kepano/defuddle)

![obsidianmd/obsidian-clipper 的 GitHub 預覽](https://opengraph.githubassets.com/1/obsidianmd/obsidian-clipper)

![obsidianmd/obsidian-help 的 GitHub 預覽](https://opengraph.githubassets.com/1/obsidianmd/obsidian-help)

![obsidianmd/obsidian-importer 的 GitHub 預覽](https://opengraph.githubassets.com/1/obsidianmd/obsidian-importer)

| 可信度 | 星數 | 出處 |
| --- | --- | --- |
| 概念動畫・可信度高 | —（各 repo 見內文） | [影片 50](https://www.facebook.com/reel/1895633831459873) |

Altair AI 上傳的 25 秒 Facebook Reel（2026-11-08），動態設計（非真實錄屏），橫幅 Follow Altair AI；說明文稱 Obsidian CEO（kepano）開源 Claude＋Obsidian 工具。OPEN SOURCE 面板列出五個項目（畫面星數／API 2026-11-09）：① [kepano/obsidian-skills](https://github.com/kepano/obsidian-skills)（畫面 58.0k、API 51.2k）→ 已見 SEQ 0094／0095，本則只交叉引用、不重複建檔；② [kepano/defuddle](https://github.com/kepano/defuddle)（畫面 9.0k、API 9.9k，MIT，把網頁主內容轉成 Markdown，最近推送 2026-10-25）；③ [obsidianmd/obsidian-clipper](https://github.com/obsidianmd/obsidian-clipper)（畫面 5.5k、API 5.5k，MIT，官方 Web Clipper 擴充功能，最近推送 2026-09-22）；④ [obsidianmd/obsidian-help](https://github.com/obsidianmd/obsidian-help)（畫面 1.9k、API 2.0k，官方說明文件 repo，最近推送 2026-11-07）；⑤ [obsidianmd/obsidian-importer](https://github.com/obsidianmd/obsidian-importer)（畫面 1.7k、API 1.7k，MIT，把 Apple Notes／OneNote 等轉成 Markdown，最近推送 2026-10-21）。五個帳號與 repo 皆可直接開啟。配樂：未標。SkillSpector 掃描待補（本批不 clone）。

![動態設計 OPEN SOURCE 面板：obsidian-skills、defuddle、clipper、help、importer](../assets/gifs/v50-altair-obsidian-open-source.gif)

GIF：影片 0:01–0:03.5，OPEN SOURCE 工具清單看板（動態設計，非錄屏）。
