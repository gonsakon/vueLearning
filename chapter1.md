# 第一章 Vue.js 簡介

相信你來到這裡，表示你對 HTML、CSS、JS 有一定的基礎，若要介紹 Vue.js ，其實在[官網](https://vuejs.org/v2/guide/)已經有詳細的介紹，對英文不擅長也可瀏覽[簡中](https://cn.vuejs.org/v2/guide/)版本，在 chrome 瀏覽器點選右鍵，便能即時翻譯成繁中版。

## 在網頁上載入 Vue.js

筆者在撰寫此文件時，Vue.js 已更新到 `2.3.4`，  
安裝方式在[官網](https://vuejs.org/v2/guide/installation.html)寫得很清楚，  
若你想要下載 Vue.js，可點選下方官網推薦 CDN 另存下載在自己本機即可，  
建議同步安裝 chrome 除錯插件。

* [CDN 下載](https://unpkg.com/vue)
* [Vue.js devtools](https://chrome.google.com/webstore/detail/vuejs-devtools/nhdogjmejiglipccpnnnanhbledajbpd)

## 使用 Vue.js 寫 Hello world 吧！

以前用 JS 寫一個 hello world，其中一個寫法會像是下面程式碼，  
選取 DOM 元素後，再用 textContent 插入文字。  
[JSBIN 範例程式碼：](http://jsbin.com/sutozoboge/edit?html,console,output)

```js
<!DOCTYPE html>
<html lang="en">
<head></head>
<body>
<div class="hi"></div>
<script>
document.querySelector('.hi').textContent ='Hello World！';
</script>
</body>
</html>
```

那假使是 Vue.js 呢？  
每個框架都會有它的規則，以下面程式碼為例：

* 新增一個`new Vue()`
* `el` 是要綁定的 DOM 元素，讓 DOM 裡面的作用域都可使用 Vue.js
* `{{ 'Hello World' }}` 兩個大刮號是 Vue.js 渲染內容的格式，裡面帶了字串 `'Hello World'` 便可直接呈現在網頁上

[JSBIN範例程式碼](http://jsbin.com/yolanumova/1/edit)

```js
<!DOCTYPE html>
<html lang="en">
<head>
    <script src="https://unpkg.com/vue"></script>
</head>
<body>
    <div id="app">
        <div class="hi">{{'Hello World！'}}</div>
    </div>
    <script>
        var app = new Vue({ el: '#app' })
    </script>
</body>

</html>
```



