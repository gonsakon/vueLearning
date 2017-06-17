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

以前用 JS 寫一個 hello world，你會這樣子寫

```js
<!DOCTYPE html>
<html lang="en">
<head></head>
<body>
    <div class="hi"></div>
    <script>
        document.querySelector('h1').textContent ='Hello World！'
    </script>
</body>
</html>
```





