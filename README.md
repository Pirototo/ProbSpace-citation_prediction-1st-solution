# ProbSpace-論文の被引用数予測-1st-solution
解説はprobspaceの以下のトピックに載せてます。

text系の特徴をfeature_engineeringディレクトリ配下で作成しています。 <br>
**make-clean-title-abstract.ipynb**　を最初に使用しテキストの前処理したdataframeをfeather形式で保存しています。
それ以降はfeature_engineeringディレクトリ配下の他のnotebookを使用すればtext系の特徴量を作れます。

scibertは　https://github.com/allenai/scibert　の　https://s3-us-west-2.amazonaws.com/ai2-s2-research/scibert/huggingface_pytorch/scibert_scivocab_uncased.tar　を使いました。
