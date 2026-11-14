# Saga pattern（影片 93）

依 Know Your System 影片 93 的六張圖卡，在瀏覽器裡跑一筆虛構結帳：Order／Payment／Inventory／Shipping。可切換事件協同（event bus）或編排（中央協調者），也可切換庫存有貨或缺貨，再一步步看補償（退款／取消，不是回滾）。一致性標成最終一致，頁面不會連網。

開啟 `index.html` 即可（不需伺服器）。
