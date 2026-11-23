# Variation C: One Page Lite（1ページ軽量型）

## 狙い

最初は名刺ページだけに絞る形。ファイル数が最小で、公開までの距離が一番短い。庭らしくなるのは後からでもよい、という案。

## ファイル構造

```text
content/
  index.md
  about.md
```

## Quartz設定のメモ（実装時に反映する）

- ExplicitPublish を使う（publish: true のものだけ公開）
- 最初は index と about だけにする
- グラフ、タグ、フォルダ一覧は最初は使わない前提で設計する
- publishAssets は referenced（公開ページが参照する添付だけ出す）
- locale は ja-JP を想定
- Cloudflare Pages の build は `npx quartz plugin install && npx quartz build`、output は `public` を想定

## 置いていないもの

- ブログ本文
- 小説の本文や素材
- 個人的なメモ

このブランチは、12月20日に一緒に実装する前の「型」の比較用です。
