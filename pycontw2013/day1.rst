=======
 Day 1
=======

ホテル(台北市内)から会場へ
==========================
宿泊した台北市内の `ホテル <http://www.fortunehiyahotel.com/main/getLanguage/jp>`_ から会場となる
`Academia Sinica <http://www.sinica.edu.tw/main_e.shtml>`_ への移動は、公共交通機関だと MRT(地下鉄)とバスを乗り継がないといけないので多少不便です。

朝早くの移動ということもあり、私たちはタクシーで移動しました。だいたい30分くらいで会場に到着します。料金は330TWDです。タクシーの運転手さんはあんまり英語が通じる感じではないので、行き先の名前(漢字のもの)を紙で見せるのが通じやすいようです。

会場に到着したら、まずは今日の宿泊先となる
`Activity Center <http://proj3.sinica.edu.tw/~gao/huo-dong/room-online-en.php>`_ に荷物を預けて、身軽になってからカンファレンス会場に移動しました。

受付
====
清水川です。

カンファレンスの受付には開始10分前の9時に到着したのですが、さすがに開始直前と言うこともあり、ほとんどの人は受付を済ませてホール内に入っていたようです。

.. figure:: /_static/checkin.jpg
   :width: 400

   受付の様子

受付は受付番号順に100番区切りでレーンが分かれており、非常にスムーズでした。受付番号自体も開催2日前にリマインダーメールが届いていたので、今年は受付での混乱は少なかっただろうと感じました。私自身はスピーカーレーンがあることに気づかず一般の方に並んでしまったので多少手間取りましたが…。そういえば昨年のPyCon JPでもスピーカー受付はわかりにくかったようで、このあたりは共通の課題ですね。

.. figure:: /_static/novelty.jpg
   :width: 400

   名札、紙袋、Tシャツ、朝食

受付後、名札の他にノベルティーとして、紙袋、Tシャツ、プログラム、朝食をもらいました。名札は厚紙に名前を印字したものをストラップのクリップでぶら下げるだけのシンプルなもので、こういうのを見るとPyCon JPでも名札ケースは無くてもそんなに問題無いんじゃないかなと言う気になりますね。紙袋は `台北101`_ を模したPyCon TWのロゴと各スポンサーのQRコードがあしらわれています。プログラムパンフレットはB5の紙を3つ折りにしたもので、昨年の数十ページのものに比べるととてもシンプルになりました。そういえば各セッションの概要についてはプログラムにもサイトにも記載されていませんでしたが、このあたりは何か事情があるのかもしれません。Tシャツは参加者全員に配られ、ちょっとポップな感じで普段着に使っても良いデザインだと思います。写真左上の小さい箱の中にはサンドイッチなどちょっとした朝食が入っていました。現地の人でも遠くから来ている人はいるでしょうし、こういうちょっとした気遣いは嬉しいですね。


.. _`台北101`: http://www.taipei-101.com.tw/index_jp.htm


私はPyCon JP/APACの予算立てに関わっているのですが、その観点から見ると、今回のイベント参加費は前回の1,300TWD(約3,700円)から1,900TWD(約6,600円)に値上がりしており、台湾の物価から考えると1,900TWDはかなり高額だと感じました。その分ノベルティーのTシャツや朝食、無料のレセプションなどにお金を掛けており、海外から参加した身としては「参加した感」があったし、2日目にはノベルティーのTシャツを着ていた参加者も多く、一体感があって良いイベントになっていたと思います。このあたり、お金の掛けどころはなかなか悩ましいですが、イベントの雰囲気に直結する部分でもあるので、今回のPyCon TWはうまく活用できていたように感じました。


Keynote Speech: Making with Python 3
====================================
鈴木たかのりです。

最初のキーノートスピーチは `David Beazley 氏 <http://www.dabeaz.com/>`_ (`@debeaz <https://twitter.com/dabeaz>`_)による "Making with Python 3" です。
このセッションでは Python 3 でのプログラミングの楽しさについての話がありました。
David 氏は `Python Essential Reference <http://www.amazon.com/Python-Essential-Reference-Developers-Library/dp/0672329786>`_ と
Python Cookbook の著者でもあり、今年の5月に発売された
`Python Cookbook, 3rd Edition <http://shop.oreilly.com/product/0636920027072.do>`_
は Python 3.3 に対応しているそうです。

