# Homework 5

## 作業名稱

讓網頁變得更完整：加上 placeholder 與 infinite scroll

## 作業說明

瀏覽器載入每一張圖片都需要時間，假如在網路連線速度不太好的情況下，就很有可能發生文字已經顯示出來，但圖片卻還在下載的情形：

![](images/hw5_broken.png)

這樣其實是很破壞使用者體驗的一件事，因為整個網頁看起來就像跑版了一樣。如果要讓使用者體驗變得更好，應該要在圖片載入的時候先放一張佔位圖（placeholder），載入完成之後才顯示真的圖片。

除此之外，光放佔位圖還是不夠的，因為目前 div 的高度是由圖片比例所決定的，所以當圖片還沒載入完成的時候，就會像上圖那樣高度是 0，所以我們可以先把高度寫死，這樣就可以確保載入前的高度就是正確的高度。

再者，現在的內容數量固定是 20 個頻道，可是使用者很有可能還想要看更多的頻道。該怎麼辦呢？一個顯而易見的做法是第一次載入時就載入更多的頻道，例如說 100 個，但是這樣子的話資料量太大，時間可能會太久。

比較好的做法是每當使用者要滑到快到底的時候，就自動載入新的 20 個頻道，只要使用者一直往下捲，內容就會一直出現，這就叫做 infinite scroll，有點像是 Facebook 的動態時報一樣，你可以一直往下滑。

這次的作業就是需要實作這兩項新功能。

## 作業規格

1. 你可以拿我們在第一次作業用的[這張圖](https://static-cdn.jtvnw.net/ttv-static/404_preview-320x180.jpg)當作 placeholder。
2. 必須先出現佔位圖，等圖片載入完成再顯示真的圖片
3. infinite scroll 的部分，可以參考 Twitch API 的 limit 跟 offset 這兩個參數

完成示意圖：

![](http://g.recordit.co/Iqw49b7Uag.gif)

![](http://g.recordit.co/gu4hwKWAMC.gif)

## 作業規範

1. 除了 `jQuery`，不能用其他的 Library


## 學習資源

1. [Check if a user has scrolled to the bottom](http://stackoverflow.com/questions/3898130/check-if-a-user-has-scrolled-to-the-bottom)
2. [onload Event](https://www.w3schools.com/jsref/event_onload.asp)


## 自我練習

1. 佔位圖也是圖片，也需要下載時間，有沒有什麼方法可以優化這點？


## 進階閱讀
1. [实例解析防抖动（Debouncing）和节流阀（Throttling）](http://jinlong.github.io/2016/04/24/Debouncing-and-Throttling-Explained-Through-Examples/)
2. [Debounce and Throttle: a visual explanation](http://drupalmotion.com/article/debounce-and-throttle-visual-explanation)
3. [throttle与debounce的区别](https://segmentfault.com/a/1190000004909376)
4. [The Difference Between Throttling and Debouncing](https://css-tricks.com/the-difference-between-throttling-and-debouncing/)