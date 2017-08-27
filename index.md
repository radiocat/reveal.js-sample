Reveal.jsとは？

>>>

HTML5で書けるプレゼンツール

>>>

`Markdown` もサポート

----

# 使い方

GitHubから`clone` して `npm`

``` bash
$ git clone https://github.com/hakimel/reveal.js.git 
$ cd reveal.js
$ npm install
$ npm start
```

ブラウザで `http://localhost:8000` を開くとスライドが表示される

>>>

できる事の詳細はコードについてくる [demo](../demo.html) が参考になる

----

# 書き方

コード一式を持ってきて`index.hml` を好きなように編集する

``` html
<div class="reveal">
  <div class="slides">
    <section>Single Horizontal Slide</section>
      <section>Vertical Slide 1</section>
      <section>Vertical Slide 2</section>
    </section>
  </div>
</div>
```

※公式のREADMEより引用

>>>

## Markdownの書き方

- `<textarea>` を使う
- `*.md` の外部ファイルを参照させる

``` html
<section data-markdown="example.md"
  data-separator="^¥\n\n\n"  
  data-separator-vertical="^\n\n"  
  data-separator-notes="^Note :"  
  data-charset="iso-8859-15">
</section>
```

※公式のREADMEより引用

>>>

例）Qiitaっぽく `----` でページを区切る場合

```html
<section data-markdown="index.md"
  data-separator="^\n----\n$">
</section>
```


----

## その他の表現方法

fragment表示

```html
- Item 1 <!-- .element: class="fragment" data-fragment-index="1" -->
- Item 2 <!-- .element: class="fragment" data-fragment-index="2" -->
```

- Item 1 <!-- .element: class="fragment" data-fragment-index="1" -->
- Item 2 <!-- .element: class="fragment" data-fragment-index="2" -->


>>>

<!-- .slide: data-background="#0000ff" -->
色を変える

```html
<!-- .slide: data-background="#0000ff" -->
```


>>>

もっとこだわりたい場合はHTML5やCSSを使う

※詳細は公式のREADME参照

https://github.com/hakimel/reveal.js

----

# おまけ

[PDFにエクスポート](/?print-pdf#/)

上記にアクセスしてブラウザの印刷機能でPDFに保存する（Chromeの場合）

※オプションで「背景のグラフィック」にチェックを入れる

----

# END

サンプルコード：https://github.com/radiocat/reveal.js-sample


----

# REFERENCES

- [reveal.js（公式）](https://github.com/hakimel/reveal.js)
- [Reveal.js、Markdown、Githubでスライドを作成する。（Qiita）](http://qiita.com/budougumi0617/items/19b19019bbe01f86e251)
- [reveal.jsでスライド作り。（Qiita）](http://qiita.com/t-kusakabe/items/725e7438892bba395062)


