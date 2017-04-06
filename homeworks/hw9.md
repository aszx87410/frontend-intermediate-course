# Homework 9

## 作業名稱

節省 Request 的極致：一為全，全為一

## 作業說明

在前端效能優化裡面，你可以適時地把 Request 數量降低來加快加載速度（但別忘記了，Reuqest 降低有可能代表檔案大小變大，下載速度不一定會比較快）。

當你把這樣的概念發揮到極致，就是把 CSS, JavaScript 全部都用 inline 的方式包在 HTML 裡面，就立刻節省了兩個 Request，但缺點就是網頁的 HTML 會變得很醜就是了。

可是，難道我們要手動來做這件事情嗎？手動的話似乎效率太低了，每一次只要更改內容，就必須手動調整一次，十分耗費精力。如果有一個工具可以幫我們自動化，那真是太好了！

沒錯，那個工具就是 Gulp。

## 作業規格

1. 把 CSS, JavaScript 都 inline 進 `index.html`
2. 不能發出任何 CSS 跟 JavaScript 的 Request

## 作業規範

1. `index.html` 裡面只能引入一個 js 檔案

## 學習資源

1. [可以幫我自動化嗎，拜託：Gulp](http://ithelp.ithome.com.tw/articles/10185976)
2. [Gulp 學習 1 - 安裝與執行](http://www.oxxostudio.tw/articles/201503/gulp-install-webserver.html)
3. [gulp 入门指南](https://github.com/nimojs/gulp-book)
4. [前端构建工具gulp入门教程](https://segmentfault.com/a/1190000000372547)
5. [Gulp 入門教學 - 壓縮 JavaScript 與 CSS](http://abgne.tw/web/gulp/gulp-tuts-compress-js-css.html)

## 自我練習

1. 除了 inline 以外，順便做 minify 吧，就是把檔案的大小縮到最小，去除程式碼中的多餘資訊（註解、空白、換行等等）。

## 進階閱讀

無
