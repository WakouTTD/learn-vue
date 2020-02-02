# Vue.jsの読み込み方法

- CDN
  - Content Delivery Network
  - Web Contentsをインターネット上で配信するために最適化されたネットワーク
  - Vue.jsで利用するのはjsDelivrというオープンソースのCDN
  - 東京と大阪にもエッジロケーション、つまり配信サーバーがあるため、高速
  - 基本的には何かしらの理由がある場合以外は、CDNを使う方が気軽でお薦め
  - [公式](https://jp.vuejs.org/v2/guide/installation.html#CDN)

jsFiddleの左上のhtmlの入力欄に記入

htmlのbodyの終了タグの直前に配置

```html
<script src="https://cdn.jsdelivr.net/npm/vue@2.6.11"></script>
```


- 直接組み込み
  - ファイルをダウンロード

- NPM
  - Node Package Manager(パッケージ管理ソフト)の利用



