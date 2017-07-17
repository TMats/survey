# Curiosity-driven Exploration by Self-supervised Prediction

## 1. どんなもの？
- 好奇心(curiosity)を「self-supervised inverse dynamics modelにより学習された画像特徴量空間で自身の行動の結果を予測したものと実際の画像の入力の差」として定義
  - 内的な報酬として扱う

## 2. 先行研究と比べてどこがすごい？
- 実世界の問題において外的な報酬が極端にスパースなことが多い
  - 基本的な強化学習手法だと偶然ゴールに到達しないと報酬がもらえず学習が進まない
  - 内的な報酬を用いて学習をはやく進ませる
- 従来の内的な報酬を用いる手法は大きく分けて2つ
  - エージェントに新規な状態を探索させるようにする
  - 自身の行動の結果の予測誤差を減らすように行動させる

## 3. 技術や手法のキモはどこ？
- 自身の行動の影響飲みを予測して，他を無視する
  - 生の感覚データ(pixel)をエージェントの行動に関係する情報が表現されている特徴空間に変換する
  
## 4. どうやって有効だと検証した？
- VizDoomでA3Cと比較
  - 内的な報酬がタスクを遂行するのに重要な役割をになっているとわかった
- スーパーマリオレベル1で外的な報酬がない条件で実験
  - 壁にぶつかったり，角で引っかかることのない行動を学習した
- 訓練した物理的環境によらない探索行動を学習
  - マリオの次のレベルのステージを早く探索できた
  - 違うテクスチャ・マップのVizDoomでも前の環境で学習した動き方を転移できた

## 5. 議論はある？
- モータレベルの方策である学習した探索行動を階層的なシステムのなかで利用することがfuture work
- 相互作用の機会も少ないシナリオではリプレイメモリを使うことも考えうるがこれもfuture work

## 6. 次に読むべき論文は？
- 逆運動学を特徴の学習や認識のタスクに利用するモデル
  - P. Agrawal, J. Carreira, J. Malik. Learning to See by Moving. arXiv. 2015.
    - https://arxiv.org/abs/1505.01596
  - D. Jayaraman, K. Grauman. Learning image representations tied to ego-motion. arXiv. 2015.
    - https://arxiv.org/abs/1505.02206 

## 7. メモ
- 「自身の行動に関係する特徴」をどう学習している？
  - 逆運動学と順運動学のモデルを両方最適化しているらしい

## 書誌情報
- D. Pathak, P. Agrawal, A. A. Efros, T. Darrell. Curiosity-driven Exploration by Self-supervised Prediction. arXiv. 2017.
  - https://arxiv.org/abs/1705.05363
