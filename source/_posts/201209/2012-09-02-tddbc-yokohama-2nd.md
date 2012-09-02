---
layout: post
title: "TDDBC横浜 Second Seasonに参加しました"
date: 2012-09-02 20:47
comments: true
categories:
---

9/1に行われた
[TDDBC横浜 Second Season](http://devtesting.jp/tddbc/?TDDBC%E6%A8%AA%E6%B5%9C2nd)
にRuby/RSpecで参加してきました。

![案内](http://img.viame-cdn.com/photos/2040f4c0-d5fc-012f-30a9-123139171a21/r600x600.jpg)

[2012/09/01 TDD Boot Camp 横浜 Second Season #tddbc - Togetter](http://togetter.com/li/360406)

# 参加の経緯
[TDD Boot Camp 福岡 2 #tddbc - Togetter](http://togetter.com/li/219441)に参加してた@dekokunとかが楽しそうだったので前々から気になってはいた。
<blockquote class="twitter-tweet" lang="ja"><p>和田さんと一緒にペアプログラミングとか嬉しすぎる！！！！やばい！！！萌えーーーーー！！！！！ <a href="https://twitter.com/search/?q=%23tddbc"><s>#</s><b>tddbc</b></a></p>&mdash; でこくんさん (@dekokun) <a href="https://twitter.com/dekokun/status/140302052680155136" data-datetime="2011-11-26T05:33:10+00:00">11月 26, 2011</a></blockquote>

それでもしばらく参加しようとしてなかったのは、  
仕事が忙しいことを言い訳にしてたのか、ペアプロすることに自信がなかったのか。  
あるいは、TDDに対してそれほど本気でなかったのかもしれない。

ともかく、先日参加した[#scmbc tokyo 3](/blog/2012/07/21/scmbc-tokyo-3/)でTDDBCの紹介があり、  
今回は自然な流れで参加することができた。

※ 募集が始まった時tddbcで一緒のテーブルだった@STAR_ZEROさんが素早く教えてくれたので、  
最初の抽選では漏れてしまったけど、繰り上がりで参加できた。  
マジでありがとうございました。

# 準備した環境
最初は今仕事で使っているPHPで申し込んだのだけど、先の事を考えてRuby / RSpecに切り替えました。

> [PHP のテストを Ruby で書く « blog.udzura.jp](http://blog.udzura.jp/2011/08/09/writing-php-test-by-ruby/)

こんなのもあるし :)

- Macbook Pro('15), mountailn lion, US配列
- Terminal + zsh
- Git
- Sublime Text 2 (Vintage Mode)
- Ruby 1.9 + RSpec 2 + autotest
- Google IME + KeyRemap4Macbook(左右コマンドキーワンショットを無変換・変換に)

> [autotest · rspec/rspec Wiki](https://github.com/rspec/rspec/wiki/autotest)

最初にペアを組んだ方が全くといっていいほど同じ環境だったので非常にスムーズだった。  
違ったのはIMEの切り替え方法ぐらい。

# Java / JUnit のTDDデモを見ながらRSpecで追いかけてみた
<div class="thumbnail"><a href="https://skitch.com/fukayatsu/etrm9/screen-shot-2012-09-01-at-12.02.45"><img style="max-width:638px" src="https://img.skitch.com/20120902-dukne6mn6tg7m5958yswbi54md.medium.jpg" alt="Screen Shot 2012-09-01 at 12.02.45" /></a></div>
デモペアプロを見ながらこんな感じでやってたら、即座に@t_wadaさんにcontext使って構造化しようとか、letじゃなくてsubject使うといいよとかアドバイスを頂いた(言い訳するとcontext前者はJUnitの書き方に引きずられた感...orz)。実際に修正してもらうときにvimプラグインを有効にしてたら、「宗教上の理由でVimは使えないんですよ...」とおっしゃってたのが印象的だったw

RSpecのよりよい書き方は[RSpec](http://kerryb.github.com/iprug-rspec-presentation/#1)というプレゼンとか
<iframe src="http://rcm-jp.amazon.co.jp/e/cm?lt1=_blank&bc1=000000&IS2=1&bg1=FFFFFF&fc1=000000&lc1=0000FF&t=atsfky-22&o=9&p=8&l=as4&m=amazon&f=ifr&ref=ss_til&asins=4798121932" style="width:120px;height:240px;" scrolling="no" marginwidth="0" marginheight="0" frameborder="0"></iframe>
とかで勉強していきます。

# 弁当
同じテーブルの人たちでポジションペーパーを見ながら、今どんなことやってるとかを話しながらお弁当食べた。  
「TDDいいと思うしやりたいと思うけど、なかなかできないよねー」とかとか。

# ペアプロ
2回め終了時のコードがこちら: 
[fukayatsu/tddbc-vending-machine](https://github.com/fukayatsu/tddbc-vending-machine)

改めて見るとコミットタイミングが微妙だし、TDDのサイクルも適当になってしまっている。  
チートシート見るとかとか、TDD本を写経して改善したい。

楽しかったが、かなりハードだった。毎日ペアプロしてる人はすごいなー

# イベント中にポチったものとか
↓ ほんたったは自宅用と会社用に複数
<iframe src="http://rcm-jp.amazon.co.jp/e/cm?lt1=_blank&bc1=000000&IS2=1&nou=1&bg1=FFFFFF&fc1=000000&lc1=0000FF&t=atsfky-22&o=9&p=8&l=as4&m=amazon&f=ifr&ref=ss_til&asins=B001RTG88Q" style="width:120px;height:240px;" scrolling="no" marginwidth="0" marginheight="0" frameborder="0"></iframe>
<iframe src="http://rcm-jp.amazon.co.jp/e/cm?lt1=_blank&bc1=000000&IS2=1&nou=1&bg1=FFFFFF&fc1=000000&lc1=0000FF&t=atsfky-22&o=9&p=8&l=as4&m=amazon&f=ifr&ref=ss_til&asins=4894717115" style="width:120px;height:240px;" scrolling="no" marginwidth="0" marginheight="0" frameborder="0"></iframe>
<iframe src="http://rcm-jp.amazon.co.jp/e/cm?lt1=_blank&bc1=000000&IS2=1&nou=1&bg1=FFFFFF&fc1=000000&lc1=0000FF&t=atsfky-22&o=9&p=8&l=as4&m=amazon&f=ifr&ref=ss_til&asins=4798116831" style="width:120px;height:240px;" scrolling="no" marginwidth="0" marginheight="0" frameborder="0"></iframe>


↓ こっちじゃんけんで買って頂いたもの


<a href="http://www.amazon.co.jp/gp/product/0131495054/ref=as_li_ss_il?ie=UTF8&camp=247&creative=7399&creativeASIN=0131495054&linkCode=as2&tag=atsfky-22"><img border="0" src="http://ws.assoc-amazon.jp/widgets/q?_encoding=UTF8&ASIN=0131495054&Format=_SL110_&ID=AsinImage&MarketPlace=JP&ServiceVersion=20070822&WS=1&tag=atsfky-22" ></a><img src="http://www.assoc-amazon.jp/e/ir?t=atsfky-22&l=as2&o=9&a=0131495054" width="1" height="1" border="0" alt="" style="border:none !important; margin:0px !important;" />

<a href="http://www.amazon.co.jp/gp/product/0131495054/ref=as_li_ss_tl?ie=UTF8&camp=247&creative=7399&creativeASIN=0131495054&linkCode=as2&tag=atsfky-22">xUnit Test Patterns: Refactoring Test Code (Addison-Wesley Signature Series (Fowler))</a><img src="http://www.assoc-amazon.jp/e/ir?t=atsfky-22&l=as2&o=9&a=0131495054" width="1" height="1" border="0" alt="" style="border:none !important; margin:0px !important;" />




# Tweetsを一部抜粋
<blockquote class="twitter-tweet" lang="ja"><p>技術書の「写経」の方法。 1.ローカルで使える SCM を用意 2.「ほんたった」などで対象の本を固定 3.ひたすらサンプルコードを写して実行 4.実行するたびにコミット(コミットログにページ番号を含める) 5.疑問点があったらコミットログや本に書き込む 6.章ごとにタグを打つ</p>&mdash; Takuto Wadaさん (@t_wada) <a href="https://twitter.com/t_wada/status/9000231741" data-datetime="2010-02-12T08:06:50+00:00">2月 12, 2010</a></blockquote>

<blockquote class="twitter-tweet" lang="ja"><p>ある程度、やることリストを書いておいたほうがいい。一歩一歩進んでいて、どこにいっているのかわからなくなくなるために。<a href="https://twitter.com/search/?q=%23tddbc"><s>#</s><b>tddbc</b></a></p>&mdash; Yotaro TAKAHASHI さん (@PoohSunny) <a href="https://twitter.com/PoohSunny/status/241718475725357057" data-datetime="2012-09-01T02:05:50+00:00">9月 1, 2012</a></blockquote>

<blockquote class="twitter-tweet" lang="ja"><p><a href="https://twitter.com/search/?q=%23tddbc"><s>#</s><b>tddbc</b></a> テスト駆動開発のコツ：一番単純なところから探す。何もしないときにどうなるか。</p>&mdash; しんやさん (@shinyaa31) <a href="https://twitter.com/shinyaa31/status/241720222619430912" data-datetime="2012-09-01T02:12:46+00:00">9月 1, 2012</a></blockquote>

<blockquote class="twitter-tweet" lang="ja"><p>和田さん：『チャレンジしてもらいたいのは"ゴールから書く"。何を達成すればゴールになるのかを考えながら。』 <a href="https://twitter.com/search/?q=%23tddbc"><s>#</s><b>tddbc</b></a></p>&mdash; しんやさん (@shinyaa31) <a href="https://twitter.com/shinyaa31/status/241720701436956672" data-datetime="2012-09-01T02:14:40+00:00">9月 1, 2012</a></blockquote>
↑ 例えば、asertから書くとか

<blockquote class="twitter-tweet" lang="ja"><p>何かやる時は1回目は普通に書いて、2回目で匂いを感じて、3回目が発生したら重複をまとめるという感じが、良く言われるタイミングかな。 <a href="https://twitter.com/search/?q=%23tddbc"><s>#</s><b>tddbc</b></a></p>&mdash; Tomohiro Hashidateさん (@joker1007) <a href="https://twitter.com/joker1007/status/241726133018701824" data-datetime="2012-09-01T02:36:15+00:00">9月 1, 2012</a></blockquote>
↑ 2回目、場合によってはコメントでTODO書いたりするんだろうと思う

<blockquote class="twitter-tweet" lang="ja"><p>仮実装でテストがグリーンになったらコミット。リファクタリングしてグリーンになったらコミット。 <a href="https://twitter.com/search/?q=%23tddbc"><s>#</s><b>tddbc</b></a></p>&mdash; 「原発が無くても安心の社会」に一票さん (@aetos382) <a href="https://twitter.com/aetos382/status/241727204243939328" data-datetime="2012-09-01T02:40:31+00:00">9月 1, 2012</a></blockquote>
↑ 最後のQAで手動コミットはオワコンという指摘もｗ

<blockquote class="twitter-tweet" lang="ja"><p>デフォルトのgitkは見づらいですね。Macな人はSourceTreeおすすめ <a href="https://twitter.com/search/?q=%23tddbc"><s>#</s><b>tddbc</b></a></p>&mdash; sue445さん (@sue445) <a href="https://twitter.com/sue445/status/241733156779208704" data-datetime="2012-09-01T03:04:10+00:00">9月 1, 2012</a></blockquote>

<blockquote class="twitter-tweet" lang="ja"><p>クリーンコードのボブマーチンですらテストファーストが辛くなる→自分を戒めるためのグリーンバンド <a href="https://twitter.com/search/?q=%23tddbc"><s>#</s><b>tddbc</b></a></p>&mdash; sue445さん (@sue445) <a href="https://twitter.com/sue445/status/241734176431284224" data-datetime="2012-09-01T03:08:13+00:00">9月 1, 2012</a></blockquote>
↓ 昼休みに購入  
![グリーンバンド](http://img.viame-cdn.com/photos/93b13440-d614-012f-0f92-123139183adb/r600x600.jpg)

<blockquote class="twitter-tweet" lang="ja"><p>目標としては一つのテストメソッドで一つのアサーション <a href="https://twitter.com/search/?q=%23tddbc"><s>#</s><b>tddbc</b></a></p>&mdash; すたぜろ（けん）さん (@STAR_ZERO) <a href="https://twitter.com/STAR_ZERO/status/241765792880943104" data-datetime="2012-09-01T05:13:51+00:00">9月 1, 2012</a></blockquote>

<blockquote class="twitter-tweet" lang="ja"><p>（何が失敗しているかわからない）グレー(表示上はレッド)はレッドより避けたい <a href="https://twitter.com/search/?q=%23tddbc"><s>#</s><b>tddbc</b></a></p>&mdash; Atsuo Fukayaさん (@fukayatsu) <a href="https://twitter.com/fukayatsu/status/241766446164762624" data-datetime="2012-09-01T05:16:27+00:00">9月 1, 2012</a></blockquote>

<blockquote class="twitter-tweet" lang="ja"><p>it "hogehoge"を列挙してから、それぞれを記述していくのもありなのかー <a href="https://twitter.com/search/?q=%23tddbc"><s>#</s><b>tddbc</b></a></p>&mdash; Atsuo Fukayaさん (@fukayatsu) <a href="https://twitter.com/fukayatsu/status/241826957468246018" data-datetime="2012-09-01T09:16:54+00:00">9月 1, 2012</a></blockquote>

<blockquote class="twitter-tweet" lang="ja"><p>ピサ！今日の懇親会！ <a href="https://twitter.com/search/?q=%23tddbc"><s>#</s><b>tddbc</b></a><a href="http://t.co/29YYJYEs" title="http://instagr.am/p/PB3FXtv23H/">instagr.am/p/PB3FXtv23H/</a></p>&mdash; ずきゅ～んたんさん (@ZuQ9Nn) <a href="https://twitter.com/ZuQ9Nn/status/241842472752386048" data-datetime="2012-09-01T10:18:33+00:00">9月 1, 2012</a></blockquote>
気のせいか、いつもの勉強会のピザより美味しかった

<blockquote class="twitter-tweet" lang="ja"><p><a href="https://twitter.com/search/?q=%23tddbc"><s>#</s><b>tddbc</b></a> 横浜道場道場主『いやぁ、見積り難しいね！』(※おっぱいアプリのプランニングポーカーでのお話です)</p>&mdash; しんやさん (@shinyaa31) <a href="https://twitter.com/shinyaa31/status/241867270639464449" data-datetime="2012-09-01T11:57:05+00:00">9月 1, 2012</a></blockquote>
↑ 相対見積りが大事、というのを実感できたｗ

<blockquote class="twitter-tweet" lang="ja"><p><a href="https://twitter.com/search/?q=%23tddbc"><s>#</s><b>tddbc</b></a> 一発で決まった！w <a href="http://t.co/6Sil27PR" title="http://yfrog.com/kgc6ojyj">yfrog.com/kgc6ojyj</a></p>&mdash; しんやさん (@shinyaa31) <a href="https://twitter.com/shinyaa31/status/241877105598689280" data-datetime="2012-09-01T12:36:10+00:00">9月 1, 2012</a></blockquote>
じゃんけんとは言え、人から本を貰うというのは重いものだな、と思った。  

<blockquote class="twitter-tweet" lang="ja"><p><a href="https://twitter.com/search/?q=%23tddbc"><s>#</s><b>tddbc</b></a> で、いただいた本について書評を書いてブログに載せるというミッションが・・・。</p>&mdash; たのっち@XP祭りの仕込み中さん (@dproject21) <a href="https://twitter.com/dproject21/status/241879837235613697" data-datetime="2012-09-01T12:47:01+00:00">9月 1, 2012</a></blockquote>
800ページ超...。

<blockquote class="twitter-tweet" lang="ja"><p><a href="https://twitter.com/search/?q=%23tddbc"><s>#</s><b>tddbc</b></a> 横浜 Second Season の記念写真です。 <a href="http://t.co/s4rAnSwg" title="http://twitpic.com/aq6nzl">twitpic.com/aq6nzl</a></p>&mdash; せとあずさ♂さん (@setoazusa) <a href="https://twitter.com/setoazusa/status/242091049806356480" data-datetime="2012-09-02T02:46:18+00:00">9月 2, 2012</a></blockquote>


<script src="//platform.twitter.com/widgets.js" charset="utf-8"></script>

# おわりに
会場を提供していただいた、[株式会社アットウェア](http://www.atware.co.jp)さん、  
スタッフの皆さん、  
一緒にペアプロをしていただいた皆さん、  
本当にありがとうございました！！

引き続きTDDを自分のものにするのと、頂いた本をなんとかするのを頑張ります！
