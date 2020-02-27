# Neural Network
生物の神経回路網を模倣することから始まったとされる。回帰、分類どちらにもよく使われる。<br>
ディープラーニングはニューラルネットワークの応用。<br>
<br>

## 概要
入力層と出力層の間に**中間層**を挟むことで複雑な決定境界を学習できるモデル。<br>
中間層は入力層からシグモイド関数などの非線形関数を用いて計算される。<br>
中間層の次元はハイパーパラメータである。ちなみにハイパーパラメータ（英語: Hyperparameter）とは、推論や予測の枠組みの中で決定されないパラメータのことを指す。損失関数の正則化項の影響度を表す係数などが該当する。(wikipedia)

## アルゴリズム
### 単純パーセプトロン
特徴量に重みをかけた結果に、非線形な関数を適用して識別を行うモデルのこと。<br>
入力となる特徴量を活性化関数にかけて確率yを出力する。<br>
※単純パーセプトロンはロジスティック回帰とよく似た性質をもつ。

### ニューラルネットワーク
単純パーセプトロンを積み重ねることで複雑な決定境界を表現できるようにしたモデル。<br>
単純パーセプトロンでは線形分離可能な問題でないと解くことができない。<br>
こう言った問題を解けるように中間層に分離し重ね合わせて出力層に出力を行う。<br><br>

### アーリーストリッピング
過学習になる前に学習を打ち切って、過学習を防ぐもの。<br>
学習の最中に評価データなどを用いて損失などの評価指標を逐次記録しておき、損失度合いがわかるようにする。<br>
過学習の傾向が見え始めたら学習を打ち切るようにする。<br>