現在 Python プログラミング言語では、今後はメンテナンスサポートのみの **Python 2** と、一部の言語仕様で Python 2 との後方互換性を排除した **Python 3** の2つのバージョンが存在しています。この基調講演では全 Python ユーザーが興味を持っている Python 3 の特徴や Python 3 に移行するタイミングについて講演されました。

.. figure:: /_static/david.jpg
   :width: 400

   David Beazley 氏

David 氏は17年前(!!)に参加したのが最初の PyCon で、そのときの参加者は数十名だったでそうです。まずは Python 3 が4.5年開発されていること、Python 3 が Python 2 のデザイン上の傷を修復したものであることといった説明がされました。

会場に「Python 3を使っている人」という問いかけをしましたが、10人程度といった感じでした。今年の PyCon US で同じ質問があったときには 10% くらいの人が手を上げたそうです。その後、dict_keys、整数の割り算、print メソッド、非同期IO(`PEP 3156 <http://www.python.org/dev/peps/pep-3156/>`_)、Enum(`PEP 435 <http://www.python.org/dev/peps/pep-0435/>`_)などの Python 3 での新しい部分について説明をしました。Unicode/Bytes については Python 3 ではもっとも痛いところだというのは共通認識のようです。

最後に「Python 3 でのプログラミングは楽しいか?」という自らの問いに対して、いろいろ揃っているので楽しい、今が Python 3 を試すときだ。として、キーノートをまとめました。

その頃、清水川さんはキーノート直後の自分の発表準備をしており、まったく発表を聞いていなかったそうです。

.. figure:: /_static/day1-shimizukawa-at-keynote1-time.jpg
   :width: 400

   キーノート後の発表に向けて資料最終調整中の清水川さん

Sphinx発表
==================

清水川です。今回、スピーカーとして参加したのですが、1日目のキーノート直後の発表と言うこともあり、当日は緊張する間もなく発表時間となりました。

.. figure:: /_static/day1-shimizukawa-sphinx.jpg
   :width: 400

発表は、 `Introduction to Sphinx documentation generator`_ というタイトルで Sphinx_ の紹介をしました。SphinxはreStructuredTextという記法で書いた文章をHTMLやその他のフォーマットに変換してドキュメントを生成するツールで、Pythonの公式ドキュメントや、Python以外にもPHPやRubyなど多くのツール類で使用されています。昨年のPyCon TWでSphinxについて触れた発表がまったく無かったため、活用方法よりも紹介が良いと思いこのテーマで応募しました。というか、英語での発表は初めてなので、紹介とデモなら簡単な英語で発表できそうと思ったというのもあります。個人的には昨年のPyCon JP 2012終了後から、毎週英会話レッスンを受けたり、SphinxのCo-Maintainerとして英語を書く機会が非常に多くなったこともあり、実際の英語力はともかく、英語発表できそうな気がしてきていたというタイミングだったというのもあります(笑)。

.. figure:: /_static/day1-shimizukawa-sphinx-atendees.jpg
   :width: 400

私のセッションの参加者は60人前後で、そのうちSphinxを使ってる人は1割の6,7人という感じでした。Sphinxを知ってる人は、というと半分以上の人が知っているようで、さすがにあちこちのドキュメントがSphinxで書かれているだけありますね。

.. figure:: /_static/day1-shimizukawa-sphinx-atendees2.jpg
   :width: 400


さて、肝心の発表はと言うと、Sphinx紹介、デモ、事例紹介と3つのパートに分けて行ったのですが、最初のSphinx紹介は発表練習を何度か行っていたこともあり問題なく進めることが出来ました。また、ネタを仕込んだ部分ではしっかりと笑いを取ることも出来たので多少緊張がほぐれた気もします。話す内容はiPadで見られるようにしていたのですが、アドリブが出来るほどとっさには英語が出てこないので、一言一句読み上げている様に見えたかもしれません。次の機会には暗唱できるくらいには話す練習をしてチャレンジしようと思います。


