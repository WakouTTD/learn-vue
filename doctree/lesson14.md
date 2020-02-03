# Vueのインスタンス作成

jsfiddle

javascript
```javascript
<script>
src＝”https://cdn.jsdelivr.net/npm/vue@2.6.11/dist/vue.js”
</script>
```

html
```html
var app = new Vue({})
```
上記の`Vue`をルートVueインスタンスと呼ぶ
上記のままでは空のVueインスタンス

変数名は慣例としてappやvm
vmは、view model
vue.jsはmvvmパターンと厳密には関連が無いが、部分的には
影響を受けている

このように変数化してコンソールからアクセスできる
