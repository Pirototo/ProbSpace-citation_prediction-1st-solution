# ProbSpace-論文の被引用数予測-1st-solution
解説はprobspaceの以下のトピックに載せてます。

全てGoogle Colaboratoryで行いました。

## 流れ

1. 特徴量作成<br>
   text系の特徴をfeature_engineeringディレクトリ配下で作成しています。<br>
   **make-clean-title-abstract.ipynb**　を最初に使用しテキストの前処理をします。<br>
   それ以降はfeature_engineeringディレクトリ配下の他のnotebookを使用すればtext系の特徴量を作れます。

   scibertは　
   https://github.com/allenai/scibert<br>
   のPyTorch HuggingFace Modelsのscibert-scivocab-uncasedを使いました。

2. 学習<br>
   citation-prediction-rotto_category_to_nan_v5.ipynb　でtext系以外の特徴量を生成、学習を行いました。
3. アンサンブル<br>
   citation_ensemble_category_to_nan_v2.ipynb　でアンサンブルしています。
