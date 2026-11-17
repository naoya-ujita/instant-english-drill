# 瞬間英作文ドリル（単独 URL 版）

ホーム画面に置いてアイコンのバッジ（今日あと N 個）を出すための配信用リポジトリです。
中身は `naoya-ujita/greeting-tool-practice` の `instant_english/` から
`build_site.py` で書き出したもので、ここでは編集しません。

- 公開先: https://naoya-ujita.github.io/instant-english-drill/
- `index.html` … アプリ本体（ホーム画面アプリ用の meta と manifest を追加済み）
- `seed.js` … 書き出した時点の記録。端末にまだ記録がないときの初期値になる
- `manifest.webmanifest`, `icon-*.png`, `apple-touch-icon.png` … ホーム画面用
- 配信は `gh-pages` ブランチから（GitHub Pages の自動有効化）。更新は main を push したあと `git push origin main:gh-pages`

記録はこの端末（ホーム画面アプリ）の中に保存されます。claude.ai のアーティファクト版とは同期しません。

## vocab-hacker/（Vocab Hacker 単独 URL 版）

- 公開先: https://naoya-ujita.github.io/instant-english-drill/vocab-hacker/
- 中身は `naoya-ujita/greeting-tool-practice` の `vocab-hacker/` の書き出し。`index.html` の本体スクリプトの直前に `seed.js` を読み込む行を足してある
- `seed.js` … 書き出した時点の学習記録（claude.ai 版のクラウド記録）。端末に記録がないときだけ初期値として取り込む
- `manifest.webmanifest`, `sw.js`, `icon-*.png` … ホーム画面用
- 更新は `vocab-hacker/` を差し替えて main を push したあと `git push origin main:gh-pages`
