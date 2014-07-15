# Vim

## vim-fugitive覚書
せっかくなのでVimからGitしよう
 * [ダウンロードしてプラグインを入れる](https://github.com/tpope/vim-fugitive)

### コマンド
[参考1](http://yuku-tech.hatenablog.com/entry/20110427/1303868482)
[参考2](http://threetreeslight.com/post/56296194503/fugitive-vim)

新しい窓を作ってgit statusを表示
 * ：Gstatus

現在開いているソースをgit add
 * ：Gwrite

現在開いているソースの直前のコミット時のソースを表示
 * ：Gread

現在開いているソースをgit mvする
 * ：Gmove destination/path

現在開いているソースをgit rmする
 * ：Gremove

git commit
 * ：Gcommit

git push
 * :Git push origin master

現在のソースをgit blame。vimが色づけしてくれる
 * ：Gblame

現在のソースの変更点をvimdiffで表示
 * ：Gdiff

ヘルプ表示
 * :help fugitive
