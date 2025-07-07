# Misaki Section 6

1. GitHub にリポジトリを作成する
2. ローカルにクローンする

```bash
git clone https://github.com/ユーザー名/リポジトリ名.git
cd リポジトリ名　//クローンしたディレクトリに移動
```

3. ブランチを作成する　`feature/機能名を入れる`

```bash
   git checkout -b feature/code-fix
```

4. ファイル作成しコード訂正しコード訂正
5. ESLint を導入
6. 変更内容をコミットし、GitHub に反映

```bash
git add .
git commit -m "コードを訂正"
git push origin feature/code-fix　//ブランチ名
```

7. GitHub 上でプルリクエストを作成し、マージ

- マージ完了後のローカル作業

```bash
# main（または develop）に戻る
git checkout main

# 最新の状態を取得
git pull origin main

# 不要になったブランチは削除
git branch -d feature/code-fix
git push origin --delete feature/code-fix

```
