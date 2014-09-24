# 2014-09-11 vim-fugitive�ŗV�ڂ�


## vim-fugitive�Ƃ�
vim-figitive��Vim�̃v���O�C���ŁAVim��ŊJ���Ă���o�b�t�@�ɂ��Ă̏��X��Git�R�}���h�����s�o����B
���������Ȃ̂�Vim�ŏ�����GitBucket�ɂ����Ă���Vim���L�AVim����Git-Push���Ă݂�B

* [�_�E�����[�h���ăv���O�C��������](https://github.com/tpope/vim-fugitive)

## �R�}���h
[�Q�l1](http://yuku-tech.hatenablog.com/entry/20110427/1303868482)
[�Q�l2](http://threetreeslight.com/post/56296194503/fugitive-vim)

* �V�������������git status��\��

```vim:vimcommand
:Gstatus
```

* ���݊J���Ă���\�[�X��git add
�t�@�C���p�X�������ɂ���Ƃ��̃t�@�C����Ώۂɂ���炵���B

``` vim:vimcommand
:Gwrite
```


* ���݊J���Ă���\�[�X�̒��O�̃R�~�b�g���̃\�[�X��\��

``` vim:vimcommand
:Gread
``` 

* ���݊J���Ă���\�[�X��git mv

``` vim:vimcommand
:Gmove destination/path
``` 

* ���݊J���Ă���\�[�X��git rm

``` vim:vimcommand
:Gremove
``` 

* git commit

``` vim:vimcommand
:Gcommit
``` 

* git push

``` vim:vimcommand
:Git push origin master
``` 

* ���݂̃\�[�X��git blame�B
vim���F�Â����Ă����Bblame�͍s���ɒN�������������\�����Ă�����B

``` vim:vimcommand
:Gblame
``` 


* ���݂̃\�[�X�̕ύX�_��vimdiff�ŕ\��

``` vim:vimcommand
:Gdiff
``` 

* �w���v�\��

``` vim:vimcommand
:help fugitive
``` 

----

## ����Ă݂悤

### console�\��

``` vim:vimcommand
:Gstatus
```

![fugitive_console](./Images/fugitive_console.jpg)
�Ȃ񂩕\�����ꂽ��B


### git add 
���̃o�b�t�@(���ҏW���Ă���Vim���L�t�@�C��)��add�B
(���̃t�@�C���͗\�߃��|�W�g���̃f�B���N�g���ɓ���Ă��܂��B)

``` vim:vimcommand
:Gwrite
``` 

``` vim:figitive console
# Changes to be committed:
#   (use "git reset HEAD <file>..." to unstage)
#
#	new file:   VimDiary/2014-09-12_LetsPlayVimFigitive.md
#	new file:   VimDiary/2014-09-10_WallsOfVim.md
#	new file:   VimDiary/2014-09-12_LetsPlayVimFigitive.md
#
```

����y!
�ߋ����L���ړ�����̂ŁA�e�X�J���ăR�}���h�Ă��add������B

### git commit 

``` vim:vimcommand
:Gcommit
```

�܂������悤�ȃR���\�[����ʂ��o���B�R�~�b�g���b�Z�[�W��ł����ނ炵����B
���̉�ʑS�����R�~�b�g���b�Z�[�W�ŁA����#�t���Ă���͖̂��������悤�B
���̃t�@�C�����R�~�b�g�Ɋ܂߂Ă��܂����̂ŁA�����I���Ȃ������ɃR�~�b�g���ꂿ�Ⴄ��I

console��ʂŁA:write���邱�ƂŃR�~�b�g�m��B�܂��ʂ̃R���\�[�����o�Ă�����B
![fugitive_commit](./Images/fugitive_commit.jpg)

### git push

``` vim:vimcommand
:Git push origin master
```
���[�U�[�ł�����A�p�X���[�h�ł�����B
Push�܂ŏo�����I������[�B


