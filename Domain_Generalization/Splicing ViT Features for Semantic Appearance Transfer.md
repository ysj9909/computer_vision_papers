[Splicing ViT Features for Semantic Appearance Transfer](https://arxiv.org/pdf/2201.00424.pdf)



 we propose novel deep representations of appearance and structurethat are extracted from DINO-ViT – a Vision Transformer model that has been pre-trained in a self-supervised manner


From shallow to deep layers, the [CLS] token gradually accumulates appearance information. Earlier layers mostly capture local texture patterns, while in deeper
layers, more global information such as object parts
emerges.
![image](https://user-images.githubusercontent.com/93501772/179619295-e2ec516b-bd9e-4ac5-85d1-e0ca0a8035da.png)



The [CLS] token encodes appearance information in a
spatially flexible manner, i.e., different object parts can stretch, deform or be flipped. Figure 4 shows multiple
runs of our inversions per image; in all runs, we can notice similar global information, but the diversity across
runs demonstrates the spatial flexibility of the representation.
