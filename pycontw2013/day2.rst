=======
 Day 2
=======

2日目のキーノート書ける?(しみずかわ->宵)
==========================================
- ThinkPython, 動画中継でのゲスト講演。
- (宵補足)話としてはpythonで綺麗にアルゴリズムを表現する方法を説明していました。例えば与えられた2つの単語がアナグラムになっているかどうかを判定する問題です。キーノートでの例とは少し変わりますが、"taiwan"と"anwait"はアナグラムになっています。pythonではいくつか解き方がありますが、例えば{ 単語:出現頻度 }のdictにまとめて比較を行えば綺麗にまとまります。 

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
- Djangoクラック話、超満員
  https://speakerdeck.com/p8361/hai-ke-kan-django 

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

クロージング、集合写真(清水川)
==============================
- 日本語と英語が少し分かる台湾の方と知り合った！
- クロージング英語無くて辛かった

.. figure:: /_static/day2-closing1.jpg
   :width: 800

   Pythonista召喚ルーレット

.. figure:: /_static/day2-closing2.jpg
   :width: 800

   クロージング中に知り合ったQmole氏と、清水川さん

.. figure:: /_static/day2-closing3.jpg
   :width: 800

   `Yung-Yu Chen`_ 氏から `Tim Hsu`_ 氏へバトンタッチ

.. figure:: /_static/group.jpg
   :width: 800

   集合写真


.. _Yung-Yu Chen: https://www.facebook.com/yungyuc
.. _Tim Hsu: https://www.facebook.com/wenchang.hsu

ディナー、その後ビール(たかのり)
================================
