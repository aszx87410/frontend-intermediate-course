# Homework 7

## 作業名稱

走向國際：i18n

## 作業說明

i18n 的全名叫做`internationalization`，這個簡寫的由來就是因為 i 跟 n 中間有 18 個字母。

現在很多服務都不只面向單一一個市場，而是會發佈到各個國家去。雖然也可以全部都用英文，但這樣對本地的使用者來說就相對沒有那麼友善。因此，本地化也是很重要的一件事。

在這次的作業當中，我們要試著讓我們的網頁走出國際，多支援一個英文版。

所以呢，要做到兩件事：

1. 可以只抓取某個語言的實況（可參考 Twitch API）
2. 提供按鈕切換語言

完成示意圖：
![](http://g.recordit.co/NC8zbXBlaN.gif)

## 作業規格

雖然這一次作業要翻譯的文字很少，只有頁面的標題而已，但一般網站需要翻譯的文字可多了。因此，會有一個語言檔來負責這件事情。例如說英文的叫做：`lang-en.js`，中文就叫做`lang-zh-tw.js`。

那語言檔的內容是什麼呢？其實就是一個 JavaScript 的 Object 而已：

```
if (!window.I18N) window.I18N = {};
window.I18N['zh-tw'] = {
  TITLE: '用中文直播的頻道'
}
```

在頁面上面引入檔案之後，就可以在要顯示文字的地方用`I18N['zh-tw'].TITLE`來拿到中文的翻譯。

這次作業的規格就是必須要有兩個檔案：`lang-en.js`與`lang-zh-tw.js`，以及利用上述的方式輸出不同語言。

``` html
<script src="lang-en.js"></script>
<script src="lang-zh-tw.js"></script>
<script src="script.js"></script>
```


## 作業規範

1. 放心，你現在可以使用 jQuery 了，但你也可以挑戰繼續使用 vanilla js


## 學習資源

無


## 自我練習

1. 我們在這範例中用了 `window` 儲存 I18N 這個全域變數，這樣有什麼壞處嗎？

## 進階閱讀

1. [moment.js 語言檔](https://github.com/moment/moment/blob/develop/locale/zh-tw.js)
2. [jquery UI 語言檔](https://github.com/jquery/jquery-ui/blob/master/ui/i18n/datepicker-zh-TW.js)
3. [Javascript模块化编程（一）：模块的写法](http://www.ruanyifeng.com/blog/2012/10/javascript_module.html)
4. [从0到1学习node(一)之模块规范](https://www.xiabingbao.com/definition/2017/01/10/mod-definition.html)
5. [JavaScript 模块化七日谈](http://huangxuan.me/js-module-7day)