# kaggle-LMSYS-Chatbot Arena Human Preference Predictions

## LMSYS-Chatbot Arena Human Preference Predictions

- コンペの目的
  任意の2つの大規模言語モデル（LLM）の回答から人間が好む回答を予測するタスク。
  ※明記されてはいませんが、LLM強化学習用の報酬モデル作成が主なメリットとして挙げられると推察されます。
  
- データについて
  [Chatbot Arena](https://lmarena.ai/)という、公開済みの様々なLLMの中でランダムに選ばれた2つのモデルのどちらかの回答をユーザーが選好することで相対的なモデルの評価を下すプラットフォームにおける過去のデータ（ユーザーのprompt、モデルの回答×2、ユーザーの選考（または引き分け）結果）を利用。
  ![image](https://github.com/user-attachments/assets/337d1d20-c483-4fdd-b939-d28f19e320c4)
  [引用元](https://www.kaggle.com/code/abaojiang/lmsys-detailed-eda)
