# 三鷹市スキー連盟 Web（website）

GitHub Pages ＋ Jekyll（minima）で公開する公式サイトの本体リポジトリーです。

## プレビュー URL

https://mitaka-ski.github.io/website/

## 更新手順

1. Markdown（`.md`）を編集する
2. commit して `main` に push する
3. 数分待つと Pages に反映される

お知らせは `_posts/` に `YYYY-MM-DD-title.md` を追加する。ホームには直近最大5件が表示される。

## プラグイン・クロール補助（GitHub Pages 対応）

- `jekyll-feed` / `jekyll-seo-tag` / **`jekyll-sitemap`**
- サイトマップ: ビルド後に `/sitemap.xml`（preview では `/website/sitemap.xml`）
- **`robots.txt`**: 全許可＋上記 Sitemap を明示（`url` / `baseurl` に追従）

## 注意

- 秘密情報・Joomlaバックアップ本体はコミットしない
- 本番で独自ドメインを使うときは `_config.yml` の `baseurl` を `""` に変更する
- カスタムドメイン設定はこのリポジトリー（`website`）のみに行う

運用アカウント: `mitaka-ski-web` ／ Organization: `mitaka-ski`
