# 系統設計與工程基礎

中文 | [English](../en/docs/systems-design.md)

[回首頁](../README.md)

非 AI 的後端／分散式系統基礎與維運常識（如 TLS 健檢）

### [12 個系統設計基本概念](https://www.facebook.com/reel/3285768298275601)

12 個系統設計基本概念一句話速查

| 可信度 | 星數 | 出處 |
| --- | --- | --- |
| — | — | [影片 22](https://www.facebook.com/reel/3285768298275601) |

Code Crack 的 13 秒動態圖卡（深色格線背景、12 張卡片依序亮起、無旁白，人工製作非 AI 生成）：Load Balancer 分散流量；Caching 快取重複查詢；CDN 把內容放到靠近使用者的地方；Sharding 資料分片；Replication 複本供讀取與容錯；Message Queue 非同步可靠處理；Rate Limiting 限流；Consistent Hashing 加節點時不必大量重分配；CAP 一致性／可用性／分區容錯；Idempotency 重試無害；Circuit Breaker 熔斷避免連鎖故障；Observability 用 logs／metrics／traces 看清系統。更正：圖上 CAP「三選二」的說法過度簡化，分區不是能選的，發生分區時只能在一致性與可用性之間擇一；沒有分區時則如 PACELC 所說，是在延遲與一致性之間取捨。配樂：UI 音效（上行的馬林巴鐘聲、結尾提示音）疊在微弱的通用輕快科技感節拍上。

![深色格線背景 3×4 卡片依序淡入，每張卡內有小型示意動畫（流量分流點、快取方塊、分片條）並輪流綠框高亮；可用 CSS grid + animation-delay stagger 重現](../assets/gifs/v22-system-design-cards.gif)

深色格線背景 3×4 卡片依序淡入，每張卡內有小型示意動畫（流量分流點、快取方塊、分片條）並輪流綠框高亮；可用 CSS grid + animation-delay stagger 重現

### [10 個指令檢查網站 HTTPS](https://www.facebook.com/reel/4523349764619784)

從憑證到期、HSTS 到舊版 TLS，10 個指令快速健檢 HTTPS

| 可信度 | 星數 | 出處 |
| --- | --- | --- |
| — | — | [影片 23](https://www.facebook.com/reel/4523349764619784) |

Code Crack（CodeCrackAI）的動態終端機圖卡「SECURITY • TLS FIRST AID」，示範輸出以紅字標出憑證到期日、仍開著 TLSv1.0、`server: nginx/1.18.0` 洩漏版本。人工製作，非 AI 生成。十項檢查：`curl -sI` 看是否回應；`openssl s_client` 取憑證；`openssl x509 -enddate` 看到期日；`-issuer` 看簽發者；`-ext subjectAltName` 看涵蓋哪些網域；HTTP 是否用 `location` 導向 HTTPS；是否有 `strict-transport-security`（HSTS）；`nmap --script ssl-enum-ciphers` 找舊協定；`server` 標頭是否洩漏版本；`dig CAA` 看誰可以簽發憑證。更正：第 2 步說「存成 cert.pem」，但指令本身沒有存檔，應為 `echo | openssl s_client -connect example.com:443 -servername example.com 2>/dev/null | openssl x509 > cert.pem`，且要加 `-servername` 才會帶 SNI。實測 wiki.singularityengine.dev（2026-10-31）：HTTP/2 200；Let's Encrypt（YR2）簽發、2027-01-29 到期；SAN 只有 wiki.singularityengine.dev；`server: GitHub.com`；但 http:// 回 Cloudflare 500、沒有導向，也沒有 HSTS 標頭；singularityengine.dev 沒有 CAA 紀錄。配樂：無人聲與音樂，只有 UI 嗶聲與結尾和弦。另見「安全與治理」分類。

![左側步驟清單橘色高亮逐項前進、右側終端機逐行打出指令與輸出、紅字標出風險；背景綠色流動線條；可用 typewriter 效果 + 步驟 active class 重現](../assets/gifs/v23-https-terminal-steps.gif)

左側步驟清單橘色高亮逐項前進、右側終端機逐行打出指令與輸出、紅字標出風險；背景綠色流動線條；可用 typewriter 效果 + 步驟 active class 重現

### [Kafka 架構手寫風筆記](https://www.facebook.com/reel/3443590945824757)

一張手寫風筆記看懂 Kafka 架構（注意 ZooKeeper 已過時）

| 可信度 | 星數 | 出處 |
| --- | --- | --- |
| — | — | [影片 25](https://www.facebook.com/reel/3443590945824757) |

softwaredeveloper077 的 15 秒靜態圖，數位手寫風筆記「KAFKA ARCHITECTURE」分 11 塊：Producers；Cluster／Brokers；Consumers；Topics；Partitions（有序、不可變，提供平行度）；Replication（leader／followers）；ZooKeeper；資料流（offset、commit）；好處；使用情境；最佳實務（topic 名稱要有意義、partition 數量要合適、開複本、監控 consumer lag、依時間與大小設 retention、用 consumer group、調 batch size）。無浮水印，字跡乾淨，看起來是人工製作，但無法完全排除 AI。更正：ZooKeeper 已過時，KRaft 取代它（3.3 起可用於正式環境，4.0 移除 ZooKeeper）。配樂：通用的免版稅輕快電子／House。

### [BFS 廣度優先搜尋：幾步找到 Crush](https://www.facebook.com/reel/1108544155324652)

用「朋友的朋友」一圈圈往外找，說明 BFS 為何能找到最短路徑

| 可信度 | 星數 | 出處 |
| --- | --- | --- |
| 可信度高・程式小 bug | — | [影片 30](https://www.facebook.com/reel/1108544155324652) |

thachdv.it（越南語）的 BFS 動畫，文案「Thuật toán tìm kiếm theo chiều rộng - BFS. Cách các nền tảng giúp b dò nhà crush 😁」（BFS 演算法：平台怎麼幫你找到 crush 的家）。圖以「YOU」為中心排成同心圓，目標「Crush」在第 4 圈；檢查到的節點會亮起，QUEUE 列顯示節點加入與取出（FIFO），另有 CHECKED 與 RING 計數。步驟：先查朋友、再一圈圈查朋友的朋友；佇列維持先進先出；第一次找到就停；最後標出最短路徑「4 handshakes: the fewest there are」。畫面程式：`queue, seen = deque([you]), {you}`，`while queue: u = queue.popleft(); if u == crush: break; for v in friends[u]: if v not in seen: seen.add(v); came[v] = u; queue.append(v)`。正確性：無權重圖上 BFS 確實給出最短路徑（幾度分隔）。小 bug：`came` 沒有初始化（要先 `came = {}`），照抄會出現 NameError。文案說「找 crush 的家」，但影片只講社交關係的握手數；真的地圖導航道路有權重，要用 Dijkstra／A*。配樂：8-bit chiptune，無旁白。GIF 片段：0:00–0:11。

![BFS 由 YOU 一圈一圈向外擴散（節點依層著色）、上方 CHECKED/RING 計數、下方程式碼逐行高亮與 QUEUE 圓點進出，找到後以金色標出最短路徑；可用 SVG 節點 + 逐步狀態機 + 程式碼行高亮重現](../assets/gifs/v30-bfs-ring-expansion-queue.gif)

BFS 由 YOU 一圈一圈向外擴散（節點依層著色）、上方 CHECKED/RING 計數、下方程式碼逐行高亮與 QUEUE 圓點進出，找到後以金色標出最短路徑；可用 SVG 節點 + 逐步狀態機 + 程式碼行高亮重現

▶ 互動 Demo：[開啟](../demos/bfs/)（https://wiki.singularityengine.dev/demos/bfs/）

### [Prim 演算法：最小生成樹](https://www.facebook.com/reel/2132850694107274)

從一個點開始，每次挑最便宜的往外邊，長出連接所有點的最省樹

| 可信度 | 星數 | 出處 |
| --- | --- | --- |
| 可信度高 | — | [影片 31](https://www.facebook.com/reel/2132850694107274) |

Software with John 的動畫（文案「Prim's Algorithm #dsa」），無向圖 A–G，邊：A-B 4、A-C 2、B-C 1、B-D 5、B-E 9、C-D 8、C-F 10、D-E 3、D-F 2、E-F 4、E-G 3、F-G 3。從 A 開始依序選：A-C(2)、C-B(1)、跳過 A-B(4)（B 已在樹中，會形成環，閃紅）、B-D(5)、D-F(2)、D-E(3)、F-G(3)，總權重 16。畫面重點：「Grow one tree outward from a start node, always taking the cheapest edge that leaves it.」（從起點長出一棵樹，每次都挑離開這棵樹最便宜的邊）。程式：Python `heapq`，`v in seen` 就跳過，再把鄰邊推進 heap；複雜度標示時間 O(E log V)、空間 O(E)。正確性：已驗算，總和 16 就是最小生成樹（用 Kruskal 交叉驗算也是 16）。畫面：深色背景，heap 裡的邊是藍色虛線，選中的邊發青光，捨棄的邊閃紅。配樂：未確認（分析時沒有音軌）。GIF 片段：0:02–0:07（含閃紅跳過）。

![Prim 演算法：從 A 起逐步把最小邊加入樹（青色實線）、候選邊在 heap 中以虛線表示、已在樹內的邊以紅色標示跳過，下方程式碼與說明同步；可用 SVG 邊線 class 切換 + 步驟資料陣列重現](../assets/gifs/v31-prim-mst-heap-edges.gif)

Prim 演算法：從 A 起逐步把最小邊加入樹（青色實線）、候選邊在 heap 中以虛線表示、已在樹內的邊以紅色標示跳過，下方程式碼與說明同步；可用 SVG 邊線 class 切換 + 步驟資料陣列重現

▶ 互動 Demo：[開啟](../demos/prim/)（https://wiki.singularityengine.dev/demos/prim/）

### [每個工程師都該知道的 5 個 GitHub repo](https://www.facebook.com/reel/1849291249414632) ⚠️

五個經典 GitHub repo：自己重做工具、學習路線圖、系統設計、免費書、演算法

![codecrafters-io/build-your-own-x 的 GitHub 預覽](https://opengraph.githubassets.com/1/codecrafters-io/build-your-own-x)

![nilbuild/developer-roadmap 的 GitHub 預覽](https://opengraph.githubassets.com/1/nilbuild/developer-roadmap)

![donnemartin/system-design-primer 的 GitHub 預覽](https://opengraph.githubassets.com/1/donnemartin/system-design-primer)

![EbookFoundation/free-programming-books 的 GitHub 預覽](https://opengraph.githubassets.com/1/EbookFoundation/free-programming-books)

![TheAlgorithms/Python 的 GitHub 預覽](https://opengraph.githubassets.com/1/TheAlgorithms/Python)

| 可信度 | 星數 | 出處 |
| --- | --- | --- |
| ⚠️ 引流・可信度高 | — | [影片 32](https://www.facebook.com/reel/1849291249414632) ⚠️ |

James Mcquay 的真人口述片（貼文文案「Comment “AI”」，片中又要觀眾留言「Github」由私訊送連結，是留言導流；不過沒藏私，每個 repo 名稱都有念出來也有上字幕）。畫面字幕「10/10 GitHub repositories to make you an elite developer」屬誇大行銷。① build-your-own-x（⚠️ https://github.com/codecrafters-io/build-your-own-x ⚠️）：從零重做 Git、Docker、資料庫等，557.8k ⭐（影片說 485k，已過時）；② roadmap.sh（⚠️ https://github.com/nilbuild/developer-roadmap ⚠️，原 kamranahmedse/developer-roadmap，已改名）：後端、前端、DevOps、AI 學習路線圖，370.9k ⭐；③ system-design-primer（⚠️ https://github.com/donnemartin/system-design-primer ⚠️）：快取、負載平衡、可擴展性，376.3k ⭐；④ free-programming-books（⚠️ https://github.com/EbookFoundation/free-programming-books ⚠️）：免費書與課程，400.6k ⭐；⑤ TheAlgorithms/Python（⚠️ https://github.com/TheAlgorithms/Python ⚠️）：各種演算法實作，225.7k ⭐。星數為 2026-10-31 查詢。可信度：高，repo 都是真的經典專案，只有「elite developer」說法誇大。配樂：輕柔 lo-fi 背景音樂。靜態口述，無 GIF 片段。

### [Altair AI：Karpathy 的六個免費 GitHub 專案（含 LLM Wiki gist）](https://www.facebook.com/reel/1655634979372088)

動態儀表板介紹 Karpathy 六個公開專案。五個 GitHub repo 都在、星數與說明文大致相符；LLM Wiki 是 gist，完整網址已找到，說明文寫 50K 星與畫面／gist 頁面不符

| 可信度 | 星數 | 出處 |
| --- | --- | --- |
| 概念動畫・可信度高 | — | [影片 78](https://www.facebook.com/reel/1655634979372088) |

Altair AI 上傳的約 22 秒直式 Facebook Reel（2026-11-12；Brian 於 2026-11-12 22:00 Asia/Taipei 在對話傳來 [這則 Reel](https://www.facebook.com/reel/1655634979372088)）。畫面是風格化科幻 HUD（標題 KARPATHY／REPO SWARM），不是真實操作錄屏，無私人資訊。說明文列出六個項目（原連結寫 http，本則改用 https），並稱合計超過 30 萬星；片尾要人 Save these 六個 repo，只是普通收藏呼籲，不是留言換連結，不標引流。片尾另有 Follow Altair AI 橫幅，同屬普通追蹤呼籲。

查證（2026-11-12 台北時間，GitHub API，皆為 karpathy 帳號下的公開專案）：

1. [karpathy/autoresearch](https://github.com/karpathy/autoresearch)：說明文 92.7K，API 99,902，license 欄為空
2. [karpathy/nanoGPT](https://github.com/karpathy/nanoGPT)：說明文 64.4K，API 64,676，MIT
3. [karpathy/nanochat](https://github.com/karpathy/nanochat)：說明文 60.2K，API 60,508，MIT
4. LLM Wiki：說明文寫 50K，連結被截成 gist.github.com/karpathy/442a6。完整 gist 已找到 [gist.github.com/karpathy/442a6bf555914893e9891c11519de94f](https://gist.github.com/karpathy/442a6bf555914893e9891c11519de94f)（檔名 llm-wiki.md）。查證當日 gist 頁面星數只顯示 5,000+（GitHub 對 gist 的顯示上限），API 回 502 未取到精確數字；畫面卡片與底欄寫 5.8K gist，與說明文 50K 不符
5. [karpathy/llm.c](https://github.com/karpathy/llm.c)：說明文 31.4K，API 31,452，MIT
6. [karpathy/micrograd](https://github.com/karpathy/micrograd)：說明文 18.7K，API 18,881，MIT

前五個 repo 的 API 星數合計 275,419，再加上 gist 至少 5,000+，接近畫面標題列的 277.6K；說明文「超過 30 萬星」把 gist 算成 50K，偏高。畫面總覽把六個都標 MIT，但 autoresearch 與該 gist 在查證當日看不到 SPDX 授權，不以畫面為準。可對照 SEQ 0095（其中 Astro-Han/karpathy-llm-wiki 是這個 gist 構想的衍生實作）、0077（另一則工程師該看的 GitHub repo 清單）。SkillSpector 掃描待補（本批不 clone；routines 暫停中）。配樂：未標。GIF：0:10–0:15。

![Karpathy REPO SWARM 風格化儀表板](../assets/gifs/v75-karpathy-six-repos.gif)

### [Know Your System：Saga pattern（跨服務補償交易：編排 vs 事件協同）](https://www.facebook.com/reel/2222208475400708)

六張圖卡說明跨四個服務結帳時，失敗要用補償（退款而不是回滾），並對比事件協同與編排。畫面的 Consistent 是最終一致，不是 ACID 隔離；影片沒提到編排中心可能成為單點故障。

| 可信度 | 星數 | 出處 |
| --- | --- | --- |
| 可信度高 | — | [影片 93](https://www.facebook.com/reel/2222208475400708) |

Know Your System 上傳的約 30 秒直式 Facebook Reel（2026-11-14 18:30 Asia/Taipei；360×640；Brian 於 2026-11-14 21:56 Asia/Taipei 從電腦傳來[這則 Reel](https://www.facebook.com/reel/2222208475400708)）。說明文只寫「Payment charged, but the item is out of stock」與 Saga pattern 標籤，沒有留言換連結，故不標引流。畫面是深色格線上的手做系統設計圖卡（標題 Saga Pattern · System Design），無旁白字幕，不是 AI 工具介紹。

六張卡依序為：

1/6 PARTIAL FAILURE：Order Pending、Payment Charged、Inventory No stock、Shipping 尚未動作。畫面用虛線框標 one ACID tx 並打叉，寫 Money taken, no item，接著 2PC 也打叉，並標 locks held、tight coupling。

2/6 LOCAL STEPS：四個服務各有本地正向與補償動作——Order Create／Cancel、Payment Charge／Refund、Inventory Reserve／Release、Shipping Ship（失敗路徑下補償為 —，因為還沒出貨）。並標 local tx、compensation、eventually consistent。

3/6 COMPENSATE：庫存失敗後 Payment 改為 Refunded、Order 改為 Canceled，大標 Consistent，並寫 Refund, not rollback。這裡的 Consistent 是卡 2 已寫出的最終一致（eventual consistency），不是單一資料庫 ACID 交易的隔離或自動回滾；補償是另做一筆反向本地交易（例如退款），見 [microservices.io 的 Saga pattern](https://microservices.io/patterns/data/saga.html)（該文並指出 saga 缺少 ACID 的 isolation，需另做隔離對策）與 [Azure Architecture Center 的 Saga](https://learn.microsoft.com/en-us/azure/architecture/patterns/saga)（寫明各服務已提交的變更不能靠回滾還原）。

4/6 CHOREOGRAPHY：服務之間走 Event bus，事件依序 OrderPlaced、PaymentDone、OutOfStock，標 No central brain、decoupled、hard to trace。

5/6 ORCHESTRATION：由中央 Orchestrator 依序下 Create、Charge、Reserve，失敗後再下 Refund、Cancel，標 Central brain、clear flow、extra service。影片沒有提到編排中心可能成為單點故障；Microsoft 的 Saga 說明則把「orchestrator 管理整段流程，因而引入一個故障點」列為編排的缺點。

6/6 HAPPY PATH：庫存足夠時狀態變成 Created、Charged、Reserved、Booked，標 Order complete、all local tx committed。

可對照 SEQ 0067（系統設計基本概念，含訊息佇列與一致性相關卡片）、0070（Kafka 事件架構）、0075（BFS）、0076（Prim）。

互動重現：[saga-pattern 示範](https://wiki.singularityengine.dev/demos/saga-pattern/)（四個服務的虛構結帳板，可切換事件協同／編排與庫存有貨或缺貨，再一步步走補償；一致性標成最終一致，不會連網）。配樂：僅配樂、無旁白。

![Saga 圖卡：本地補償與 Refund, not rollback](../../assets/gifs/v88-saga-pattern.gif)
