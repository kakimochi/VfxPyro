# VFX Graphで花火をつくる
- [keijiro/VfxPyro](https://github.com/keijiro/VfxPyro)

# HDRPのインストール
(省略)

# VFX Graphをインストール
(省略)

# Particleを散らす
- Randomな速度Vectorを与える
- "Initialize Partice" へ set velocity ノードを追加する
    - InspectorでRandom:PerComponentにする
    - X:-1, Y:-1, Z:-1
    - X:1,  Y:1,  Z:1
    - いろんな方向へ散るようになる

# 同時に同心円状にParticleでるようにする
- "Spawn System"で"Single Burst"にする
- Count : 100

# 繰り返しにする
- "Span Sytem"へ"Periodic Burst"を追加する
- Count : 100
- Delay : 1

# ParticleのLifetime調整
- "Initialize Particle"の"Set Lifetime"のLifetime:0.6

# 飛び散る範囲を円状にする
- 中心からランダムな方向に長さ１のベクトルで散らす
- Random Directionノードを追加する
  - 
