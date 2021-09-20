# Jリーグの観客動員数予測

経過発表段階のソースコードです。

その後改善したものは現時点で非公開（公開日未定）

## Result

![rank](https://user-images.githubusercontent.com/73447865/134067951-85b3b19f-e327-4fdf-853a-00ee5bbbf7d1.png)

## NoteBook 目次

### Preparation
- Google Drive に接続
- Import Libraries
- Helper functions
- Base Model
### Prepare Data
- Load
- Concatenate
  - 追加データの結合
  - 学習用・テスト用データの結合
### Visualization
- 基本統計量
- グラフ化
### Preprocessing
- Cleansing / Feature Engineering
  - 学習用・テスト用データに対する処理
    - 不要列の削除準備
    - match列（開催節）の処理
    - gameday列（試合日）の処理
    - time列（キックオフ時間）の処理
    - tv列（TV放送）の処理
    - home, away列（ホーム/アウェイチーム名）の処理
    - 他の文字型の列
  - 付加情報データに対する処理
    -不要列の削除準備
    - weather列（天候）の処理
    - humidity列（湿度）の処理
    - address列（所在地）の処理
    - 他の文字型の列
  - 追加データに対する処理
    - 不要列の削除準備
    - 県名列の処理
    - 経営情報の年列の処理
    - クラブ名の処理
    - 昇降格列の処理
  - 特徴量生成
    - 数値データの組み合わせ
    - カテゴリデータの組み合わせ
    - ターゲットエンコーディング
    - スタジアムの収容率
    - チーム成績テーブル
