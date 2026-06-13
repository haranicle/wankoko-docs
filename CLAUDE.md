# ワンココ ドキュメント

ワンココアプリの利用規約・プライバシーポリシーを GitHub Pages として公開するリポジトリ。

## 公開 URL

| ページ | URL |
|---|---|
| トップ | https://haranicle.github.io/wankoko-docs/ |
| 利用規約 | https://haranicle.github.io/wankoko-docs/terms-of-service |
| プライバシーポリシー | https://haranicle.github.io/wankoko-docs/privacy-policy |

## Git 運用

- `main` ブランチへの直接 push は禁止。必ずフィーチャーブランチを切って PR を作成する
- GitHub Pages は main ブランチのルートから自動ビルドされる

## バージョン管理

各ドキュメントのバージョンはコミット ID で管理する。ページ上に表示されるバージョンは GitHub Pages のビルド時に `site.github.build_revision`（先頭7文字）が自動的に埋め込まれる。

## ドキュメントの更新手順

1. `terms-of-service.md` または `privacy-policy.md` を編集する
2. フィーチャーブランチを切ってコミット＆プッシュし、PR を作成する
3. **main へマージする前に** 以下を確認する
   - `terms-of-service.md` の `## 附則` にある施行日が **今日の日付** になっているか
   - `privacy-policy.md` の `## 附則` にある施行日が **今日の日付** になっているか
4. 確認が取れたら main にマージする
5. GitHub Pages が自動的にビルド・公開される（通常1〜2分）

## ファイル構成

| ファイル | 説明 |
|---|---|
| `_config.yml` | Jekyll 設定（テーマ・サイト情報） |
| `index.md` | トップページ |
| `terms-of-service.md` | 利用規約 |
| `privacy-policy.md` | プライバシーポリシー |
