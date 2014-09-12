# 2014-09-11 vim-fugitiveで遊ぼう


## vim-fugitiveとは
vim-figitiveはVimのプラグインで、Vim上で開いているバッファについての諸々のGitコマンドを実行出来る。
せっかくなのでVimで書いてGitBucketにあげているVim日記、VimからGit-Pushしてみる。

* [ダウンロードしてプラグインを入れる](https://github.com/tpope/vim-fugitive)

## コマンド
[参考1](http://yuku-tech.hatenablog.com/entry/20110427/1303868482)
[参考2](http://threetreeslight.com/post/56296194503/fugitive-vim)

新しい窓を作ってgit statusを表示

```vim:vimcommand
:Gstatus
```

現在開いているソースをgit add

``` vim:vimcommand
:Gwrite
```

現在開いているソースの直前のコミット時のソースを表示

``` vim:vimcommand
:Gread
``` 

現在開いているソースをgit mv

``` vim:vimcommand
;Gmove destination/path
``` 

現在開いているソースをgit rm

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

現在のソースをgit blame。vimが色づけしてくれる

``` vim:vimcommand
:Gblame
 ``` 

blameは行毎に誰がいつ書いたか表示してくれるよ。


現在のソースの変更点をvimdiffで表示

``` vim:vimcommand
 * ：Gdiff
``` 

ヘルプ表示

``` vim:vimcommand
 * :help fugitive
``` 

----

## やってみよう

``` vim:vimcommand
:Gstatus
``` 
なんか表示されたよ。
このバッファ(今編集しているVim日記ファイル)をadd。
(このファイルはリポジトリのディレクトリに入れています。)

``` vim:vimcommand
:Gwrite
``` 

