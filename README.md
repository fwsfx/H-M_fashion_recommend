## H&M カスタマー商品レコメンデーションコンペ向けの作業ディレクトリ

### 作業環境
- python 3.9.6: まず[pythonのofficial site](https://www.python.org/downloads/)で3.9.6バージョンをダウンロード、インストルールし、[このマニュアル](https://qiita.com/fiftystorm36/items/b2fd47cf32c7694adc2e)にしたがって、仮想環境を作成する
- モジュール・ライブラリーなど：```requirements.txt```の中身を```'python3 -m pip install -r requirements.txt'```の実行によってインストールする

### ディレクトリ構造
```
h&m_personalized_fashion_recommendations
  ├data
      ├images
          ├010
          ├011
          ...
      ├articles.csv
      ├customers.csv
      ├transactions_train.csv
      ├sample_submission.csv
  ├notebook
      ├eda
      ├poc
  ├output
  ├src
  ├requirements.txt
```

### フォルダ概要
- data  
  ```images```:商品アイテムの写真  
  ```articles.csv```:商品アイテムの属性  
  ```customers.csv```:消費者の属性  
  ```transactions_train.csv```:消費者の過去の商品購買経歴情報(訓練データ)  
  ```sample_submission.csv```:提出データの形
- notebook  
  ```eda```:探索的分析のコード  
  ```poc```:サンプルコードやちょっと複雑なことを実行できるかを試す場所
- output  
  予測結果を出力する場所
- src  
  .pyファイルなどのソースコードを配置する場所