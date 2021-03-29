# ProbSpace-論文の被引用数予測-1st-solution
解説はprobspaceの以下のトピックに載せてます。

全てGoogle Colaboratoryで行いました。

## 流れ

1. 特徴量作成
   text系の特徴をfeature_engineeringディレクトリ配下で作成しています。 <br>
   **make-clean-title-abstract.ipynb**　を最初に使用しテキストの前処理したdataframeをfeather形式で保存しています。
   それ以降はfeature_engineeringディレクトリ配下の他のnotebookを使用すればtext系の特徴量を作れます。

   scibertは　
   https://github.com/allenai/scibert<br>
   のPyTorch HuggingFace Modelsのscibert-scivocab-uncasedを使いました。

2. 学習
   citation-prediction-rotto_category_to_nan_v5.ipynb
3. アンサンブル
   citation_ensemble_category_to_nan_v2.ipynbでアンサンブルしています。
