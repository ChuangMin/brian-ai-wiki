# API 設計八則／Eight API design practices

依 Aman Views「API Design 八則」動畫圖卡做的互動頁：八張可操作卡片，分別對應 Clear Naming、Idempotency、Pagination、Filter & Sort、Resource Paths、Rate Limiting、Versioning、Security，並加上實務補充。這不是原圖翻製，示例資料都是虛構的，也不會連網。權杖只顯示 `Bearer <token>`。

來源圖卡的說明文是另一套 10 點清單（狀態碼、錯誤內容、快取、OpenAPI 等），與畫面上的八則並不完全一致。本頁以畫面為準。這八則清單廣泛沿用 ByteByteGo／Sahn Lam 的整理。

補充重點：圖上 Update 只畫 PUT，部分更新應是 PATCH（RFC 5789）。冪等定義見 RFC 9110；Idempotency-Key 是應用層慣例。offset 分頁在列表變動時會漂移。巢狀路徑是風格不是規則。URI 版本只是做法之一。HTTPS 加 bearer 是基本盤。限流觸及時示範 429 與 Retry-After。限流額度在本頁縮成 8 次，方便操作（影片例子是 100 req/min）。

English: an interactive walkthrough of the eight on-screen rules, with caveats, an original layout, and fictional data. Open `index.html`. Toggle 中文 / English, or append `?lang=en`.

對應公開站條目：影片 103／SEQ 0147。Live: https://wiki.singularityengine.dev/demos/api-design-best-practices/
