# MATH LOG

Collaborative Mathematics Learning Log — クラスを越えて学習を記録・共有するWebアプリ。

## Features
- 学習記録の投稿（日付・分数・内容・ひとこと）
- みんなの記録一覧
- 学習時間ランキング
- スマートフォン / タブレット / PC対応
- Supabase接続前はブラウザ内だけで動くデモモード

## GitHub Pages
Repository Settings → Pages → Deploy from a branch → `main` / `/(root)` を選択して保存。

公開URL: https://tyonntindayon.github.io/math-log-connect/

## 共有機能を有効にする（Supabase）
1. Supabaseで新しいプロジェクトを作成。
2. SQL Editorで `supabase/schema.sql` の内容を実行。
3. Project Settings → API から Project URL と publishable/anon key を取得。
4. `index.html` 内の `SUPABASE_URL` と `SUPABASE_ANON_KEY` に設定。
5. GitHubへpushし、Pagesの反映後に複数端末から投稿・閲覧できることをテスト。

**注意:** ブラウザに置くキーはpublishable/anon keyのみ。service_role keyや秘密鍵を絶対に公開しないこと。RLSを無効にしないこと。

## Privacy & safety
- ニックネームを使い、本名・学校名・連絡先・住所などを投稿しないでください。
- 現在のv1は公開読み取り・公開投稿のシンプルな構成です。投稿者本人確認や編集・削除機能はありません。
- 実際のクラスで広く使う前に、認証、投稿制限、管理者による通報・削除手段を追加してください。
- デモモードのデータは投稿した端末のブラウザにだけ保存され、他の人とは共有されません。

## Project structure
```
index.html
supabase/schema.sql
README.md
```
