# 2014-09-11 vim-fugitiveで遊ぼう


## vim-fugitiveとは
vim-figitiveはVimのプラグインで、Vim上で開いているバッファについての諸々のGitコマンドを実行出来る。
せっかくなのでVimで書いてGitBucketにあげているVim日記、VimからGit-Pushしてみる。

* [ダウンロードしてプラグインを入れる](https://github.com/tpope/vim-fugitive)

## コマンド
[参考1](http://yuku-tech.hatenablog.com/entry/20110427/1303868482)
[参考2](http://threetreeslight.com/post/56296194503/fugitive-vim)

* 新しい窓を作ってgit statusを表示

```vim:vimcommand
:Gstatus
```

* 現在開いているソースをgit add
ファイルパスを引数につけるとそのファイルを対象にするらしい。

``` vim:vimcommand
:Gwrite
```


* 現在開いているソースの直前のコミット時のソースを表示

``` vim:vimcommand
:Gread
``` 

* 現在開いているソースをgit mv

``` vim:vimcommand
:Gmove destination/path
``` 

* 現在開いているソースをgit rm

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

* 現在のソースをgit blame。
vimが色づけしてくれる。blameは行毎に誰がいつ書いたか表示してくれるよ。

``` vim:vimcommand
:Gblame
``` 


* 現在のソースの変更点をvimdiffで表示

``` vim:vimcommand
:Gdiff
``` 

* ヘルプ表示

``` vim:vimcommand
:help fugitive
``` 

----

## やってみよう

### console表示

``` vim:vimcommand
:Gstatus
```

![fugitive_console](./Images/fugitive_console.jpg)
なんか表示されたよ。


### git add 
このバッファ(今編集しているVim日記ファイル)をadd。
(このファイルは予めリポジトリのディレクトリに入れています。)

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

お手軽!
過去日記も移動するので、各々開いてコマンド呼んでaddしたよ。

### git commit 

``` vim:vimcommand
:Gcommit
```

また同じようなコンソール画面が出た。コミットメッセージを打ち込むらしいよ。
この画面全部がコミットメッセージで、頭に#付いているのは無視されるよう。
このファイルもコミットに含めてしまったので、書き終わらないうちにコミットされちゃうよ！

console画面で、:writeすることでコミット確定。また別のコンソールが出てきたよ。
![fugitive_commit](./Images/fugitive_commit.jpg)

### git push

``` vim:vimcommand
:Git push origin master
```
ユーザー打ったり、パスワード打ったり。
Pushまで出来た！やったー。


