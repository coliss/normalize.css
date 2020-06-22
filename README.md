# normalize.css

<a href="https://github.com/necolas/normalize.css"><img
  src="https://necolas.github.io/normalize.css/logo.svg" alt="Normalize Logo"
  width="80" height="80" align="right"></a>

> CSSリセットに代わるモダンな方法

[![npm][npm-image]][npm-url] [![license][license-image]][license-url]
[![changelog][changelog-image]][changelog-url]
[![gitter][gitter-image]][gitter-url]


**NPM**

```sh
npm install --save normalize.css
```

**CDN**

See https://yarnpkg.com/en/package/normalize.css

**Download**

See https://necolas.github.io/normalize.css/latest/normalize.css


## これは何をするの？

* 多くのCSSリセットとは異なり、有用なデフォルトを保持します。
* さまざまな要素のスタイルを正規化（normalize）します。
* バグや一般的なブラウザの不整合を修正します。
* 精緻な修正で使い勝手を向上させます。
* コメントで、コードが何をするのかを説明しています。


## サポートするブラウザ

* Chrome
* Edge
* Firefox ESR+
* Internet Explorer 10+
* Safari 8+
* Opera


## 拡張されたディテールと既知の問題

normalize.cssの難しい部分の詳細と解説を追加しました。

#### `pre, code, kbd, samp`

`font-family: monospace, monospace`は、フォーマット済みテキストのフォントサイズの継承とスケーリングを修正します。
`monospace`の重複は意図的なものです。
[出典](https://en.wikipedia.org/wiki/User:Davidgothberg/Test59).

#### `sub, sup`

通常、`sub`や`sup`を使用すると、すべてのブラウザでテキストの行ボックスの高さに影響を与えます。
[出典](https://gist.github.com/413930).

#### `select`

デフォルトで、OS XのChromeとOS XのSafariでborderプロパティが定義されていない限り、`select`のスタイル定義が非常に制限されます。
OS XのChromeとOS XのSafariで、`optgroup`要素のデフォルトのフォントのウェイトは安全に変更できません。

#### `[type="checkbox"]`

Firefoxの実装では、box-sizing, padding, widthを考慮していないため、チェックボックスとラジオボタンのスタイルを定義しないことをお勧めします。

#### `[type="number"]`

数値入力に適用されるフォントサイズの値によっては、カーソルのスタイルが`default`から`text`に変更されることがあります。

#### `[type="search"]`

デフォルトで、検索の入力欄は完全にスタイル可能ではありません。OS X/iOSのChromeとSafariでは、`font`, `padding`, `border`, `background`をコントロールできません。また、WindowsのChromeでは、`border`をコントロールできません。`border-width`は適用されますが、ボーダーの外側1px分のボーダーカラー（コントロールできません）しか表示されません。
`-webkit-appearance: textfield`を適用することで、検索の入力欄の利点（過去の検索結果を表示するなど）を損なうことなく、これらの問題を解決できます。

## その他のCSSリセット・ノーマライズ
[モダンブラウザに適したCSSリセットのまとめ](https://coliss.com/articles/build-websites/operation/css/css-reset-for-modern-browser.html)

## 貢献

投稿に関わるすべての人が簡単かつ効果的に投稿できるよう、[contribution guidelines](CONTRIBUTING.md)をご覧ください。


[changelog-image]: https://img.shields.io/badge/changelog-md-blue.svg?style=flat-square
[changelog-url]: CHANGELOG.md
[license-image]: https://img.shields.io/npm/l/normalize.css.svg?style=flat-square
[license-url]: LICENSE.md
[npm-image]: https://img.shields.io/npm/v/normalize.css.svg?style=flat-square
[npm-url]: https://www.npmjs.com/package/normalize.css
[gitter-image]: https://img.shields.io/badge/chat-gitter-blue.svg?style=flat-square
[gitter-url]: https://gitter.im/necolas/normalize.css
