# そもそもGitHub に登録しましょう，以下その前提で．

## GitHub サイト上で，リポジトリを作ってURLを取得しておく．

## local のディレクトリをリポジトリに push する．
https://qiita.com/bakainubau/items/4613dda50a5fa302d212
1. そのディレクトリに移動し，`git init`
2. `git add .` `git commit -m "FirstCommit"`
3. `git remote add origin https://github.com/Okdenn/HowtoGitHub.git`, URLは適宜リポジトリごとに変える．
4. `git push origin master` で完了．後は普段通り，ファイルを編集し，`git add hogehoge`, `git commit -m "hogepiyo"`, `git push origin master`するだけ．
### たまにサイトでリポジトリを作る前に local repository を commit してしまうことがある（なくしろ）．その際は，上の1-3までは同じで，https://qiita.com/takanatsu/items/fc89de9bd11148da1438
5. `git fetch`
6. `git merge --allow-unrelated-histories origin/master` として半強制的にマージする．その後 `git push origin master` で完了．
