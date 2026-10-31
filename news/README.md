---
lang: zh-Hant
---

<!-- 這不是新聞簡報。每日簡報是 news/YYYY-MM-DD.md。 -->

# 怎麼新增一天的新聞簡報

每天一篇。做兩件事：新增 `news/YYYY-MM-DD.md`，並在 `news/index.md` 的清單最上面加一列。不要改更早的日期檔，也不要改 `docs/`、`demos/` 或其他 wiki 頁。

公開網址：

- 索引：`https://wiki.singularityengine.dev/news/`
- 某一天：`https://wiki.singularityengine.dev/news/YYYY-MM-DD.html`

## 1. 新增 `news/YYYY-MM-DD.md`

`YYYY-MM-DD` 是簡報日期，例如 `news/2026-10-31.md`。這個檔已經存在就停：不要再開一頁，也不要在索引再加一列。

檔案用這個開頭。標題列沿用簡報原文，含 emoji 與星期：

```markdown
---
lang: zh-Hant
---

# 📰 Brian 每日新聞簡報｜YYYY/MM/DD（週）

[每日新聞](index.md) · [回首頁](../README.md)
```

標題下面照原文分段。區塊標題是原文那一行，前面加 `## `。每一則維持原來的編號與文字。

```markdown
## 🤖 AI 與科技

1. 摘要原文，一個字都不要改。

    <https://example.com/source>

2. 標題原文 — 作者

    第二行原文。

    <https://example.com/source>
```

- 不要改寫、不要翻譯、不要增刪任何一則。
- 網址單獨一行，行首空四個空格，包在 `<` 與 `>` 裡。畫面上仍是那條網址，而且可以點。
- 一則若有第二行（說明，或「頁面未提供描述」），那一行也是行首空四格，放在網址上面，中間空一行。
- 第十則以後同樣空四格，不要只空三格，否則那一行會掉出清單。

## 2. 更新 `news/index.md`

在這兩行註解中間維護清單，新的日期放最上面。註解和清單之間留空行。新的一天插在第一列：

```markdown
<!-- briefings:newest-first -->

- [YYYY/MM/DD（週）](YYYY-MM-DD.md)

<!-- /briefings -->
```

連結文字用該篇標題裡的日期與星期，例如 `2026/10/31（六）`。連結目標是檔名。同一天已經有一列就不要再加。不要把 `index.md` 或 `README.md` 寫進這個清單。
