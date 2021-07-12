# Image-recognition-of-fashion-items-implemented-in-Tensorflow
Tensorflowを用いて、ファッションアイテムの画像認識を行いました。公式のチュートリアルではSequentialモデルの書き方を使って書いていたので、
TensorFlowスタイルで構築してみました。  

構成は簡単なもので、入力層と出力層の間に全結合層（Dense）を2つ入れた構成になっています。
epoch数を100として学習を行いましたが、GPUを使っていないため10数分かかってしまいました。  

【考察】
epoch数が増えるにつれて、Trainingの精度は上がっていますが、Validationの精度は横ばいになっています。これはオーバーフィッティングが起きていると考えられるので、ドロップアウトを配置することが良い改善案になると考えられます。

【感想】
Kerasを用いたSequential記法よりも複雑に設定する必要があり、難しかったです。




***
.ipynbファイルが開かれない時は、こちらのリンクにURLを貼ってご覧になってください。  
[nbviewer](https://nbviewer.jupyter.org/)
