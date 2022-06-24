paper : [EdgeNeXt: Efficiently Amalgamated CNN-Transformer Architecture for Mobile Vision Applications](https://arxiv.org/pdf/2206.10589v1.pdf)

ConvNeXt를 기본 모듈로 하되 Cross-Covariance self-attention 과 스테이지가 깊어짐에따라 CNN encoder 에서의 kernel size를 3, 5, 7, 그리고 9로 늘려가는 
방식을 통해서 성능을 향상시키고 매우 light-weight model의 특성을 지닐 수 있다.

![image](https://user-images.githubusercontent.com/93501772/175471341-44fb2c1c-957d-4368-ab55-bc8ce5640cd3.png)
SDTA encoder를 후반 스테이지에 한 개씩만 배치.. 그리고 adaptive multi-scale feature representation 파트도 재밌는 아이디어라고 생각한다.

