# K-means
クラスタリングの一種でデータ分析において広く活用されている<br>

## 概要
- 代表的なクラスタリングの方法の一つ
  - クラスタリング (clustering) とは，分類対象の集合を，内的結合 (internal cohesion) と外的分離 (external isolation) が達成されるような部分集合に分割すること([参考](http://www.kamishima.net/jp/clustering/))
- データの各クラスタの重心距離を計算する
- 最も近いクラスタの重心を求めることで決まる<br>

## アルゴリズム
1. データの点の中から、適当な点をクラスタ数だけ選びそれらを重心とする
  - 1のクラスタ数はハイパーパラメータであるため自分で設定する必要がある
  - ハイパーパラメータとは、機械学習アルゴリズムの挙動を制御するパラメータのこと
2. データ点と各重心の距離を計算し、最も近い重心をそのデータ点の所属するクラスタとする
3. クラスタごとにデータ点の平均値を計算し、それらを新しい重心とする
4. 2,3を繰り返し実行し、全てのデータ点が所属するクラスタが変化しなくなるか計算ステップ数の上限に達するまで計算を続ける
  - 重心の決め方によっては学習がうまく進まないことがある
  - k-means++をいう手法でなるべく離れた重心を初期値として選ぶことができる
<br>

## その他
- クラスタリング結果の評価方法は**クラスタ内平方和**を計算することで定量的に評価することができる
  - 値が小さい方が良いクラスタリング
- クラスタ数の推定するのが難しい場合はElbow法などでクラスタ数の推定をすることができる