# t-SNE(t-Distributed Stochastic Neighbor Embedding)
高次元の複雑なデータを２次元または３次元に次元削減する手法で、低次元空間の可視化に利用される<br>

## 概要
- 多様体学習の一種であり、複雑なデータの可視化を目的として利用される手法
- 高次元のデータを二次元、または三次元に削減する(これはLLEも一緒)
- 次元削減する際に自由度1のt分布を利用しているのが特徴

## アルゴリズム
1. 全ての組i,jについてxi,xjの類似度をガウス分布を利用した類似度で表す
  - 確率分布を利用して類似度を求める
  - データ間の距離が近いほど類似度が大きい
  - 類似度はt分布を利用している
2. xiと同じ数の点yiを低次元空間にランダムに配置し、全ての組i,jについて、yi, yjの類似度をt分布を利用した類似度で表す
3. 1と2から定義される類似度分布がなるべく同じになるように、データ点yiを更新していく
4. 収束条件まで3を繰り返す

t分布の性質上高次元空間では中心から離れた部分が影響し局地的な情報を保持できなくなる。そのため４次元以上の空間への削減はうまくいかないことがある。<br>

## その他
- 手書き数字の画像についてはt-SNEが一番うまく分類することができる
- 次元削減についてはデータによって一長一短なのでデータにあった次元削減を行うことが好ましい