発表の、デモ部分については発表時間的に入りきらないのは分かっていたので、様子を見ながら随時スキップしていく作戦で行いました。デモ自体は見たままなので、まあまあ伝わった気がしますが、デモ内容を飛ばしながらアドリブで話すのは、話す側も聞く側もなかなか厳しかったように思います。私はこのあたりで一日分の英語エネルギーを大体使い果たしてしまいました。

.. figure:: /_static/day1-shimizukawa-sphinx-question-and-answer.jpg
   :width: 400

最後の質疑応答では、 IPython Notebook というツール（MatplotlibのグラフやSympyの数式をインタラクティブ表示したり入力した結果をHTMLで表示したりできる）とSphinxを連携させたことがあるか？という質問を受けて、私は使ったことが無いと回答したような気がしますが、続けて訊かれたことについては英語エネルギー不足だったこともありうまく理解できずに司会者に助けてもらいました。後で聞いたところ、どうやら会場内に経験者がいるかどうか聞いていたみたいです。質疑応答は発表の価値を構成する大きな要素だと思うので、次の機会までにヒアリングをもうちょっと練習しておきたいと思います。

質疑応答のあとでスライドの残り、 `PyCon APAC 2013`_ の紹介、 `Sphinx-users.jp`_ の紹介、そしてSphinx-users.jpからのプレゼントを行いました。 残念ながら持っていったTシャツがSとXXLのみだったため「欲しい」という人が1人しか居ませんでした。そのため、中国語でジャンケンを何て言うか練習したのを披露することはありませんでしたが、用意したプレゼントを手渡すことが出来て良かったです（このときSサイズのTシャツが1枚残ったのは夜のレセプションで役に立つことになります）。

.. figure:: /_static/day1-shimizukawa-sphinx-tshirt-present.jpg
   :width: 400


発表後、Tシャツをプレゼントした方と、廊下で10分ほどSphinxの中国語PDF出力の話しました。質問は、中国語の文字を :command:`make latexpdf` で出力しようとすると問題があって、日本語の場合はどうやっているのか？という内容でした。実はSphinxには日本語向けにいくつか特別な処理が入っていて、そのおかげでPDF出力や検索が機能するようになっていますが、これはlanguage設定が ``'ja'`` の場合のみ動作するようになっているため、日本語以外のマルチバイト文字言語ではうまく動作しません。いろいろな言語に対応出来るようにするにはlatexとマルチバイト文字両方への理解が必要なため、非マルチバイト文字圏の開発者だけでは簡単にはいかないだろう、という話をしました。

ということで、私の初めての英語発表、初めての海外発表はうまく行かないことも多くありましたが、とても有意義なものになりました。次の機会がPyCon TWになるかどうか分かりませんが、それまでにまたレベルアップして臨みたいと思います。この機会を設けてくれた PyCon Taiwan スタッフの皆さんに感謝いたします。また、この発表に向けて、旅行の手配やスピーチ練習、現地での写真撮影など、妻が現地まで来てフルサポートしてくれました。多大な協力をしてくれた妻には感謝してもしきれません。ありがとう、本当に助かったよ。

.. _Introduction to Sphinx documentation generator: http://shimizukawa.bitbucket.org/pycontw2013-sphinx-introduction/index.html

.. _Sphinx: http://docs.sphinx-users.jp/

.. _PyyCon APAC 2013: http://apac-2013.pycon.jp/

.. _Sphinx-users.jp: http://sphinx-users.jp/


1日目のセッション
====================

清水川です。1日目の日中はいくつかセッションを見て廻りましたが、朝からの発表準備や発表疲れもあり、基本的にぐったりしていました。また、3トラックのうち1つは英語トラックなのですが、それ以外のトラックでは話している言葉が分からないため、なかなか厳しかったですね。

そんな状態でしたが、参加したセッションからすこし紹介したいと思います。

Python memory management & Impact to memory-hungry application
--------------------------------------------------------------
:発表者: 郭彥廷(`Kilik <https://www.facebook.com/kilik.kuo>`_) 
:動画: http://www.youtube.com/watch?v=iCzAmzGDTWk

