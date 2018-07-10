# そもそもGitHub に登録しましょう，以下その前提で．

## GitHub サイト上で，リポジトリを作ってURLを取得しておく．

## local のディレクトリをリポジトリに push する．
https://qiita.com/bakainubau/items/4613dda50a5fa302d212
1. そのディレクトリに移動し，`git init`
2. `git add .` `git commit -m "FirstCommit"`
3. `git remote add origin https://github.com/Okdenn/HowtoGitHub.git`, URLは適宜リポジトリごとに変える．
4. `git push origin master` で完了．後は普段通り，ファイルを編集し，`git add hogehoge`, `git commit -m "hogepiyo"`, `git push origin master`するだけ．
### たまにサイトでリポジトリを作る前に local repository を commit してしまうことがある（なくしろ）．その際は，上の1-3までは同じで，
https://qiita.com/takanatsu/items/fc89de9bd11148da1438

5. `git fetch`
6. `git merge --allow-unrelated-histories origin/master` として半強制的にマージする．その後再び2を行い，`git push origin master` で完了．

**この段階で .gitignore を必要に応じて書き足しておくこと!!!** 後からではめんどくさい．

### cmd からリポジトリ作る方法ないんですかね...... いちいちサイト行くのなんかこう精神に反する感じがする．


## コマンドオプションについて
1. `git commit *-a* -m "hogepiyo"` の `-a` について．これは（バージョン管理されている）全てのファイルを，**add されていなくても** commit してしまうので，普段使いするものではない．反省せよ．

## .gitignore を書き忘れてしまって途中から書きたい場合