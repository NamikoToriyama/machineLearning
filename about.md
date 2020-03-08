# 機械学習の概要
## 機械学習とは
与えられた問題や課題または環境に応じて、コンピュータ自身が学習をし学習結果を生かした問題解決などを行う仕組みのこと。

## 機械学習の種類
### 教師あり学習
問題の答えをコンピュータに与えることで学習させていく手法のこと。

### 教師あり学習の種類の分類
  * 分類問題
    * [ロジスティック回帰](https://github.com/NamikoToriyama/machineLearning/tree/master/LogisticRegression)
  * 回帰問題
    * [線形回帰](https://github.com/NamikoToriyama/machineLearning/tree/master/LinearRegression)
    * [正則化](https://github.com/NamikoToriyama/machineLearning/tree/master/Regularization)
  * どちらにも含まれる
    * [サポートベクターマシン](https://github.com/NamikoToriyama/machineLearning/tree/master/SupportVectorMachine)
    * [サポートベクターマシン(カーネル法)](https://github.com/NamikoToriyama/machineLearning/tree/master/SVM(kernel))
    * [ナイーブベイズ](https://github.com/NamikoToriyama/machineLearning/tree/master/NaiveBayes)
    * [ランダムフォレスト](https://github.com/NamikoToriyama/machineLearning/tree/master/RandomForest)
    * [ニューラルネットワーク](https://github.com/NamikoToriyama/machineLearning/tree/master/NeuralNetwork)
    * [KNN](https://github.com/NamikoToriyama/machineLearning/tree/master/kNN)

## 教師なし学習
特徴を表すデータを入力とし、そのデータを変換して別の形式で表現したり、データの中に部集合を見つけたりすることで入力データの構造を理解することができる。結果を解釈するために入力データの前提知識がある程度必要になる。

### 教師なし学習の種類の分類
  * 次元削減
    * [PCA](https://github.com/NamikoToriyama/machineLearning/tree/master/PCA)(主成分分析)
    * [LSA](https://github.com/NamikoToriyama/machineLearning/tree/master/LSA)(Latent Semantic Analysis)
    * [NMF](https://github.com/NamikoToriyama/machineLearning/tree/master/NMF)(Non-negative Matrix Factorization 非負値行列因子分解)
    * [LDA](https://github.com/NamikoToriyama/machineLearning/tree/master/LDA)(Latent Dirichlet Allocation 潜在ディリクレ配分法)
    * [LLE](https://github.com/NamikoToriyama/machineLearning/tree/master/LLE) (LocallyLinearEmbedding 次元圧縮)
    * [t-SNE](https://github.com/NamikoToriyama/machineLearning/tree/master/t-SNE)(t-Distributed Stochastic Neighbor Embedding)
  * クラスタリング
    * [k-means](https://github.com/NamikoToriyama/machineLearning/tree/master/k-means)
    * [混合ガウスモデル](https://github.com/NamikoToriyama/machineLearning/tree/master/GMM)

### 強化学習
ある行為に対する報酬を最大化するように行動していき、行為に対して最適解を学習していく学習。
