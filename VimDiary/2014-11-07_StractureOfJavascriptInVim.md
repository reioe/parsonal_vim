# 2014-11-07 Vim��JavaScript�J�����𐮂���

![syntastic_errors](./Images/syntastic_errors.jpg)

JavaScript�ŊJ�����Ă��Ċ��𐮂��Ȃ���΁A
�V���^�b�N�X�`�F�b�N���Ȃ��Ǝ��ʁA�Ƃ������ƂɂȂ����̂�
Vim�ɓ���Ă݂܂����Ƃ������b�ł��B


## �A�W�F���_
1. JavaScript�J�����ɕK�v�Ȃ��̂Ƃ���
1. �C���X�g�[��
1. ����


## JavaScript�J�����ɕK�v�Ȃ��̂Ƃ���

### �V���^�b�N�X�`�F�b�N�̋@�\
�����ł��Ă����Ɨǂ���ˁB

���ꂾ���ŏ\���B�I���j�⊮(�T�W�F�X�g)�Ƃ��͂���قǕK�v����Ȃ��A�Ǝv���B
���K�ɂȂ�悤��������g�ݍ��������B


### ���邱��

�����V���^�b�N�X�`�F�b�N�\���̃v���O�C���ł���[Syntastic](https://github.com/scrooloose/syntastic)�����āAjavascript�̃`�F�b�N���C�u�����Ƃ���[js.hint�̃m�[�h](http://www.jshint.com/install/js.hint)
������B

�����Ȃ̂����ǁA���̂��߂ɂ�
* node.js�̃C���X�g�[��
* npm�̒���
* neobundle�̃C���X�g�[��
�ȂǕK�v�ł��ꂼ��n�}�����̂ŁA���̓_�������܂��B


## �C���X�g�[��

### neobundle

[neobundle](https://github.com/Shougo/neobundle.vim)�̓v���O�C����github����_�E�����[�h���Ă��ꂽ��A
�X�V���`�F�b�N���Ă��ꂽ�肷��v���O�C���B�����Ǝ蓮�Ŋe�v���O�C�������Ċ撣���Ă�������ǁA
Syntastic���ǂ��������Ă���Ȃ��̂ŁA����m�����֗��ɃC���X�g�[���o����d�g�݂Ƃ���
�Җ]�̓����B��neobundle���̂̓����Ńn�}���ė܂�����ł����̂ŁA����T�N�b�Əo���Ċ������ȁB

### Syntastic

neobundle���g���ăC���X�g�[���B\_vimrc�Ɉȉ����L�q���āAvim���N������Ǝ����ŃC���X�g�[�������B

``` _vimrc
NeoBundle 'scrooloose/syntastic'
``` 

### node.js

[node.js�̃T�C�g](http://nodejs.org/)����C���X�g�[���B���ϐ���path��ʂ��炵���̂����ʂ�Ȃ��A�����Ȃ������B
���ϐ��Ɉȉ���ǉ��B

``` 
"C:\Program Files\nodejs"
``` 

### npm 

node.js�̃p�b�P�[�W�Ǘ��ł���[npm](https://www.npmjs.org/)��node.js�̃C���X�g�[�����ɓ����Ƀv���O�C���Ƃ��Ă��Ă���B�������N������ƃt�H���_�p�X��������Ȃ��Ɠ{��ꂽ�B
�Ȃ񂩐F�X���ׂ��


``` 
C:\Program Files\nodejs"C:\Users\[UserName]\AppData\Roaming\npm
``` 
�̃t�H���_���Ȃ��ē{���Ă���炵���B����ȂɃn�}���Ă�l���Ȃ����ۂ��̂�
�C���X�g�[���Ŏ��s���Ă���̂��낤�B�t�H���_��ǉ�����ƒʂ�悤�ɂȂ����B

### js.hint

node.js�̃p�b�P�[�W�Ƃ��Ă�js.jshint���_�E�����[�h����ƁAsyntastic������ɓǂݎ���Ă����炵���B
node.js��Windows�ŋN������ɂ�[msys.git](http://msysgit.github.io/)����bash���K�v�B�K��GitBash�������Ă����̂ŁA�R�}���h��@���B


``` 
$ npm install -g jshint
``` 

�������������B�ł��A���ꂾ���Ŋ����������B���Vim���N������js�t�@�C�����J���΁A
�����ŃV���^�b�N�X�`�F�b�N���n�܂��B


## ����

.js�t�@�C�����J���āASyntastic�̐ݒ���m�F���悤�B

``` vim:vimcommand
:SyntasticInfo
``` 

![syntastic_info](./Images/syntastic_info.jpg)


���������ɐݒ肳��Ă���ˁI


``` vim:vimcommand
:w
``` 

�ۑ����Ɏ����Ń`�F�b�N������A�G���[������΃}�[�N�����B
�s�ԍ����̍��ɗ̈悪�o����">>"���\�������̂ŁA�C�Â��₷���A�Ƃ����΋C�Â��₷������ǁA
���ƋC�t���Ȃ������B�o�Ă���̂ɓ�������IE��F12�̃G���[�ŋC�Â��܂����B

``` vim:vimcommand
:Errors
``` 
![syntastic_errors](./Images/syntastic_errors.jpg)

��łƂ���ȕ��ɔh��ɕ\�����Ă�����B������ˁB

������Œ���R�~�b�g�O�ɑł��Ċm�F����悤�ɂ���΁A�\���G���[�͖h����͂��B

