# 2014-09-11 vim-fugitive�ŗV�ڂ�


## vim-fugitive�Ƃ�
vim-figitive��Vim�̃v���O�C���ŁAVim��ŊJ���Ă���o�b�t�@�ɂ��Ă̏��X��Git�R�}���h�����s�o����B
���������Ȃ̂�Vim�ŏ�����GitBucket�ɂ����Ă���Vim���L�AVim����Git-Push���Ă݂�B

* [�_�E�����[�h���ăv���O�C��������](https://github.com/tpope/vim-fugitive)

## �R�}���h
[�Q�l1](http://yuku-tech.hatenablog.com/entry/20110427/1303868482)
[�Q�l2](http://threetreeslight.com/post/56296194503/fugitive-vim)

�V�������������git status��\��

```vim:vimcommand
:Gstatus
```

���݊J���Ă���\�[�X��git add

``` vim:vimcommand
:Gwrite
```

���݊J���Ă���\�[�X�̒��O�̃R�~�b�g���̃\�[�X��\��

``` vim:vimcommand
:Gread
``` 

���݊J���Ă���\�[�X��git mv

``` vim:vimcommand
;Gmove destination/path
``` 

���݊J���Ă���\�[�X��git rm

``` vim:vimcommand
:Gremove
``` 

git commit

``` vim:vimcommand
:Gcommit
``` 

git push

``` vim:vimcommand
:Git push origin master
``` 

���݂̃\�[�X��git blame�Bvim���F�Â����Ă����

``` vim:vimcommand
:Gblame
 ``` 

blame�͍s���ɒN�������������\�����Ă�����B


���݂̃\�[�X�̕ύX�_��vimdiff�ŕ\��

``` vim:vimcommand
 * �FGdiff
``` 

�w���v�\��

``` vim:vimcommand
 * :help fugitive
``` 

----

## ����Ă݂悤

``` vim:vimcommand
:Gstatus
``` 
�Ȃ񂩕\�����ꂽ��B
���̃o�b�t�@(���ҏW���Ă���Vim���L�t�@�C��)��add�B
(���̃t�@�C���̓��|�W�g���̃f�B���N�g���ɓ���Ă��܂��B)

``` vim:vimcommand
:Gwrite
``` 

