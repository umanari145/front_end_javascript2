# front_end_javascript2

## vue.js

JavaScriptのフレームワーク。<br>
jQueryでは簡易的で便利な反面、DOM操作が厳しくなり、HTMLの構造を変えることが難しい。<br>
特にSPA(Single Page Application:単一ページ内でのアプリ)に向いている。

## 基礎サンプル(cdn)
- cnd
  - index.html
  - vue.js

```
JS側
var app = new Vue({
    //vueが有効なHTML要素
    el : '#app',
    //バインドできる変数
    data : {

    },
    //イベントに関連づけられるメソッド
    methods:{

    }
})


HTML側
<!-- vueが入ることのできるスコープ -->
<div id="demo">
    <p>{{message}}</p>
    <input v-model="message">
    <!-- inputのなかにある変数を紐付けできる -->
</div>

<div id="app">
    <li v-for="todo in todos">
        {{todo.text}}
    </li>
    <button v-on:click="showMessage">押してみよう</button>
    <!-- イベントに紐付けることができる -->
</div>
```
