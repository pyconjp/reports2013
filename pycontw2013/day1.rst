=======
 Day 1
=======

ホテル(台北市内)から会場へ
==========================
宿泊した台北市内の `ホテル <http://www.fortunehiyahotel.com/main/getLanguage/jp>`_ から会場となる
`Academia Sinica <http://www.sinica.edu.tw/main_e.shtml>`_ への移動は、公共交通機関だと MRT(地下鉄)とバスを乗り継いがないといけないので多少不便です。

朝早くの移動ということもあり、私たちはタクシーで移動しました。だいたい30分くらいで会場に到着します。料金は330TWDです。タクシーの運転手さんはあんまり英語が通じる感じではないので、行き先の名前(漢字のもの)を紙で見せるのが通じやすいようです。

会場に到着したら、まずは今日の宿泊先となる
`Activity Center <http://proj3.sinica.edu.tw/~gao/huo-dong/room-online-en.php>`_ に荷物を預けて、身軽になってからカンファレンス会場に移動しました。

受付
====

- ノベルティー: 紙袋、Tシャツ(普段着にできそう)、名札(シンプル)、プログラム(シンプル)、朝食(2時間以内)
- 名札がシンプルになった。
- 2日前に登録番号入りのリマインダメールもらってたので迷わず。
- 昨年のような登録番号の掲示はしてなかった。
- オープニングが英語だった

Keynote Speech: Making with Python 3
====================================
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

David 氏は17年前(!!)に参加したのが最初の PyCon で、そのときの参加者は数十名だったでそうです。まずは Python 3 が4.5年開発されていること、Python 3 が Python 2 のデザイン上の傷を修正したものであることといった説明がされました。

会場に「Python 3を使っている人」という問いかけをしましたが、10人程度といった感じでした。今年の PyCon US で同じ質問があったときには 10% くらいの人が手を上げたそうです。その後、dict_keys、整数の割り算、print メソッド、非同期IO(`PEP 3156 <http://www.python.org/dev/peps/pep-3156/>`_)、Enum(`PEP 435 <http://www.python.org/dev/peps/pep-0435/>`_)などの Python 3 での新しい部分について説明をしました。Unicode/Bytes については Python 3 ではもっとも痛いところだというのは共通認識のようです。

最後に「Python 3 でのプログラミングは楽しいか?」という自らの問いに対して、いろいろ揃っているので楽しい、今が Python 3 を試すときだ。として、キーノートをまとめました。

その頃、しみずかわさんはキーノート直後の自分の発表準備をしており、まったく発表を聞いていなかったそうです。

.. figure:: /_static/day1-shimizukawa-at-keynote1-time.jpg

   キーノート後の発表に向けて資料最終調整中の清水川

Sphinx発表(清水川)
==================

.. todo:: 写真多い？

.. figure:: /_static/day1-shimizukawa-sphinx.jpg

- 部屋の参加者 -> 40人くらい
- Sphinx使ってる人！ -> 5人
- Sphinx知ってる人！ -> 30人くらい

- ちょっとしたネタを資料に仕込んで置いたところで笑いが取れたので安心した。
- 質疑応答ではイッパイイッパイになってしまって英語での質問の内容がうまく理解できずに司会者に助けてもらった。次の機会までにヒアリングをもうちょっと練習しておきたい。

.. figure:: /_static/day1-shimizukawa-sphinx-atendees.jpg

- Tシャツプレゼントしました。SとXXLなので欲しい人いなかった.. XXLだけもらい手が一人いて良かった。次の機会があったらちゃんとM/Lサイズを用意して置こうと思った。

.. figure:: /_static/day1-shimizukawa-sphinx-tshirt-present.jpg

- Tシャツをプレゼントした方と、Sphinxの中国語PDF出力の話を廊下でやってました。中国語の文字をlatexpdfで出力しようとすると問題があって、日本語の場合はどうやっているのか？ -> 日本語向けに異なる処理が入っている、いろいろな言語に対応出来るようにするにはlatexとマルチバイト文字両方への理解が必要なため非マルチバイト文字圏の開発者だけでは簡単にはいかないだろう、という話をした。

- その後昼まで疲れてぼーっとしてました。



なにか気になったセッション(清水川)
==================================

- 5/25 14:30 「Python memory management & Impact to memory-hungry application」（会議室１）
  連続したメモリをOSで確保できなくても巨大なメモリ空間を使えるようにするPyObjectのメモリバンク実装について（だったと思う）。PyBank。


