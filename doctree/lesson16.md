# ルートのテンプレートとは何か

- テンプレートとは
  - HTMLベースのテンプレート構文を使用した描画部分に関する記述のこと
  - いわゆるMVCやMVVMパターンで言うところのV(View)に相当

jsfiddle

javascript
```javascript
// Vueインスタンス
var app = new Vue({
  // マウントする要素を指定
  // オプション名:値　というハッシュ形式
  el: '#app',
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
    {{ message }}
  </p>
</div>

<script>
src＝"https://cdn.jsdelivr.net/npm/vue@2.6.11/dist/vue.js"
</script>
```

- ルートのテンプレートを作成

- マウントする要素を指定
