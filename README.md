# quartz-open-kitchen-starter

## Variation C: One Page Lite（1ページ軽量型）

Obsidian の Vault を「開放キッチン」的な個人サイトとして公開するための、Quartz 5 + Cloudflare Pages のスターターです。

このブランチは、比較用のテンプレート案です。ブログ本文や個人コンテンツは入れていません。置いてあるのは、構造を見るための最小限のプレースホルダーだけです。

## この案の考え方

最初は名刺ページだけに絞る形。ファイル数が最小で、公開までの距離が一番短い。庭らしくなるのは後からでもよい、という案。

## 構成

- 静的サイト生成: Quartz 5
- コンテンツ: Obsidian Vault（Markdown）
- ホスティング: Cloudflare Pages
- 公開範囲: frontmatter に `publish: true` と書いたノートだけを公開（ExplicitPublish）

詳しくは `TEMPLATE.md` を見てください。
