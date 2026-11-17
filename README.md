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