- 5/25 15:30 「Praat-py: The Force Unleashed!」（会議室２）
  人間は年齢とともに高周波数の音を聞き分けにくくなっていく。
  人間が感じている音の違いをコンピューターで分析するツール「Praat」は
  GUI操作をスクリプト保存して繰り返し実行などができるが、文法がわかりにくい。
  これをPythonスクリプトで扱えるようにする話。


LT(たかのり、清水川)
====================
1日目の16時過ぎからはライトニングトーク(LT, 中国語では **閃電秀**)です。
事前にLTの申し込み登録がありましたが、当日も参加募集を募っており、15ほどのLT発表が行われました。

.. figure:: /_static/day1-lt-recruitment.jpg

   1日目午後、LT募集中


LTの最初の2つが日本人参加者の発表でした。

まず1人目が、鈴木たかのりさんの ``Introduction of PyCon APAC`` です。
LT1人目ということもあり、本人はかなり緊張していたとのことですが、発表を見ていた私としては非常に落ち着いて、しっかりと笑いを取りつつ今年の秋に行われる `PyCon APAC 2013`_ の紹介をしていました。発表の内容としては、PyCon APAC の紹介をしていたハズなのですが途中から……詳しくは当日の資料と動画を公開していますので、是非ご覧下さい。

.. figure:: /_static/day1-lt-takanory.jpg

   鈴木たかのりさんのLT発表

:資料: http://www.slideshare.net/takanory/pyconapac-0525
:動画: http://youtu.be/8lSMCSd8oCo

.. _`PyCon APAC 2013`: http://apac-2013.pycon.jp/

LT2人目は、日本からPyConTWのスポンサーとして参加している `(株)Catchball21`_ さんです。

* Introduced CatchBall21 comany and promise with Yung-Yu Chen.

.. todo:: もうちょっと内容紹介する

.. todo:: 資料あればURLを教えてもらう

.. 動画は http://youtu.be/_RxIrOkByTQ だが途中からなので掲載しない方がいいかな


.. _`(株)Catchball21`: https://www.cb21.co.jp/


3つめ以降のLTは中国語が多かったのですが、いくつか面白かったものを紹介します。

.. todo:: LTいくつか紹介

   * PyTesserというOCRエンジンのPythonブリッジ
     https://pypi.python.org/pypi/PyTesser ver 0.0.1
     PyTesserのバージョンは若すぎるけど、ブリッジしてるだけなら精度は
     Engine側次第かな

   * jenny(梁睿珊)のdoctest+sphinx
     day1-lt-jenny.jpg
     day1-lt-jenny-doctest.jpg
     http://www.slideshare.net/juishanliang/py-contw2013-doctest


.. 以下は予定していたLT
..
.. - Plone: Powerful Python based Content Management System - Takanori Suzuki
.. - Introduction to PyCon APAC 2013 in Japan - Takanori Suzuki
.. - WeasyPrint − bring the web to PDF and paper - Simon Sapin
.. - 用 Python 讓 Raspberry Pi 和臉部辨識來個小小相遇 (暫定) - 王興謙
.. - Bottle vs. Startup （微議程之 - 微框架 vs. 微創業） - 曾君宇
.. - Modularize your Django settings - 潘韋成
.. - Building a fast digit recognition solution with Python - 許家誠
.. - 3 個不同的 Python 組織文化 - Keith Yang
.. - 真蝦! 意外接到的 case - 陳炯廷
.. - Violent Python: Python in the dark side. - xatierlike Lee
.. - Dot.py - 陳建勳
.. - The Zen of Language Choice - TsungWei Hu
.. - doctest: 註解、測試一次搞定 - 梁睿珊


レセプション、BoF(清水川)
=========================
17時頃から予定していたレセプション（晩宴）はLTが伸びたため17時半過ぎから始まりました。レセプション会場がメインホール前のフロアで無料だったこともあり、自然に人が集まって自然に始まった感じでした。

.. todo:: レセプションの写真

LTで doctest + Sphinx の発表を行ったJenny(梁睿珊)を、昨年のPyConTWで知り合ったmoskyに紹介してもらいました。私(清水川)の発表の時間には友人の発表を聞いていたということでしたが、Sphinxにはとても関心があるとのことでした。Sphinx Tシャツ(S)をプレゼントしたところ非常に喜んでもらえました。今年秋のPyCon APAC 2013にも誘ったのですが、ちょうどその時期に残念ながら旅行に出かけているため参加出来ないそうです。残念ですね。


.. todo:: BoFは並行でやってた

.. todo:: PyLadiesについて

夜市(たかのり)
==============

夜散歩のあとにYY-chenと話したこと(たかのり)
===========================================
