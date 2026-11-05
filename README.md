# 國王的百枚硬幣 / The King's 100 Coins

一道經典邏輯謎題的互動版：蒙著眼睛，你要怎麼把硬幣分成正面數量相等的兩堆？第一頁只有題目，讓你自己想、自己試；想看解說再進答案頁。

An interactive version of a classic logic puzzle: blindfolded, how do you split a pile of coins into two groups with the same number of heads? The first page only poses the question so you can think and experiment. The explanation is on a separate answer page.

**線上試玩 / Play online: https://jeffcc.github.io/100coins/**

也可以直接用瀏覽器開啟 `index.html`，不需安裝任何東西。網頁介面目前只有繁體中文。

You can also just open `index.html` in a browser, with nothing to install. The page itself is currently in Traditional Chinese only.

## 謎題

桌上有 100 枚硬幣，10 枚正面、90 枚反面。你被蒙上眼睛，也摸不出正反。請把硬幣分成兩堆，讓兩堆的正面數量完全相同。

<details>
<summary>看解法（雷）</summary>

**解法：** 隨便摸 10 枚當一堆，再把這 10 枚全部翻面。

**為什麼成立：** 假設你摸到 k 枚正面。

- 手上有 10 − k 枚反面，翻面後變成 10 − k 枚正面。
- 桌上原本的 10 枚正面被摸走 k 枚，剩下 10 − k 枚。

兩堆都是 10 − k 枚正面。k 是多少都不影響結果，所以不必看，也不靠運氣。

</details>

## 網頁功能

**題目頁（`index.html`）**

- 開場先列出 100 枚硬幣，蓋住正反後洗牌，再排成 10×10。
- 第一堆要挑幾枚由你決定：點硬幣自己挑、拉桿子，或用 50/50、40/60、電腦隨機分。
- 分堆後可以翻單枚或整堆，再揭曉結果。
- 可以把同一個做法連試 100 次，看是不是真的每次都成立。

**答案頁（`answer.html`）**

- 親手操作正確解法，也可以勾選「蒙上眼睛」。
- 拉桿對照手上和桌上的硬幣。
- 列出摸到 0 到 10 枚正面的 11 種情況，並附真實隨機實驗的次數。
- 改摸其他數量，看兩堆的差距如何固定不變。

---

## The puzzle

There are 100 coins on a table: 10 heads and 90 tails. You are blindfolded and cannot feel which side is up. Split the coins into two groups so that both have exactly the same number of heads.

<details>
<summary>Show the solution (spoiler)</summary>

**Solution:** Take any 10 coins as one group, then flip all 10 of them.

**Why it works:** Suppose you picked up k heads.

- Your hand holds 10 − k tails, which become 10 − k heads after the flip.
- The table started with 10 heads and lost k of them, leaving 10 − k.

Both groups have 10 − k heads. The value of k does not matter, so you never need to look and luck plays no part.

</details>

## Features

**Puzzle page (`index.html`)**

- Opens by laying out all 100 coins, hiding their faces, shuffling them, and arranging them in a 10×10 grid.
- You decide the size of the first group: click coins, drag the slider, or use 50/50, 40/60, or a random computer split.
- After splitting, flip single coins or a whole group, then reveal the result.
- Replay the same strategy 100 times to see whether it really holds every time.

**Answer page (`answer.html`)**

- Walk through the solution by hand, with an optional blindfold.
- Use a slider to compare the coins in your hand with those on the table.
- See all 11 outcomes (0 to 10 heads picked), with counts from real random trials.
- Pick a different number of coins and see the gap between the groups stay fixed.

## 技術說明 / Technical notes

兩個獨立的 HTML 檔案，沒有建置步驟。字型來自 Google Fonts。

Two standalone HTML files with no build step. Fonts come from Google Fonts.

訪客統計使用 GoatCounter（只在 GitHub Pages 上啟用），代碼設定在兩個 HTML 檔開頭的 `GOATCOUNTER`。

Visitor stats use GoatCounter (only enabled on GitHub Pages). The account code is set in `GOATCOUNTER` at the top of both HTML files.

## 版本 / Versions

- **v2：** 第一頁改為只有題目的自由試玩，解說移到答案頁。 / The first page is now a free-play puzzle, and the explanation moved to an answer page.
- **v1：** 單頁解說與模擬。 / A single page with the explanation and simulation.
