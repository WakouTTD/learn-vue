# 属性のデータバインディング v-bind

## 例題

- テキストの入力欄に"HelloVue.js"と表示

- 補足:dataオプションに指定したデータをデータバインディングする

下記のようにvalueのダブルクォート内にマスタッシュ構文を使いたくなるが、
属性にマスタッシュ構文を使うことはできない

マスタッシュ構文はテキストコンテンツのための記法であるため、属性には使用できない

属性へのデータバインディングへはvデータバインディングを使用する。

- ダメな例

```html
<input type="text" name="name" size="30" maxlength="20" value="{{ message }}"/>
```

- 正しい例

```html
<input type="text" name="name" size="30" maxlength="20" v-bind:value="message"/>
```

属性へのバインディングは、マスタッシュ構文ではなくて、v-bindディレクティブを使用する。

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
