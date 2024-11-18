## LMSYS-Chatbot Arena Human Preference Predictions![image](https://github.com/user-attachments/assets/231d312c-60ba-42d8-9ea4-0de804ab4df3)


このプロジェクトは、Kaggleで開催された「LMSYS Chatbot Arena Human Preference Predictions」コンペティションへの参加記録です。大規模言語モデル（LLM）の回答に対する人間の選好を予測するAIモデルを開発しました。

## コンペティション概要

- **目的**: 2つのLLMの回答から人間が好む方を予測するモデルの開発
- **期間**: 2024-05-03 ~ 2024-08-13 
- **主催**: LMSYS Org

## データセット
- **ソース**: [Chatbot Arena プラットフォーム](https://lmarena.ai/)
- **形式**:  
  ユーザーがランダムな2つのLLMの回答のどちらかを選好することで相対的なモデルの評価を下す（引き分けも含む）  
  集積した過去データ（ユーザーのprompt、モデルの回答×2、ユーザーの選考結果）を利用
![image](https://github.com/user-attachments/assets/337d1d20-c483-4fdd-b939-d28f19e320c4)
[引用元](https://www.kaggle.com/code/abaojiang/lmsys-detailed-eda)

- **サイズ**: 訓練データ(57477, 9) / テストデータ(3, 4)  
※未公開テストデータは明記なし。
## 評価指標
- [対数損失関数](https://ja.wikipedia.org/wiki/%E4%BA%A4%E5%B7%AE%E3%82%A8%E3%83%B3%E3%83%88%E3%83%AD%E3%83%94%E3%83%BC)を利用
  
  
## チャレンジポイント
1. 大規模言語モデルのFine-tuningの実装
2. データの前処理（クリーニング、テキストの修正など）のトライ＆エラー
3. Kaggle環境での使用メモリ・時間制限とコスト面の制限下での効率的なモデル訓練と推論の処理を構築
  

## 主な成果
- 最終順位: 87/ 1849チーム（銀メダル）
- 公開リーダーボードスコア: [0.99298]
- 私的リーダーボードスコア: [0.88562]  

※本コンペでは、データリークに対応するため最終提出後に評価用データの入れ替えが行われました。
  

## 技術スタック
- 言語: Python 3.8
- 主要ライブラリ: PyTorch, Transformers, Scikit-learn, Numpy, Pandas
- モデル: [Gemma2, Llama3, Llama3.1,(LightGBM)]
- 環境: Google Colab, Kaggle Notebooks
