# エンジニアタイプ診断

12問の二択に答えると、4つの軸から開発スタイルを16タイプに分類する診断アプリです。

| 軸 | 左 | 右 |
|---|---|---|
| 進め方 | **E** 探索 | **P** 設計 |
| 関心 | **U** ユーザー | **S** システム |
| 働き方 | **A** ソロ | **T** チーム |
| 技術観 | **N** 新技術 | **R** 枯れた技術 |

## ローカルで確認する

ビルドは不要です。`index.html` 1ファイルで動きます。

```sh
git clone https://github.com/taboki1100/engineer-type.git
cd engineer-type
open index.html          # macOS（Windows は start index.html）
```

ローカルサーバーで見たい場合:

```sh
npx serve .              # または python3 -m http.server 8000
```

## 構成

- `index.html` … 画面・質問データ・タイプ説明・判定ロジックをすべて含む
  - 質問は `QS`、タイプ説明は `T`、軸の定義は `AX` に入っています
