# ディレクティブとは

- v- で始まる特別な属性のこと

- derective(指令)という名前の通り、何らかの指示を行う仕組みです。

## ディレクティブの例

- v-bind
- v-if
- v-show
- v-for
- v-on
- v-model

## 使用のイメージ

```html
<input type="text" v-bind:value="message" />
```

 v-bindの部分はdomへ反映される前にview.jsによって解釈変換され、
 その後は内部的にのみ利用される。

### DOMとは

#### Document Object Model

- ツリー構造とも呼ばれる階層構造を取る
- それぞれノードという言葉で説明される
- WEBページとJavaScriptなどのプログラミング言語とを繋ぐ

[MDN web docsのDOM の紹介](https://developer.mozilla.org/ja/docs/Web/API/Document_Object_Model/Introduction)
