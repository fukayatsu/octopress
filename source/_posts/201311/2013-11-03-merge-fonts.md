---
layout: post
title: "半角:全角==1:2な等幅フォントを作る"
date: 2013-11-03 02:13
comments: true
external-url:
categories:
---

普段プログラミングする時は[Sublime Text 3](http://www.sublimetext.com/3)と[Source Code Pro](http://sourceforge.jp/projects/sfnet_sourcecodepro.adobe/)を使っているのだけれど、半角:全角の文字幅が1:2じゃなくて気になる時があった。

ちょっと無理矢理な例だけど、こんな感じ:
![](https://photos-3.dropbox.com/t/0/AADiNZK_LiJD2_M0TXMRxVv5mlPtTQX2qMbvch8txpwN9A/12/85825/png/2048x1536/3/1383418800/0/2/Screenshot%202013-11-03%2002.07.56.png/1WBSByeieM1FF0IeVHVnxf1LBxkd71dBIeM7uDKfvIA)

- 半角スペースが全角文字の半分の幅じゃないので`=>`が揃わない。もやっとする


## [Source Code Pro](http://sourceforge.jp/projects/sfnet_sourcecodepro.adobe/) と [MigMix 1M](http://mix-mplus-ipa.sourceforge.jp/migmix/#diff_migmix1p_migmix2p)の合成

ベース: [MasayukiFukada/CodeMFont](https://github.com/MasayukiFukada/CodeMFont)

#### ベースからの変更点
- Source Code Proの中間フォントに`Scale(70)`を適用
- 記号をあまり改変しないように変更。全角スペースの可視化は残した

![](https://photos-4.dropbox.com/t/0/AAD0Ce1z2kn40M8UpH01nkwP-ysqc1hCKeqXUfEk4CmuHg/12/85825/png/1024x768/3/1383418800/0/2/Screenshot%202013-11-03%2002.08.37.png/qto5DmwG8lwZPzjXJOtcBJLThC4eMaWKH1lKXBnWnaM)

- Hashのkeyに日本語が入っていても、もやっとしなくなった。
- 半角文字が思ったより横に圧縮されたけど、ちょっと使ってたら慣れた

## Tips
Macではフォントを削除→再生成→再インストールしてもキャッシュを消さないと反映されなかった。

キャッシュ削除コマンド: `$ atsutil databases -removeUser`

## TODO
- generator公開
    - 素材用のフォントを自動的にダウンロードしてフォント生成するやつを作りたい