`Python memory management & Impact to memory-hungry application`_ という発表では、連続したメモリをOSで確保できない状況でも巨大な連続メモリ空間を使えるようにする、PyBankというPyObjectのメモリバンク実装について紹介していました。

.. figure:: /_static/day1-pybank1.jpg
   :width: 400

   8000x6000 pixelsの巨大な画像データ


.. figure:: /_static/day1-pybank2.jpg
   :width: 400

   連続したメモリを必要とする巨大画像を複数扱う

8000x6000 pixelsもの高精細な写真では、イベントコンパニオンのバストアップ写真で産毛が判別できるほどの精度を持っています。このような巨大な画像データを扱うには連続したメモリ空間が必要で、さらに画像加工のためにはそのような巨大連続メモリ空間が複数画像分必要となります。PythonのPyObjectでそのようなことをすると連続したメモリが確保出来ずMemoryErrorとなってしまう問題と、そのような問題を回避するためにPyBankを用いるといったことや、その仕組みをPythonのC言語の実装でどのようにして実現するかといったことを紹介していました。

実践的な内容というよりはPythonのC実装モジュールの解説という雰囲気でしたが、立ち見も含めて80名ほどの参加者が興味深そうに聞いていたのが印象的でした。


Praat-py: The Force Unleashed!
-------------------------------
:発表者: 王文傑(PeterWolf)

.. figure:: /_static/day1-praatpy.jpg
   :width: 400

   Praat-py の発表

`Praat-py: The Force Unleashed!`_ という発表では、音声学の分野で使われる音声分析ソフトウェア Praat_ の紹介と、その操作を簡単に行うための補助ツール praat-py_ について紹介していました。音声学というのはこの発表で初めて知ったのですが、物理現象としての音を扱うのでは無く、音声学では人間の耳が音をどう捉えているかに注目するそうです。そのために人間が感じている音の違いをコンピューターで分析するツールが「Praat」で、年齢が上がるにつれて高周波数帯の音を聞き分けにくくなる、といった現象も再現して見ることができるそうです。PraatはGUIツールなのですが、その操作をスクリプト保存して繰り返し実行できる機能を持っています。しかし、そのスクリプトの文法がわかりにくいのでPythonスクリプトで扱えるようにするのがpraat-pyということでした。

発表自体は音声学の紹介とPraatoのデモを中心としたものだったため、Pythonの要素はほとんどありませんでしたが、数学系の特色が強いPyCon TWの特徴をあらわした発表だったと思います。


.. _`Python memory management & Impact to memory-hungry application`: http://tw.pycon.org/2013/ja/speaker/#speaker_id_16
.. _`Praat-py: The Force Unleashed!`: http://tw.pycon.org/2013/ja/speaker/#speaker_id_32
.. _Praat: http://www.fon.hum.uva.nl/praat/
.. _praat-py: https://github.com/tauberer/praat-py

Lightning Talks
===============
清水川です。

1日目の16時過ぎからはライトニングトーク(LT)、中国語では **閃電秀** と書くようです。
LTは技術系カンファレンスではおなじみの、一人5分ほどの短い時間でプレゼンテーションを行うものです。
今回のPyConTWでは事前にLTの募集をしていましたが、当日も募集しており、最終的には15ほどの発表が行われました。

.. figure:: /_static/day1-lt-recruitment.jpg
   :width: 400

   1日目午後、LT募集中

LTの最初の2つが日本人参加者の発表でした。

まず1人目が、鈴木たかのりさんの ``Introduction of PyCon APAC`` です。
LT1人目ということもあり、本人はかなり緊張していたとのことですが、発表を見ていた私としては非常に落ち着いていたように思います。発表中は、しっかりと笑いを取りつつ、今年の秋に行われる `PyCon APAC 2013`_ を紹介していたハズなのですが、途中からボルダリングの話に……詳しくは当日の資料と動画を公開していますので、是非ご覧下さい。

.. figure:: /_static/day1-lt-takanory.jpg
   :width: 400

   鈴木たかのりさんのLT発表

:資料: http://www.slideshare.net/takanory/pyconapac-0525
:動画: http://www.youtube.com/watch?v=8lSMCSd8oCo
:動画(オフィシャル): http://www.youtube.com/watch?v=USPaHaFqM1Y

