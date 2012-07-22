---
layout: post
title: "markdown形式でリンクをクリップボードにコピーするchrome-extension作った。"
date: 2012-07-22 17:29
comments: true
categories: chrome-extensions
---

## 作ったもの
> [Chrome Web Store - Markdown Linker](https://chrome.google.com/webstore/detail/kgadgjmlofjccpefhdagbonmohjknlll)


octopressでブログを書くようになって、markdownで文章を書く機会が増えた。
しかしながら画像やリンクをmarkdown形式で挿入するのが若干面倒なので
chrome extensionを作ることにした。作りながら記事を書いてみる


## やりたかったこと
とりあえずやりたいことは以下の3つ

1. ページのタイトルとurlをコピー => `[ title ]( url )`
2. テキストリンクのtextとurlをコピー => `[ text ]( url )`
3. 画像のaltとurlをコピー => `![ alt ]( url )`

このうち、1. はそういう拡張機能がすでにあるようだったが、2,3　は軽く探した限りでは見つからなかった。
ちょっとモチベーションが上がる。


## 名前
まず名前を決めてリポジトリを作る。あまり考えずに、
> chrome-markdown-linker


とした。likerがちょっとニュアンス違うと思うけど、まあいいか。
chrome-markdown-link-copyだとちょっと長いし。


## 準備
extentionはchrome上でもビルドできるが、コンソールからビルドしたいので[Constellation/crxmake](https://github.com/Constellation/crxmake)を入れる。

    gem source -a http://gemcutter.org
    sudo gem install crxmake

githubで使い方を見てRakefileを書いておく

## 資料
> [Google Chrome Extensions - Google Code](http://code.google.com/chrome/extensions/index.html)

ここのGetting Started tutorialとかSamplesとか見ながらやるのが早いと思う。

## 実装
以前[twitterのparmalinkをはてな記法でクリップボードにコピーする拡張](https://chrome.google.com/webstore/detail/fnpppbhohekmekeomhfihapjadolpjjh)を作ったのでそれを参考にする。
ポイントは一度リンクの情報をbackground pageのtextareaに渡して、文字列を選択してからクリップボードにコピーするところ。

> [fukayatsu/chrome-markdown-linker](https://github.com/fukayatsu/chrome-markdown-linker)

とりあえずこんな感じになった。

## TODO
- アイコン作る
- ストアのページを充実させる
- ショートカットキーに対応する