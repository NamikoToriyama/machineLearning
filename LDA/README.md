# LDA
次元削減の手法の1つで文書のモデル化に適した手法<br>

## 概要
- 自然言語処理などに利用されている手法
- トピックという単語に関する確率分布と単語分布を利用して文書データを生成する
- 文書内の単語はトピック分布によってトピックが割り当てられ
- そのあとトピックが持つ単語分布に従って選ばれる<br>

## アルゴリズム
1. 各文書の単語についてランダムにトピックを割り当てる
2. 単語に割り当てられたトピックから文書ごとのトピック確率を計算する
3. 単語に割り当てられたトピックからトピックごとの単語確率を計算する
4. 2と3の積で計算される確率を元に、各文書の単語にトピックを再び割り当てる
  - 同じ文書内では特定のトピックが選ばれやすくなる
5. 2,3,4を収束条件まで繰り返す
