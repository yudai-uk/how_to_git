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

- 上記だけだと403やnot repositoryが出る可能性があるため、下記を対応する。
    1. `Personal Access Token`を発行する。
        - github内`settings`ページ
        - `Developers Settings`ページ
        - `Personal Access Token`
        1度しかトークンは表示されないため、コピーしておく

    1. 資格情報設定からユーザーにユーザー名,パスワードに先ほど発行した`Personal Access Token`を入れて保存する。

```shell
# ローカルにブランチを引っ張ってくるとき
git branch main remotes/main

# ブランチ変更
git checkout main

# ブランチ削除
git branch -d master

# ブランチ作成
git branch Hoge
```
