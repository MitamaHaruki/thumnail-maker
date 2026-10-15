# thumnail-maker
サムネイルメーカー配布用

## ダウンロード

[最新版のページ](https://github.com/MitamaHaruki/thumnail-maker/releases/latest)から `ThumbnailMaker-Setup-<版>.exe` をダウンロードして実行してください（Windows 10 / 11、64bit）。

- 署名なしのため、初回は Windows SmartScreen の警告が出ることがあります（「詳細情報」→「実行」）。
- 1.2.0 以降は、起動時に新しい版がないか確認します。ヘルプ →「更新を確認」からも確認できます。

## リリースの作り方（管理用）

`release-upload` ブランチに次のファイルを置いて push すると、GitHub Actions が `v<版>` のリリースを作ります（`.github/workflows/publish-release.yml`）。

- `upload/version.txt`：版（例：`1.2.0`）
- `upload/notes.md`：リリースの説明（アプリの更新のお知らせにも表示されます）
- `upload/ThumbnailMaker-Setup-<版>.exe`：インストーラー
