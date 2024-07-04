# 修了要件の詳細

## 開発のステップと要件を確認
- 自身の課題設定をもとに一連の開発を実践する:
  1. データの収集と前処理
  2. モデルの学習
  3. APIの作成
  4. フロントエンド部分の作成【ステップアップ】
  5. Web上に公開（デプロイ）【ステップアップ】
- 使用するデータは、テーブルデータ、画像データ、自然言語データのいずれでもOK
- 機械学習モデルについては、学習済みモデルを使用してOK
- 外部で作成された API (例: [OpenAI API](https://openai.com/index/openai-api/) etc.) を利用するだけではNG

## 要件達成に必要な技術要素
### 1. データ収集・前処理【必須】
- 自分で作成（撮影）
- 公開データを利用
- スクレイピング（例: [Beautiful Soup](https://www.crummy.com/software/BeautifulSoup/)）
- アノテーション（ラベル付け）

### 2. 機械学習モデル作成【必須】
- Google Colabなどでnotebookを実行
- 学習済みモデルをファイル保存

### 3. FastAPIの実装【必須】
- 学習済みモデルを読み込み、推論のみ行う
- ここまでで要件クリア！

![01_FastAPI](./images/01_FastAPI.svg)

### 4. フロントエンドの実装【ステップアップ】
- APIだけでは物足りないので、ほとんどの方はフロントエンドまで作成します
- [Streamlit](https://streamlit.io/) がおすすめ
- FastAPIとの接続
  - `requests.psot()`

![02_Streamlit](./images/02_Streamlit.svg)

### 5. デプロイ【ステップアップ】
Web上に公開して他ユーザーも使えるようにすること。

無料で使えるデプロイ先の例:
- [Streamlit Cloud](https://streamlit.io/cloud)
- [Render](https://render.com/)

![03_Deployment](./images/03_Deployment.svg)

[▲TOP PAGE](./README.md)

2024@rockyhg (Hiroki Haga)
