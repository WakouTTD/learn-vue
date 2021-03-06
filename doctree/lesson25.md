# 条件分岐　v-if

## 条件分岐 v-ifを使用すると

- 要素の表示・非表示を切り替える

- 例題

1. p要素を配置

2. 表示 / 非表示切り替え

- v-ifディレクティブでは要素はDOMレベルで削除される点に注意

要素を頻繁に表示、非表示を繰り返す用途の場合、描画コストが高くなる恐れがある
対策としてはcssのdisplayプロパティを利用するv-showディレクティブを使用する

```html
<div id="app">
  <p v-if="toggle">
    Hello
  </p>
</div>

<script>
src＝"https://cdn.jsdelivr.net/npm/vue@2.6.11/dist/vue.js"
</script>
```

```javascript
// Vueインスタンス
var app = new Vue({
  // マウントする要素を指定
  // オプション名:'値'　というハッシュ形式
  el: '#app',
  // プロパティ名:値 という形式　カンマ区切りで複数のプロパティを指定できる
  data: {
   toggle: true
  }
})
```
