# Vue.jsの本番バージョンと開発バージョン

- 開発
  - 警告出力、デバッグモード

- 本番
  - スピード


開発
```javascript
<script>
src＝”https://cdn.jsdelivr.net/npm/vue@2.6.11/dist/vue.js”
</script>
```

本番 (違いは`min`)
```javascript
<script>
src＝”https://cdn.jsdelivr.net/npm/vue@2.6.11/dist/vue.min.js”
</script>
```
- `min`はminify、つまりファイル圧縮を意味する
- それぞれのsrcのurlをブラウザのurl欄にそのまま貼れば、それぞれのソースが見れる。
