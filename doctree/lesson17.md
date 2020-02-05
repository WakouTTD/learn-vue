# テキストのデータバインディング

画面にHello Vue.jsと表示するプログラムをテキストのデータバインディングにより実装する

まず表示するテキストのデータを定義

DOMの更新を自動化するデータバインディングを行うためにはテンプレートで使用する全てのデータは
リアクティブデータとして定義する必要がある

## リアクティブとは

- 各要素を繫げて反応的に変化させること


jsfiddle

javascript
```javascript
// Vueインスタンス
var app = new Vue({
  // マウントする要素を指定
  // オプション名:'値'　というハッシュ形式
  el: '#app',
  // プロパティ名:値 という形式
  data: {
    message: 'Hello Vue.js!'
  }
})
```

html
```html
<!-- この部分をテンプレートと言う。 `app`をセレクターと言う -->
<div id="app">
  <p>
    <input type="text" v-model="message">
  </p>
  <p>
    <!-- テンプレートの中にブレイス2つでプロパティ名を記述してバインディング -->
    {{ message }}
  </p>
</div>

<script>
src＝"https://cdn.jsdelivr.net/npm/vue@2.6.11/dist/vue.js"
</script>
```

ブレイス2つの記述--Mustache構文という--を利用したテキスト展開
(マスタッシュ・口ひげ)