.. _`PyCon APAC 2013`: http://apac-2013.pycon.jp/

LT2人目は、日本からPyConTWのスポンサーとして参加している `(株)Catchball21`_ さんの ``Introduced CatchBall21 company and promise with Yung-Yu Chen.`` です。
「昨年のPyConJPに来ていた `Yung-Yu Chen`_ 氏と2013年のPyConTWに行くよ、と約束したのでやって来ました」とPyConTWに参加した経緯を紹介しつつ、昨年自社の標準開発言語をPythonにしたこと、どのようなことにPythonを使っているかなどを紹介し、最後に「Pythonistaを募集してます！」と締めくくりました。

:資料: http://www.slideshare.net/shnmorimoto/pycon-taiwan-2013-lt-cb21-from-japan
:動画: http://www.youtube.com/watch?v=q0QOFdSHAiw


.. _`(株)Catchball21`: https://www.cb21.co.jp/


これ以降のLTでは以下の発表が行われました。

- WeasyPrint − bring the web to PDF and paper - Simon Sapin
- 用 Python 讓 Raspberry Pi 和臉部辨識來個小小相遇 (暫定) - 王興謙
- Bottle vs. Startup （微議程之 - 微框架 vs. 微創業） - 曾君宇
- Modularize your Django settings - 潘韋成
- Building a fast digit recognition solution with Python - 許家誠
- 3 個不同的 Python 組織文化 - Keith Yang
- 真蝦! 意外接到的 case - 陳炯廷
- Violent Python: Python in the dark side. - xatierlike Lee
- Dot.py - 陳建勳
- The Zen of Language Choice - TsungWei Hu
- doctest: 註解、測試一次搞定 - 梁睿珊
- （他、当日募集分）

タイトルを見たとおり、ほぼ中国語での発表だったのですが、doctestとSphinxについてのLTがあったので紹介します。
``doctest: 註解、測試一次搞定`` の発表者 `Jenny`_ はMoskyに「なぜそんなに速くプロダクトを書けるのか」という質問をしたところ、「doctestとSphinxを使っているから」という答えをもらったそうです。LTで紹介されたのは、コード中にdocstringとしてドキュメントを書いてこれをdoctestでテストする方法と、docstringを書いておけばSphinxで自動的に抽出してドキュメントを生成できるという例でした。ちなみにMoskyは昨年のPyConTWに参加した際に知り合った台湾の大学生で、PyCon JP 2012にも参加して `Clime: With A Line, Convert Your Functions into a Multi-Command CLI Program`_ という演題で発表してくれた方です。

.. _`Clime: With A Line, Convert Your Functions into a Multi-Command CLI Program`: http://2012.pycon.jp/program/sessions.html#session-15-1430-room351a-ja

.. figure:: /_static/day1-lt-jenny.jpg
   :width: 400

   梁睿珊 (Jenny/jsliang) さんのLT発表

:資料: http://www.slideshare.net/juishanliang/py-contw2013-doctest
:動画: http://www.youtube.com/watch?v=y7sk2gW8y3E

.. _Jenny: http://tw.pycon.org/2013/ja/speaker/#speaker_id_15

鈴木たかのりです。

ここでは発表した自分目線から少し裏話を書きたいと思います。
私自身初めての海外での英語での発表でしたので、非常に緊張しました。私は通常の30分発表でもエントリーしていたんですけど、正直落選してよかったなーと清水川さんの発表や自分で発表の準備をしていて思いました(笑)。

その場でしゃべるのは自分の英語力として絶対無理だろうと思っていたので、発表用のテキストを作ってプレゼンテーション資料のノートに書き込みまくりました。ただ、「こいつ原稿読んでいるなー、つまんねーなー」とは感じさせないように、できるだけ前を向いてしゃべることと、大きい声でしゃべることを心がけました。あとは次のスライドに移るための導入の部分は一つ前のスライドのメモに書くなどの工夫を心がけて、全体的に流れが悪くならないように注意しました。

