=======
 Day 2
=======

招待講演と基調講演
==================
鈴木たかのりです

PyCon Taiwan の2日目は招待講演(Guest Speech)と基調講演(Keynote Speech)がありました。それぞれ簡単に紹介します。

Pythonic Epistemology
---------------------
:発表者: Allen Downey(`allendowney.com <http://allendowney.com/>`_)
:資料: `Python Epistemology: PyCon Taiwan 2013 <https://docs.google.com/presentation/d/1xEim-cnkUORU_tLBT1P-wnJ78xU_lbydAOdkrszps_M/edit#slide=id.p>`_
:動画: http://www.youtube.com/watch?v=XpPfv2zPWoQ

Allen Downey 氏の招待講演は、中継によって行われました。氏は大学でコンピューターサイエンスを教えているそうなので、おそらくその部屋からの中継のようです。
台湾の会場では2画面を使って、公園をしている Allen Downey 氏と資料を映しだしていました。発表には `Google Houngouts <http://www.google.com/+/learnmore/hangouts/?hl=ja>`_ を使用して、スライドの共有には `Skype <http://www.skype.com/ja/>`_ を使っているのが個人的には興味深かったです。

内容としては課題があって、それを Python でこう書くと綺麗にアルゴリズムが評伝できるよという解説があり、実際に授業を受けているような気持ちになりました。プログラミングは目的ではなくて課題を理解するための道具であるといって話をしていました。

.. figure:: /_static/guestspeech1.jpg
   :width: 400

   Allen Downey 氏による Guest Speech

Allen Downey 氏が書いた `Think Python <http://shop.oreilly.com/product/0636920025696.do>`_ という書籍もあるようです。
`Think Python: How to Think Like a Computer Scientist <http://www.greenteapress.com/thinkpython/>`_ から全文を読むことができるようです。興味を持った方は読んでみるとよいかも知れません。

Building to scale
-----------------
:発表者: David Cramer(`@zeeg <https://twitter.com/zeeg>`_)
:資料: `David Cramer: Building to scale <http://www.slideshare.net/it-people/david-cramer-building-to-scale>`_

2日目の基調講演は David Cremer 氏による Building to scale というスケーリングに関する話です。
氏は現在 `tenXer <https://www.tenxer.com/>`_ というデータ解析ツールを開発する会社で働いているそうです。現在携わっている tenXer や
`Disqus <http://disqus.com/>`_
`Sentry <https://getsentry.com/>`_ での経験を元に話をしていました。

.. figure:: /_static/guestspeech1.jpg
   :width: 400

   Daivd Cramer 氏

セッションの紹介
================

當 Python 遇上魔術方塊
----------------------
鈴木たかのりです。ここでは「當 Python 遇上魔術方塊」というセッションについて紹介します。このセッションではルービックキューブ(魔術方塊)の解き方の解説と、それを Python で実装した pyRubiks ついて紹介していました。

:発表者: 戴嘉駿(darkgerm) 
:資料: https://docs.google.com/file/d/0B64bMmimU6LaTzFMMTJCU1c5RUk/edit

.. figure:: /_static/rubik1.jpg
   :width: 400

   戴嘉駿(darkgerm)氏

前半はルービックキューブの解き方を図を交えてわかりやすく紹介していました。最初に「爆力解(?)」というのがあって、それはもしや?と思ったら想定通りでした。昔良くやりました。

.. figure:: /_static/rubik2.jpg
   :width: 400

   爆力解

その後手書きメモなども交えて、いろいろな解き方について説明がありました。ルービックキューブの解き方には色んな種類があるんですねー。私は爆力解以外で自力で6面揃えたことがない気がします。

