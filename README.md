# 更新手順

1. 作業用ブランチを切ってMarkdown（`.md`）を編集する
2. commitしてそのブランチへpushする
3. Pull Requestを作り、approveされたら`main`へmergeする
4. 数分待つとhttps://mitaka-ski.com/に反映される

お知らせは`_posts/`に`YYYY-MM-DD-タイトル.md`を追加する。ホームには直近最大5件が表示される。

## 未来日付のお知らせ（予定日公開）

`date` を未来にすると、その日時より前のビルドではサイトに出ない（Jekyll 既定）。

掲載予定日に GitHub Actions（`.github/workflows/pages.yml`）が正午・23時（JST）に再ビルドする。出ない場合は Actions タブから「Deploy Jekyll site to Pages」を手動実行（`workflow_dispatch`）する。
