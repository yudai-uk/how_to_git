# how_to_git
とりあえずgitの使い方

```shell
# 対象ディレクトリに移動して初期化
git init

# git remote add origin https://~
# このコマンドはoriginというショートカットにレポジトリのURLを登録する処理
# git add origin mainなどと使うときにURLを打つのがめんどくさいから登録する
git remote add <ショートカット> <レポジトリのURL>

# git pull <ショートカット名> <ブランチ名>
git pull origin main
```