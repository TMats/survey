# Seven neurons memorizing sequences of alphabetical images via spike-timing dependent plasticity

## 1. どんなもの？
- スパイクタイミング依存可塑性(STDP)をモデルに取り入れたボルツマンマシンDynamic Boltzmann Machineを提案
- 伝導遅延(conduction delay)と各ニューロンとニューロン間にあるメモリユニット(eligibility trace)をモデル化
- 7つのニューロンにバイナリの系列を学習させた

## 2. 先行研究と比べてどこがすごい？
- STDPを利用したモデルである
    - パーセプトロンやBMはHebb則(ニューロンが同時に発火すると結合が強まる)
- conduction delayよりも長い系列を学習することに成功
- 時空間的に局所的に利用可能な情報のみでパラメータを更新してゆく
    - 生物学的なニューロンの特徴で，ハードウエア実装される場合に理想的な形態

## 3. 技術や手法のキモはどこ？
- STDPのモデル化
    - conduction delayとeligibility traceの導入
    - 発火順序により結合の重みが変わる(LTP・LTD)

## 4. どうやって有効だと検証した？
- バイナリ系列の学習(SCIENCEの文字列を0/1の画像に変換し学習させた)

## 5. 議論はある？

## 6. 次に読むべき論文は？
- Learning binary or real-valued time-series via spike-timing dependent plasticity
    - https://arxiv.org/abs/1612.04897
    - https://github.com/TMats/survey/issues/2
- Nonlinear Dynamic Boltzmann Machines for Time-Series Prediction
    - https://aaai.org/ocs/index.php/AAAI/AAAI17/paper/view/14350
    - https://github.com/TMats/survey/issues/3


## 7. メモ
- https://github.com/TMats/survey/issues/1
- [輪読会](http://deeplearning.jp/seven-neurons-memorizing-sequences-of-alphabetical-images-via-spike-timing-dependent-plasticity/)

## 書誌情報
- T. Osogami and M. Otsuka. Seven neurons memorizing sequences of alphabetical images via spike-timing dependent plasticity. Scientific Reports 5 (2015). 2015.
    - https://www.nature.com/articles/srep14149
