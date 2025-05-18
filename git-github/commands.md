# Git & GitHub 基本コマンドまとめ

## 🔧 Git 初期設定（最初に1回だけやる）

```bash
git config --global user.name "Your Name"
git config --global user.email "you@example.com"

git init                       # Gitを初期化
git add .                     # すべての変更をステージに追加
git commit -m "初回コミット"  # コメント付きでコミット
git branch -M main            # ブランチ名をmainに変更（初回のみ）
git remote add origin <URL>  # GitHubのリモートURLを追加
git push -u origin main       # 最初のプッシュ

git status          # 現在の変更を確認
git add ファイル名  # 変更をステージに追加
git commit -m "説明" # コミット
git push            # GitHubにプッシュ

git log             # コミット履歴を見る
git diff            # 変更差分を見る
git restore ファイル名    # 編集前に戻す
git rm --cached ファイル名 # ステージから外す（消さずに）

git pull            # GitHubの最新を取得してマージ

git branch ブランチ名       # 新しいブランチを作る
git checkout ブランチ名     # ブランチを切り替える
git checkout -b ブランチ名  # 作って切り替える（よく使う）


---

## ✅ 作成コマンド（ターミナル）

```bash
mkdir git-github
touch git-github/{commands.md,common-errors.md,README.md}
