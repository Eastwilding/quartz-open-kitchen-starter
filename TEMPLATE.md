# Variation A: Minimal Garden（最小の庭）

## 狙い

フォルダを少なく保ち、Quartzの標準的な使い方に一番近い形。まず全体像をつかむための基準案。

## ファイル構造

```text
content/
  index.md
  notes/sample-note.md
  projects/sample-project.md
```

## Quartz設定のメモ（実装時に反映する）

- ExplicitPublish を使う（publish: true のものだけ公開）
- フォルダは notes / projects の2つから始める
- グラフやタグは後で必要になってから足す
- publishAssets は referenced（公開ページが参照する添付だけ出す）
- locale は ja-JP を想定
- Cloudflare Pages の build は `npx quartz plugin install && npx quartz build`、output は `public` を想定

## 置いていないもの

- ブログ本文
- 小説の本文や素材
- 個人的なメモ

このブランチは、12月20日に一緒に実装する前の「型」の比較用です。
