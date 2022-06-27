paper : [An End-to-End Transformer Model for 3D Object Detection](https://arxiv.org/pdf/2109.08141.pdf)


해당 논문에서 크게 컨트리뷰션은 2가지이다.

1. non-parametric queries, Fourier positional embeddings 로 성능을 향상시켰다.
2. DETR을 3D 로 확장 

읽으면서 object query를 초기화할 때 신경을 많이 써야겠다는 생각이 들었다.

또한 PointNet++ 에서의 set-aggregation downsampling operation(sampling(farthest point sampling (FPS) - grouping - pointnet layer)
를 통해서 input points를 병합시켜준다.(CNN을 사용할 수 없으니까 CNN의 역활하는 기법을 도입한 것으로 이해할 수 있다.)  이 과정도 더 정교하게 이루어지면 좋을 듯... 여기서 vision longformer에서의 global token 과 object query와 연결
지으면 좋겠다는 생각이 든다.(GC - ViT와도 연결지어보자.)


또한 3DETR-m 에서는 encoder에서 point clouds에서 self-attention할 때 swin 처럼 local(with radius) attention을 진행하는데 좋은 전략같다.

GIoU를 통해서 bb가 더 gt와 가까워지도록 꾸준히 유도할 수 있도록 한다.

huber loss로 outlier 에 대해서 robust한 loss로 모델 학습..

large size decoder가 훨씬 성능 향상에 도움이 됨 -> 그럼 <set-aggregation downsampling operation - encoder> 를 longformer의 기법을 이용해서 
  단순화할 수 있을 것이다. 
  
  
  ![image](https://user-images.githubusercontent.com/93501772/175886426-2b95d70c-06c5-4600-937b-30c1b0ee18c8.png)
