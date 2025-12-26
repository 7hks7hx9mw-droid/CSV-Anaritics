# CSV Sales Analytics & AI Report Generator

## 概要

本プロジェクトは、複数の CSV 売上データをもとに、

- 売上集計・分析
- 商品別売上グラフの生成
- 月次売上推移グラフの生成
- PDF レポートの自動作成
- AI による「月次売上推移」の文章生成

を **一括で自動化する Python スクリプト**です。

データ分析結果を  
**「数値・グラフ・文章」まで含めた業務レポート形式**で出力することを目的としています。

---

## 主な機能

- CSV ファイルの一括読み込み
- 総売上・平均注文単価・顧客数の集計
- 商品別売上の棒グラフ生成（PNG）
- 月次売上推移の折れ線グラフ生成（PNG）
- PDF レポートの自動生成
- OpenAI API を用いた売上傾向コメントの自動生成
- 最終的な分析レポート（テキスト）の出力

---

## ディレクトリ構成

```text
project/
├── main.py                # 本スクリプト
├── csv_files/             # 入力CSVファイル
│   ├── sales_01.csv
│   └── sales_02.csv
├── csv_png/               # グラフ画像出力先
│   ├── *_product_sales.png
│   └── monthly_sales_trend.png
└── csv_pdf/               # レポート出力先
    ├── *_report.pdf
    └── analysis_report.txt
