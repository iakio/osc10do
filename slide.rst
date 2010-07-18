.. rst2s5.py --no-compact-list --theme-url=ui\small-black-custom slide.rst slide.html

.. include:: <s5defs.txt>

==========================
今更聞けないvimの話
==========================
:Author: 石田朗雄(@iakio)
:Organization: Cycle of 5th / JPUG北海道支部
:Date: 2010-06-26

今日の話
======================

* 初歩的な話はありません

* .vimrcとかpluginについてはあまり詳しくないです

* 普段vimを使っていて便利だなと思うこと、どういう風に考えながらvimを使っているかをピンポイントで説明します


デモ環境について
================

* VirtualBox上のCentOSにPuTTY接続

* vim-enhanced-7.0.109-6.el5

* screen + rectick(少々改造)

* vimrc


私とvim(1)
==========
.. class:: incremental

* vi歴は10数年

* h/j/k/l, i, a, x, dd, yy, p, :wp

* 何コレ？


私とvim(2)
==========
.. class:: incremental

* cw

* change word

* カーソルの下から単語の終わりまでを変更する


実践的なコンボ(1)
=================

/foo<CR>
  fooを検索(又は * でカーソルの下の単語を検索)

cwbar<Esc>
  fooをbarに変更

n
  前回の検索を繰り返し

.
  前回の変更を繰り返し

実践的なコンボ(2)
=================

.. class:: center huge

n.n.n.n.n.n.n.n.n.n.


如何にパターンにもちこむか
==========================

1. 長い文字列の先頭をちょっとだけ変更したい

2. 長い文字列の最後をちょっとだけ変更したい

  cwだと文字列全体を入力しなおす必要がある


operatorとmotion
=================

.. class:: center huge

| c    w
| {operator} {motion}

* motionは単独で使うとカーソル移動

* operatorと一緒に使うと、現在のカーソル位置から移動後の位置までに対して変更等を行う


operatorいろいろ
===================

cw
  change word

dw
  delete word

yw
  yank word

gUw
  make upper case

motionいろいろ
===================

cfx
  次のxまで変更

ctx
  次のxの前まで変更

c%
  対応する括弧まで変更

ci"
  ".."の中を変更(text objext)


検索とoffset
======================

/abcd/e
  abcdを検索してカーソルを最後へ(dの位置)

/abcd/s+1
  abcdを検索してカーソルを最初+1へ(bの位置へ)


まとめ
==========================
.. class:: incremental

* n.n.n.n.n.n.n. を活用しよう

* motionを極めよう :help {motion}

* llllllするくらいならせめてwwwwww


ご静聴ありがとうございました
============================
