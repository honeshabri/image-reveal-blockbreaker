# 画像明かしブロック崩し (Image Reveal Block Breaker)

2枚の画像を使ったブロック崩しゲームです。最初は1枚目の画像がブロックとして表示され、ブロックを崩していくと下の画像が徐々に現れる仕組みになっています。

## 特徴

- 2枚の固定画像を使ったブロック崩しゲーム
- 最初の画像がブロックとして表示され、崩すと下の画像が見えてくる
- 画像を損なわずに全体を表示、下部にプレイエリア
- スマートフォンでのタッチ操作とPCでのマウス操作に両対応
- スコア表示と残りライフ表示機能

## 遊び方

1. 「ゲームスタート」ボタンを押す
2. パドルを左右に動かしてボールを跳ね返す
3. ボールでブロックを崩していく
4. すべてのブロックを崩すとゲームクリア！
5. ボールを落とすとライフが減少（3回で終了）

## 操作方法

- **スマートフォン**: 画面をスワイプしてパドルを動かす
- **PC**: マウスを左右に動かしてパドルを操作

## カスタマイズ方法

コード内の次の変数を変更することで、ゲームの難易度や見た目を調整できます：

```javascript
// 使用する画像のURL（自分のユーザー名に変更してください）
const frontImageUrl = "https://raw.githubusercontent.com/honeshabri/image-reveal-blockbreaker/main/front.jpg";
const backImageUrl = "https://raw.githubusercontent.com/honeshabri/image-reveal-blockbreaker/main/back.jpg";

// ブロックの行数と列数
gameState.blockRows = 5;
gameState.blockColumns = 10;

// ボールの速度
gameState.ball.speed = 5;

// パドルの大きさ
gameState.paddle.width = width * 0.15; // 画面幅の15%

// 下部プレイエリアの色
ctx.fillStyle = '#333366'; // 濃い青系の色
```

## 技術的詳細

- 純粋なJavaScript、HTML5 Canvas、CSSで実装
- 外部ライブラリを使用していないため軽量
- レスポンシブデザインで様々な画面サイズに対応
- 画像のアスペクト比を維持しながら表示サイズを調整

## ライセンス

MIT License
