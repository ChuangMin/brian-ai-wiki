# K 線回放圖表演示

影片 3（[TradingView K 線回放圖表動畫](https://www.facebook.com/reel/1632204671708366)）的自包含重現：單一 `index.html`，用 canvas 畫，沒有外部依賴。畫面上的價格都是模擬的示範資料，不是真實行情。

用瀏覽器直接開啟 `index.html` 即可播放。GitHub 的檔案預覽不會執行這份頁面。若要在網上提供，可以把這個倉庫交給 GitHub Pages（此倉庫尚未啟用或設定 Pages）。

線上版：<https://wiki.singularityengine.dev/demos/chart-replay/>

## 操作

- 播放／暫停、重新開始、速度 1x／2x／4x（左下角按鈕）。
- 鍵盤：空白鍵播放或暫停，`R` 重新開始，`1`／`2`／`4` 切換速度，`H` 隱藏或顯示控制列（含「返回 Demos 索引」）。
- 網址參數：`?clean=1` 隱藏按鈕與「返回 Demos 索引」（方便錄影），`?seed=123` 固定這一輪的示範資料，`?speed=2` 設定初始速度。可以組合，例如 `index.html?clean=1&seed=123&speed=2`。

## 調整

節奏、路徑、文字與外觀改 `<script>` 裡的 `CONFIG` 與 `COLORS`。`CONFIG` 含循環長度、K 線根數、畫面上看得到的根數、時間週期、路徑轉折（`waypoints`），以及 `chartType`（`candles` 或 `line`）。

要換成真實資料，改 `genData()`，讓它回傳 `{bars:[{o,h,l,c,v,t,ticks:[...]}], ...}`。檔案開頭的英文註解有同一份欄位說明。