さて、後半はルービックキューブを自動で解く pyRubiks についての解説です。コードは bitbucket で公開されているようです(https://bitbucket.org/darkgerm/pyrubiks)。
pyRubiks 以下のようにいくつかの部分にわかれているようです。

- 実際のルービックキューブを `SimpleCV <http://www.simplecv.org/>`_ で読み取り XML ファイルを出力
- XML file を XML parser を使って cube class のコードに変換
- cubeSolver でルービックキューブを解き、解く手順を出力
- `VPython <http://www.vpython.org/>`_ で実際の動作をアニメーション表示

また cubeSolver の部分は `NumPy <http://www.numpy.org/>`_ を使用しているそうです。
実際の解き方は
`Fridrich Method <http://en.wikipedia.org/wiki/Fridrich_Method>`_ というものを使っているそうです。

.. figure:: /_static/rubik3.jpg
   :width: 400

   pyRubiks の全体像

発表者はルービックキューブが非常好きなようで、いろいろな Python のモジュールを使ってルービックキューブを解くプログラムを作っていて、趣向の変わった面白い発表でした。

駭客看 Django
-------------

清水川です。PyCon TWではWebフレームワーク系の発表が少なく、Django, Pyramid, Ploneの発表が1つずつでした。その中の一つ、Djangoの発表はWebフレームワークの紹介ではなく、Djangoをどうやってクラックするかという内容でした。発表タイトルの「駭客看 Django」は日本語で「Hackerから見たDjango」という感じみたいですね。発表の前半ではDjangoとRailsを対象にした脆弱性数の比較などを紹介していましたが、中盤からは今のDjangoにどのような弱い点があって、そこをどうやって突破するのかといった実例を紹介していました。結論としては、Djangoは十分にセキュアな作りになっているんだけど、使い方を間違えると脆弱性を作り込んでしまう、という話でした。Djangoを使っている人は一読する価値があるのではないかと思います。

.. figure:: /_static/day2-django.jpg
   :width: 400

   Djangoのセキュリティー話に20人以上が立ち見

:発表者: Orange
:資料: https://speakerdeck.com/p8361/hai-ke-kan-django



朝食、お弁当、ティーブレイク
============================
鈴木たかのりです。1日目のレポートで清水川さんも書いていましたが、今回は朝食、ランチのお弁当、ティーブレイクがついていて、会期中にお腹が空いたということがありませんでした。どちらかというと食べ過ぎになりそうなので、おやつを節制していました。ランチ、ティーブレイク会場はメインのカンファレンスホールの裏にありました。それほど混雑することもなくおいしいランチにありつけました。

.. figure:: /_static/bento1.jpg
   :width: 400

   お弁当(1日目)

.. figure:: /_static/bento2.jpg
   :width: 400

   お弁当(2日目)

.. figure:: /_static/lunch.jpg
   :width: 400

   ランチ会場の様子

.. figure:: /_static/teabreak.jpg
   :width: 400

   ティーブレイクのおやつ

また、2日目のティーブレイクの時間では日本からお土産に持っていった PyCon JP Tシャツを主要なスタッフや台湾のスピーカーに渡して「Proposal出してね、今年は日本に来てね」と地道なアピール活動もしてみました。なんとかTシャツを配りきって荷物を減らすことができてほっとしました。

.. figure:: /_static/pyconjp-t1.jpg
   :width: 400

   app engineについて発表を行った David 氏と清水川さん

.. figure:: /_static/pyconjp-t2.jpg
   :width: 400

   HackerからみたDjangoについて発表を行った Orange 氏と宵 勇樹さん

データサイエンス系のセッション紹介
==================================
宵です。PyCon Taiwan では学術系の方の発表が多く、さらにpython自体 `numpy <http://www.numpy.org/>`_ など数値計算系のライブラリが出てきているため、
いくつかデータサイエンス系の発表もありました。ここでは軽く掲載しておきます。

- **Getting Python To Learn From Only Parts Of Your Data**

  - Dr. Ami Tavory
  - 機械学習用ライブラリScikit-learnを使った、交差検定やブースティングの例を紹介していました。

- **Scientific Data Analysis Pipelines - Push, Pull, React, Or Schedule?**

  - Dr. Ami Tavory
  - ETL(Extract/Transform/Load)的なデータの処理に関して、pythonのgeneratorを使って対処する方法を紹介していました。

- **Big Data Analysis in Python**

  - Jimmy Lai
  - 資料: http://www.slideshare.net/jimmy_lai/big-data-analysis-in-python
  - あるWeb投稿サイトのテキストを収集して、オススメのテキストを推薦するシステムの構築について紹介していました。テキストの格納にはmongoDB,Solrを使い、オススメするかどうかの判定には、単語の出現頻度に対してSVM(サポートベクターマシーン)を使うことで対処しています。

くじ引き、クロージング、集合写真
================================
- 日本語と英語が少し分かる台湾の方と知り合った！
- クロージング英語無くて辛かった

2日間の発表を終えてくじびき大会とクロージングです。
去年に引き続き PyCon Taiwan では `pylottery <https://bitbucket.org/pycontw/pylottery>`_ というプログラムを使って抽選するのが伝統のようです(去年の PyCon JPでは手抜きして `random <http://docs.python.jp/2/library/random.html>`_ モジュールを使っていました)。

pylottery プログラムが起動するとなんかなぞのキャラクターが出て来ました。

.. figure:: /_static/day2-closing1.jpg
   :width: 400

   Pythonista召喚ルーレット

その後、インベーダーみたいな画面が表示されて、これで画面上部の数字を撃ちぬくと番号が決まるという仕組みです。その操作方法が斬新で、左右のマイクから声を出してボリュームが大きい方に機体が動くというものでした。

.. figure:: /_static/pylottery1.jpg
   :width: 400

   pylottery の画面

数字がこのように確定すると、PyCon Taiwan とスポンサー企業のロゴが出るというのは、なかなかいいアイデアだと思いました。

.. figure:: /_static/pylottery2.jpg
   :width: 400

   抽選結果とロゴ

しかし、この抽選がグダグダでなかなか進みませんでした。百の位で6とか7とかを連発していて「いや、そんなに人いないから」(PyCon Taiwan の参加者は400名超)って感じで何回も空振りします。いそうな数字になっても該当者が現れず再抽選となったりして、かなり抽選に時間を要しました。LLイベントではゴムボールを投げてプレゼントを渡しているそうで、それだと空振りがないので効率的だなーと思いました。

.. figure:: /_static/day2-closing2.jpg
   :width: 800

   クロージング中に知り合ったQmole氏と、清水川さん

くじ引き後のクロージングで、PyCon Taiwan 2012, 2013 の Chairperson Yung-Yu Chen 氏から、来年は PyCon APAC 2014 を台湾で開催するつもりであること、Tim Hsu 氏が来年の Chairperson を務めるということが発表されました。二人は壇上でハグし、その後 Tim 氏が今後について話してましたが、中国語なので詳しいことはわかりませんでした。

.. figure:: /_static/day2-closing3.jpg
   :width: 400

   `Yung-Yu Chen`_ 氏(右)から `Tim Hsu`_ 氏へバトンタッチ

最後に全員でカンファレンスホールの表階段に集合し、写真撮影を行いました。このとき実は雨が少し降っていて、そのためこんな感じで階段の上の方に人が集まる形となりました。みなさんいい笑顔しています。こうして二日間の PyCon Taiwan は成功裏に終了しました。

.. figure:: /_static/group.jpg
   :width: 800

   集合写真


.. _Yung-Yu Chen: https://www.facebook.com/yungyuc
.. _Tim Hsu: https://www.facebook.com/wenchang.hsu

ディナー、その後ビール
======================
鈴木たかのりです。

集合写真が終了すると基本的に PyCon Taiwan はそこで終了ですが、私達はスタッフやスピーカーがあつまる打ち上げ的なディナーに呼ばれて参加しました。
会場は宿泊していた施設のレストランで、ビュッフェスタイルの中華を楽しみました。

去年も私はこの打ち上げに参加したんですが、そのとき3テーブルくらいの規模でほとんどはスタッフだけの小じんまりとしたものでした。今年はキーノートや他の外国人スピーカーも参加していて、大変賑わっている感じでした。

.. figure:: /_static/dinner1.jpg
   :width: 400

   打ち上げの様子

この場ではいろんな人と話をしました。Catchball 21 のメンバーは日本アニメ好きのPyCon Taiwanスタッフとアニメの話題で盛り上がっていました。私は写真撮影で話をしたボルダリングをやっている人と話をして、 `#kabepy ステッカー <http://twitpic.com/cb04wq>`_ を持って行かなかったこと非常に悔やみました。

.. figure:: /_static/dinner2.jpg
   :width: 400

   台湾のクライマー Moogoo Lee と一緒に

また、打ち上げのときにおみやげとしてPyCon Taiwan Tシャツを数枚もらっいました。ここだけの話、作りすぎて数が結構余ったそうです。グッズを作るときの数を読むのが難しいという悩みは、一緒なんだなーと感じました。

打ち上げが終わって、さてお開きかなーと思ったのですが、ここでスピーカーの一人の David Cramer(`@zeeg <https://twitter.com/zeeg>`_)氏が「ビールを飲みに行こう!!」とみんなを誘っていました。疲れているしどうしようかなーと思ったんですが、せっかくなので私も飲みに行くことにしました。
タクシーとMRTを乗り継いで着いたのは `On Tap <http://www.ontaptaipei.com/>`_ というブリティッシュパブです。お店の中はどちらかというと白人系の人が多い感じでした。台湾に来て台湾ビール以外のビールを飲むのは初めてです。長めのテーブルに15、6人くらいで座っており、テーブルのこちら側ではおのおの好きなビールを頼んでいたんですが、向こう側はなにやらすごいものを注文していました。ちょっと暗くてわかりにくいですが、この入れ物(ビールタワー)は上部にビールが一杯に入っていて、それを自分で注いで飲むというスタイルでした。ビールのピッチャーのもっとすごいバージョンって感じです。

.. figure:: /_static/beer-tower.jpg
   :height: 400

   ビールタワー

ここでいろんな人と話をしていましたが、隣の席に Orange というTシャツも渡したスピーカーと話している時、彼は英語を話したり聞いたりするのは苦手ということで、急に Mac を取り出してタイピングを始めました。ブラウザ上に高橋メソッド用のツールを読み込んでいるそうで、タイピングした文字が大きく画面に表示されます。その画面上で二人で会話をしました。私もヒアリングとかそんなに得意ではないので、この方式はなかなか便利だし面白いなーと感じました。台湾でも ``orz`` が通じるとか、日本では「笑い」を ``ww`` で表すけど、台湾では ``XD`` で表すよねー、みたいな話もしました。このあたりはタイピングしているからこそできた会話かも知れません。

.. figure:: /_static/orange-mac.jpg
   :width: 400

   Orange とのやりとり

こんな感じで PyCon Taiwan の二日目は終わりました。知り合いが増えたこともあり、昨年以上に充実した二日間でした。
