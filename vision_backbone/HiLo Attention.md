paper : [Fast Vision Transformers with HiLo Attention](https://arxiv.org/abs/2205.13213)


HOW DO VISION TRANSFORMERS WORK? 라는 논문에서 MSAs는 low-pass filter이고 CNNs는 high-pass filter라는 사실을 밝혔다.
이러한 사실을 바탕으로 하나의 레이어에서 Inception Transformer에서 처럼 채널을 split하고 local MSA와 Global MSAs(to average
pooled features)를 각각 적용시켜 두 가지 features를 잘 fusion(channel concat)한다. 채널의 redundancy를 생각해봤을 때 split하는건 
굉장히 좋은 선택이라 생각이 된다. 또한 두 가지 필터를 하나의 레이어에서 적용할 수 있으므로 좋은 방법같다.

이렇듯 서로 다른 역활을 하는 모듈이 있다면 이러한 방법으로 fusion하는 것도 좋을 것 같다.
