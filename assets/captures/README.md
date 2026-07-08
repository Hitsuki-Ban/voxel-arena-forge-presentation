# プレゼン用キャプチャ

このディレクトリは `pnpm presentation:captures` が生成するプレゼン用の静止画、短い MP4 ループ、manifest を置く場所です。コマンドは保存済みサンプルリプレイだけを読み込み、DeepSeek API は呼び出しません。

MP4 の生成には `ffmpeg` が必要です。個別のリプレイだけを撮る場合は `pnpm presentation:captures -- --sample-replay storm-lancer-phalanx` のように指定します。

既定では `camera=showcase` と `mode=embed` を使い、キャンバスを viewport 全体で描画します。見せ場を固定したい場合は `--time-seconds`、余白やズームを調整したい場合は `--capture-margin` / `--capture-scale` を指定します。
