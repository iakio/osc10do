.. rst2s5.py --no-compact-list --theme-url=ui\small-black-custom slide.rst slide.html

.. include:: <s5defs.txt>

==========================
���X�����Ȃ�vim�̘b
==========================
:Author: �Γc�N�Y(@iakio)
:Organization: Cycle of 5th / JPUG�k�C���x��
:Date: 2010-06-26

�����̘b
======================

* �����I�Șb�͂���܂���

* .vimrc�Ƃ�plugin�ɂ��Ă͂��܂�ڂ����Ȃ��ł�

* ���ivim���g���Ă��ĕ֗����ȂƎv�����ƁA�ǂ��������ɍl���Ȃ���vim���g���Ă��邩���s���|�C���g�Ő������܂�


�f�����ɂ���
================

* VirtualBox���CentOS��PuTTY�ڑ�

* vim-enhanced-7.0.109-6.el5

* screen + rectick(���X����)

* vimrc


����vim(1)
==========
.. class:: incremental

* vi����10���N

* h/j/k/l, i, a, x, dd, yy, p, :wp

* ���R���H


����vim(2)
==========
.. class:: incremental

* cw

* change word

* �J�[�\���̉�����P��̏I���܂ł�ύX����


���H�I�ȃR���{(1)
=================

/foo<CR>
  foo������(���� * �ŃJ�[�\���̉��̒P�������)

cwbar<Esc>
  foo��bar�ɕύX

n
  �O��̌������J��Ԃ�

.
  �O��̕ύX���J��Ԃ�

���H�I�ȃR���{(2)
=================

.. class:: center huge

n.n.n.n.n.n.n.n.n.n.


�@���Ƀp�^�[���ɂ������ނ�
==========================

1. ����������̐擪��������Ƃ����ύX������

2. ����������̍Ō��������Ƃ����ύX������

  cw���ƕ�����S�̂���͂��Ȃ����K�v������


operator��motion
=================

.. class:: center huge

| c    w
| {operator} {motion}

* motion�͒P�ƂŎg���ƃJ�[�\���ړ�

* operator�ƈꏏ�Ɏg���ƁA���݂̃J�[�\���ʒu����ړ���̈ʒu�܂łɑ΂��ĕύX�����s��


operator���낢��
===================

cw
  change word

dw
  delete word

yw
  yank word

gUw
  make upper case

motion���낢��
===================

cfx
  ����x�܂ŕύX

ctx
  ����x�̑O�܂ŕύX

c%
  �Ή����銇�ʂ܂ŕύX

ci"
  ".."�̒���ύX(text objext)


������offset
======================

/abcd/e
  abcd���������ăJ�[�\�����Ō��(d�̈ʒu)

/abcd/s+1
  abcd���������ăJ�[�\�����ŏ�+1��(b�̈ʒu��)


�܂Ƃ�
==========================
.. class:: incremental

* n.n.n.n.n.n.n. �����p���悤

* motion���ɂ߂悤 :help {motion}

* llllll���邭�炢�Ȃ点�߂�wwwwww


���Ò����肪�Ƃ��������܂���
============================