発表をしているときは、最初の「今年の APAC は日本開催です!!」みたいなところで、会場がシーンとなって「ヤバイ、ここで拍手くるはずだったのに!!」と焦りましたが、その後はだいたい予定していたところではウケてもらえ、ほっとしました。動画を見ていると自分が舞台上で感じていたよりもウケているようで、ちょっとした感動すら覚えました。その努力が実を結んだのかはわかりませんが、写真撮影の時や打上げ時に「自分もボルダリングやってるんだよ」みたいに声をかけてくれる台湾の人がいました。後半にネタを入れすぎたので、前半の PyCon APAC のことを忘れられているような気もしますが...

なにはともあれ、貴重な体験をすることができて、こんな機会を設けてくれた PyCon Taiwan スタッフに感謝の言葉しかありません。


レセプション、BoF
=================
17時頃から予定していたレセプション（晩宴）はLTが伸びたため17時半過ぎから始まりました。レセプション会場がメインホール前のフロアで無料だったこともあり、自然に人が集まって自然に始まった感じでした。

.. figure:: /_static/day1-reception1.jpg
   :width: 400

   レセプションの様子

レセプションのどこかで何か案内があるのかなと思っていたのですが、短い案内が中国語でのみだったので、最初ちょっとどうしたらいいのか分かりませんでした。すぐにバンド演奏が始まって、みんな気ままにビュッフェ形式の料理を食べながら歓談していました。PyCon JP 2012のPartyでも同じようにDJを呼んで音楽を流していたのですが、 `Yung-Yu Chen`_ が昨年PyCon JPに参加して感銘を受けたらしく、今年のPyCon TWのレセプションで採用したらしいです。

.. figure:: /_static/day1-reception2.jpg
   :width: 400

   レセプションではバンド演奏や弾き語りなどが行われていました

レセプションでは、LTでdoctestとSphinxについての発表を行った Jenny_ と、Sphinx繋がりということで話をしてみたい、もしかしたらPyCon APAC 2013に来てくれるかも！？と思い、LTスライドで名前が出ていたMoskyに紹介してもらいました。Jennyは、私(清水川)のSphinxの発表時には友人の発表を聞いていたということでしたが、Sphinxにはとても関心があるとのことでした。Sphinx Tシャツ(S)をプレゼントしたところ非常に喜んでもらえました。今年秋のPyCon APAC 2013にも誘ったのですが、ちょうどその時期に残念ながら旅行に出かけているため参加出来ないそうです。残念。

.. image:: /_static/jenny_and_shimizukawa.jpg
   :height: 400

レセプションの時間には並行でBoFも行われてました。BoFというのはてっきり「Birds of a Feather（各ユーザー会の集会）」の事だと思っていたのですが、PyCon TWでは「BoF = Bazaar of folks」ということで、参加者は誰でも申請すればブースを貸してもらえる展示会のようなもののことでした。事前に `バザール出展のお誘い`_ として募集していましたが、ユーザー会のオフ会をやっているところもあれば、Raspberry Piのデモをしてるところもあり、あるいは難しそうな話をしているところもあり、という感じです。日本のイベントでは、オープンソースカンファレンスのブースが近い雰囲気ですが、もっと自由で雑然とした交流の場を形成していたのが良い感じでした。バンド演奏ありのレセプションエリアから数メートルのところでBoFを開催していたのも盛り上がりに貢献していたんでしょう。

.. figure:: /_static/day1-bof1.jpg
   :width: 400

   バザールの様子

.. figure:: /_static/day1-bof2.jpg
   :width: 400

   Raspberry Pi のデモ


バザールではPyLadiesという集まりのオフ会も行われていました。 PyLadies_ は世界各地域に集まりがあるようですが、まだほとんどアメリカだけなのかな。なかなか近づきがたかったため、どんな話をしているのかなど詳細はよくわかりませんでした。台湾でもPyLadies決起集会が行われた、ということにしておきます。そういえばMoskyとJennyも参加していたので今度機会があれば聞いてみようと思います。


.. image:: /_static/pyladies-taiwan.jpg
   :width: 400

.. _バザール出展のお誘い: http://tw.pycon.org/2013/ja/blog/2013/05/23/invitation-bazaar-folks-ja/
.. _PyLadies: http://www.pyladies.com/


