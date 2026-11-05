# 國王的百枚硬幣 / The King's 100 Coins

用互動模擬看懂一道經典邏輯謎題：蒙著眼睛，也能把硬幣分成正面數量相等的兩堆。

An interactive simulation of a classic logic puzzle: split a pile of coins into two groups with the same number of heads, while blindfolded.

**線上試玩 / Play online: https://jeffcc.github.io/100coins/**

也可以直接用瀏覽器開啟 `index.html`，不需安裝任何東西。網頁介面目前只有繁體中文。

You can also just open `index.html` in a browser, with nothing to install. The page itself is currently in Traditional Chinese only.

## 謎題

桌上有 100 枚硬幣，10 枚正面、90 枚反面。你被蒙上眼睛，也摸不出正反。請把硬幣分成兩堆，讓兩堆的正面數量完全相同。

**解法：** 隨便摸 10 枚當一堆，再把這 10 枚全部翻面。

**為什麼成立：** 假設你摸到 k 枚正面。

- 手上有 10 − k 枚反面，翻面後變成 10 − k 枚正面。
- 桌上原本的 10 枚正面被摸走 k 枚，剩下 10 − k 枚。

兩堆都是 10 − k 枚正面。k 是多少都不影響結果，所以不必看，也不靠運氣。

## 網頁功能

- **親手操作：** 自己點選或隨機摸 10 枚，再全部翻面。可以勾選「蒙上眼睛」，體驗看不到正反的情況。
- **拉桿對照：** 拉動「摸到幾枚正面」，把手上和桌上的硬幣對齊比較。
- **所有情況列表：** 列出摸到 0 到 10 枚正面的 11 種情況，並附真實隨機實驗的次數。
- **反例：** 改摸其他數量，看兩堆的差距如何固定不變。

---

## The puzzle

There are 100 coins on a table: 10 heads and 90 tails. You are blindfolded and cannot feel which side is up. Split the coins into two groups so that both have exactly the same number of heads.

**Solution:** Take any 10 coins as one group, then flip all 10 of them.

**Why it works:** Suppose you picked up k heads.

- Your hand holds 10 − k tails, which become 10 − k heads after the flip.
- The table started with 10 heads and lost k of them, leaving 10 − k.

Both groups have 10 − k heads. The value of k does not matter, so you never need to look and luck plays no part.

## Features

- **Try it yourself:** Pick 10 coins by hand or at random, then flip them all. Turn on the blindfold option to play without seeing the coins.
- **Side-by-side slider:** Change how many heads you picked and compare the coins in your hand with those on the table.
- **Every case:** A table of all 11 outcomes (0 to 10 heads picked), with counts from real random trials.
- **Counterexample:** Pick a different number of coins and see the gap between the groups stay fixed.

## 技術說明 / Technical notes

單一 HTML 檔案，沒有建置步驟。字型來自 Google Fonts。

A single HTML file with no build step. Fonts come from Google Fonts.

訪客統計使用 GoatCounter（只在 GitHub Pages 上啟用），代碼設定在 `index.html` 開頭的 `GOATCOUNTER`。

Visitor stats use GoatCounter (only enabled on GitHub Pages). The account code is set in `GOATCOUNTER` at the top of `index.html`.
