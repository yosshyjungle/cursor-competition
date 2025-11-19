# GitHubリポジトリのセットアップ手順

## 1. GitHubでリポジトリを作成

1. [GitHub](https://github.com)にログインします
2. 右上の「+」ボタンをクリックし、「New repository」を選択
3. リポジトリ名を入力（例: `hp`）
4. 説明を追加（オプション）
5. 公開設定を選択（Public または Private）
6. **「Initialize this repository with a README」のチェックを外す**（既にREADME.mdがあるため）
7. 「Create repository」をクリック

## 2. リモートリポジトリを追加してプッシュ

GitHubでリポジトリを作成したら、以下のコマンドを実行してください：

```powershell
# リモートリポジトリを追加（YOUR_USERNAMEとYOUR_REPO_NAMEを実際の値に置き換えてください）
git remote add origin https://github.com/YOUR_USERNAME/YOUR_REPO_NAME.git

# ブランチ名をmainに変更（GitHubのデフォルトに合わせる）
git branch -M main

# リモートリポジトリにプッシュ
git push -u origin main
```

## 代替方法：GitHub CLIを使用する場合

GitHub CLIをインストールして使用する場合：

1. GitHub CLIをインストール: https://cli.github.com/
2. 認証: `gh auth login`
3. リポジトリを作成: `gh repo create hp --public --source=. --remote=origin --push`

