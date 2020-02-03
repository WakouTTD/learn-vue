# データバインディングとは

- データと描画を同期する仕組み

jsfiddle

javascript
```javascript
var app = new Vue({
  el: '#app',
  data: {
    message: 'Hello Vue.js!'
  }
})
```

html
```html
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

## データバインディングの種類

- 双方向バインディング (TwoWay)
- 単方向バインディング (OneWay)
- ワンタイムバインディング(OneTime)