夜市と散歩とPyCon談義
=====================
鈴木たかのりです。

レセプションがなんとなくお開きな感じになってきたので、日本から来たメンバーみんなで `夜市(ナイトマーケット) <http://www.tabitabi-taipei.com/kihon/act/walk.php>`_ に出かけました。
向かったのはカンファレンス会場から一番近い
`饒河街夜市 <http://www.taipeinavi.com/food/229/>`_ で、タクシーで185TWD(約650円)でした。関係ないですが、このタクシーで日本の演歌がかかっていて、なんというか不思議な気持ちになりました。

.. figure:: /_static/nightmarket.jpg
   :width: 400

   饒河街夜市の入り口

夜市は日本のお祭りの縁日みたいなところが、毎日あるようなところです。台湾ではあちこちに夜市があるようにで、毎日たくさんの人で賑わっています。この日もすごい人でした。夜市に行ったら台湾名物のかき氷(雪花冰)を食べます。アイス自体にミルクなどの味がついていて、マンゴーなどのフルーツがのって非常においしいです。

.. figure:: /_static/ice.jpg
   :width: 400

   台湾名物のかき氷(雪花冰)

私はこの夜市でだらだら歩いていたら他のメンバーとはぐれてしまい、一人で帰ることになってしまいました。去年もバスで移動したので Android の Google Map を頼りにバスで一人で帰りました。便利な世の中です。松山車站(駅)のバス停から30分弱でカンファレンス会場近くのバス停に到着しました。バス料金はだいたい15TWD均一なのですが、このとき私は小銭を50TWDしか持っていませんでした。バスの運転手さんに「これしか小銭がないんですけど、お釣りとかないですよね?」という感じのアピールをしたところ、運転手さんが「いいよいいよ、降りな」というジェスチャーで降ろしてくれました。台湾の人って優しい人が多いです。ありがとう台湾のバスの運転手さん!!

.. figure:: /_static/songshan.jpg
   :height: 400

   松山車站(駅)のバス停

バスを降りてからコンビニでマンゴー果汁の入った台湾ビールを買ってホテルに戻って来ました。最近 `fitbit <http://www.fitbit.com/jp>`_ という活動量計を使っているんですが、この日は食べた割にあまり動いていないなぁと思ったので、夜の散歩に出かけてみました。
`台湾 中央研究院 <http://goo.gl/maps/0Fsso>`_ は敷地が結構広いので、コンビニからの帰りにも犬を散歩させている人やランニングしている人によく遭遇しました。

.. figure:: /_static/taiwan-beer.jpg
   :height: 400

   台湾マンゴービール

途中で蛙のような謎な鳴き声が聞こえる池や、野良犬っぽい仲良し4匹の犬の群れと遭遇しつつ、気持よく散歩からホテルの前に戻ってきました。
すると `ホテル前の公園のベンチ <http://goo.gl/maps/syFDE>`_ から私に声をかける人がいます。「誰だ?」と思ってみてみると PyCon Taiwan 2013 の Chairperson の
`Yung-Yu Chen`_ 氏と
Secretary の `Tim Hsu`_ 氏でした。私は二人に「ちょっとビール取ってくるから」と告げて、ちょうど先ほど購入した台湾マンゴービールを持ってベンチに戻り、三人で話をしました。

そこでは、今年は PyCon APAC を日本で開催するが、どうやったら日本人と海外から来た人たちが交流できるか、日本と台湾の Python 関連コミュニティについてなどの話をしました。他にも来年は台湾が PyCon APAC を開催する予定であること、またその Chairperson を Tim Hsu 氏が務めることなどの話を聞きました。

ちょっとした気まぐれで夜の散歩に出たおかげで、台湾Python界の重要人物二人とフランクに話ができて非常にラッキーでした。関係ないですが、この時は私が台湾ビールを飲んでいて、Yung-Yu Chenがアサヒスーパードライ、Tim Hsuがお〜いお茶を飲んでいて、なんか不思議な感じでした。

こうしてPyCon Taiwanの一日目を終えました。

.. _Yung-Yu Chen: https://www.facebook.com/yungyuc
.. _Tim Hsu: https://www.facebook.com/wenchang.hsu

