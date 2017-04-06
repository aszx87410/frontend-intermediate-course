# Homework 8

## 作業名稱

當我們包在一起：Webpack

## 作業說明

在上一次的作業裡面，我們將 i18n 需要的翻譯檔分開，每一個語言就是一個檔案，藉此讓各個語言的翻譯者只需要關注自己那份檔案即可。可是，你會發現有一個地方有點不太好，那就是我們使用全域變數來進行模組之間的溝通及引入。

我們直接在 `windows` 上面加了一個叫做 `i18n` 的物件，並且利用這個物件來當作翻譯的資源。那如果我們今天使用了別的 library，它也使用了同名的 i18n 這個物件怎麼辦？這兩個不就衝突了嗎？

因此，利用全域變數顯然不是一個解決問題的好方法。

如果你有寫過其他程式語言，例如說 ruby, python，你要用別人提供好的 library 你都會怎麼用？應該就是在程式開頭加上`import library`之類的語句，就可以直接開始使用了。

那如果寫 JavaScript 的時候也能這樣，不就太棒了嗎？

沒錯，於是 Webpack 就來幫你完成這個夢想了。

## 作業規格

1. 使用 Webpack，把 jQuery 以及其他 js 檔案都打包成一個`bundle.js`

## 作業規範

1. `index.html` 裡面只能引入一個 js 檔案

## 學習資源

1. [一看就懂的 React 開發環境建置與 Webpack 入門教學](http://blog.techbridge.cc/2016/07/30/react-dev-enviroment-webpack-browserify/)
2. [我也想要模組化開發：Webpack](http://ithelp.ithome.com.tw/articles/10188007)
2. [【webpack】的基本工作流程](https://medium.com/html-test/webpack-%E7%9A%84%E5%9F%BA%E6%9C%AC%E5%B7%A5%E4%BD%9C%E6%B5%81%E7%A8%8B-585f2bc952b9)
3. [WEBPACK入門教學筆記](http://blog.kkbruce.net/2015/10/webpack.html#.WN0gRRKGN8w)
4. [一小时包教会 —— webpack 入门指南](http://www.cnblogs.com/vajoy/p/4650467.html)
5. [入门Webpack，看这篇就够了](http://www.jianshu.com/p/42e11515c10f)


## 自我練習

1. webpack 可以把 CSS 也當作 library 那樣引入，你可以試試看
2. webpack 提供了很猛的 [Hot Module Replacement (HMR)](https://github.com/webpack/docs/wiki/hot-module-replacement-with-webpack)，試試看吧！

## 進階閱讀

1. [玩转webpack 深入理解原理](http://www.thkdog.com/html5/2015/05/08/webpack.html)
2. [打包原理](https://www.kancloud.cn/xiak/quanduan/254501)
3. [【翻译】Webpack——令人困惑的地方](https://github.com/chemdemo/chemdemo.github.io/issues/13)


