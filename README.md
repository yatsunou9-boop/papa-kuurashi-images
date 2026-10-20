# papa-kuurashi-images

Threads（@papa_kuurashi）の自動投稿で使うイラスト置き場です。
自動投稿の仕組みは `yatsunou9-boop/-` リポジトリの `threads-mcp/autopost/` にあります。

- `illustrations/` … 投稿に付けるイラスト（PNG か JPEG、8MB まで）
- `catalog.json` … イラストの一覧。自動投稿はここを見て、本文の場面に合う1枚を選ぶ

Threads はこのリポジトリの公開 URL（`raw.githubusercontent.com/.../main/...`）から画像を取りに来るので、
**リポジトリは公開のまま**にして、画像は **`main` ブランチ**に置いてください。

## イラストを足すとき

1. `illustrations/` に画像を置く（ファイル名は半角英数字・`_`・`-` だけ。例: `bath_time.png`）
2. `catalog.json` の `images` に1件足す

```json
{
  "file": "illustrations/bath_time.png",
  "scene": "どんな絵か（1文）",
  "fits": ["合う話題", "キーワード"],
  "times": ["朝", "昼", "夕方", "夜", "夜（遅め）"],
  "notes": "使うときの注意（なければ空文字）"
}
```

`times` は投稿枠の名前（朝・昼・夕方・夜・夜（遅め））です。

### 絵のルール
- いつもの3人（パパ・しましまパーカーの上の子・くま柄ロンパースの赤ちゃん）、やわらかいアニメ調の手描き風
- 文字は入れない（壁のカレンダー程度は可）
- 顔写真・実在の場所・個人が特定できるものは入れない
