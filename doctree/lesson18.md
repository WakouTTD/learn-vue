# dataオプションにオブジェクトや配列要素を設定

jsfiddle

javascript

```javascript
// Vueインスタンス
var app = new Vue({
  // マウントする要素を指定
  // オプション名:'値'　というハッシュ形式
  el: '#app',
  // プロパティ名:値 という形式　カンマ区切りで複数のプロパティを指定できる
  data: {
    message: 'Hello Vue.js!',
    count: 110,
    user: {
      lastName: 'Yamada',
      firstName: 'Taro',
      prefecture: 'Tokyo'
    },
    colors: ['Red','Green','Blue']
  }
})
```

html

```html
<!-- この部分をテンプレートと言う。 `app`をセレクターと言う -->
<div id="app">
  <!--
  <p>
    <input type="text" v-model="message">
  </p>
  -->
  <p>
    <!-- テンプレートの中にブレイス2つでプロパティ名を記述してバインディング -->
    {{ message }}
  </p>
  <p>
    {{ count }}
  </p>
  <p>
    {{ user.prefecture }}
  </p>
  <p>
    {{ colors[1] }}
  </p>
</div>

<script>
src＝"https://cdn.jsdelivr.net/npm/vue@2.6.11/dist/vue.js"
</script>
```
