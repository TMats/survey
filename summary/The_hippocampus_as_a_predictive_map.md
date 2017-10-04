# The hippocampus as a predictive map

## 1. どんなもの？
- 強化学習における予測機能の定式化と海馬が適応行動を支える新たな見方の提供
- 海馬の認知地図は場所そのものをエンコードするのではなく，現在の状態が与えられた時の将来の状態を予測をエンコードしていると主張
  - successor representation(SR)
  - 各ニューロンは環境の可能な状態をエンコードしている
  - 次の状態s'をエンコードするニューロンの発火率は現在の状態s・policyにおいてs'を訪問する割引期待回数に比例する

## 2. 先行研究と比べてどこがすごい？
- SRはモデルフリーとモデルベースの中間的立ち位置をしめる
  - 価値関数を予測の表現と報酬の表現に分けることで，報酬が変化した時にも価値を柔軟に再計算できるようになる
  - 文脈効果には事前に状況に遭遇することで海馬が文脈の予測的な表現を獲得し，その後の学習が空間を早く伝播するという解釈を与える

## 3. 技術や手法のキモはどこ？
- SRは価値関数の定義から自然に生まれる
  - 価値関数は報酬関数と状態の予測的表現の内積として表現できる
  - SRはその状態から始まる軌道の期待discount future occupancy をエンコードする
  - SRの推定は逐次的にTD学習すれば更新できる
<img width="680" alt="2017-10-04 14 26 33" src="https://user-images.githubusercontent.com/16148653/31161138-1cf60b3a-a910-11e7-9d04-aa235f5cce9d.png">
<img width="678" alt="2017-10-04 14 30 50" src="https://user-images.githubusercontent.com/16148653/31161242-a8081b96-a910-11e7-8b7a-cebeaf11ca41.png">

## 4. どうやって有効だと検証した？


## 5. 議論はある？


## 6. 次に読むべき論文は？
- Improving Generalisation for Temporal Difference Learning: The Successor Representation #69
  - http://www.gatsby.ucl.ac.uk/~dayan/papers/d93b.pdf
  - successor representation(SR)
- Deep Predictive Coding Networks for Video Prediction and Unsupervised Learning #61
  - https://arxiv.org/abs/1605.08104
  - prednet

## 7. メモ


## 書誌情報
