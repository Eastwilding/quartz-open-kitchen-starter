# Variation B: Open Kitchen（開放キッチン型）

## 狙い

完成品、道具、制作途中、メモを分ける本命寄りの形。進一の構想（作品／コード／開放キッチン／研究メモ／について）に一番近い。

## ファイル構造

```text
content/
  index.md
  works/sample-work.md
  code/sample-tool.md
  kitchen/sample-seed.md
  notes/sample-note.md
  about.md
```

## Quartz設定のメモ（実装時に反映する）

- ExplicitPublish を使う（publish: true のものだけ公開）
- kitchen は「制作中」と分かるページだけを置く前提にする
- 公開しない素材は publish を付けず、公開用リポジトリへ送らない
- publishAssets は referenced（公開ページが参照する添付だけ出す）
- locale は ja-JP を想定
- Cloudflare Pages の build は `npx quartz plugin install && npx quartz build`、output は `public` を想定

## 置いていないもの

- ブログ本文
- 小説の本文や素材
- 個人的なメモ

このブランチは、12月20日に一緒に実装する前の「型」の比較用です。
