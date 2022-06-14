paper : [Multi-Scale High-Resolution Vision Transformer for Semantic Segmentation](https://arxiv.org/pdf/2111.01236v2.pdf)


![image](https://user-images.githubusercontent.com/93501772/173487968-5e02757a-96d0-499d-9958-1207c02edd47.png)

기존의 ViT 에서 feature들을 sequentially 다룬 반면에 해당 논문에서는 각 해상도마다 병렬적으로 feature들을 처리한다.
또한 병렬적으로 처리되는 서로 다른 종류의 feature들을 융합하기 위해서 아래의 Cross-resolution fusion layer를 사용.
Locally enhanced FFNs 와는 조금 다른 종류의 FFN도 확인할 수 있다.(Not original)

 + base attention module : CSWin Attention(local)

![image](https://user-images.githubusercontent.com/93501772/173488236-13ac0289-5219-46ac-8a70-995480487950.png)
