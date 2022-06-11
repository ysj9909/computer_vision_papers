paper : [MeMViT: Memory-Augmented Multiscale Vision Transformer for Efficient Long-Term Video Recognition](https://arxiv.org/abs/2201.08383)

핵심은 이전 시점 클립의 k, v를 압축된 형태로 메모리에 저장해두고 현재 시점의 q와 attention을 진행해준다. 이때 Compression pooling을 
바로 이전 시점의 q, v에 대해서는 stop gradient를 걸어주지 않음으로써 현재 시점의 feature들과 결합적으로 학습될 수 있도록 한다.


![image](https://user-images.githubusercontent.com/93501772/173164425-5e02973f-2ebb-44d8-9a7c-39ffbf34f6a9.png)


Model Overview
![image](https://user-images.githubusercontent.com/93501772/173164540-747f7334-b98e-4440-8054-99cba98f624b.png)
