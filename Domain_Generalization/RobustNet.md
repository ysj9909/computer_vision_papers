[RobustNet: Improving Domain Generalization in Urban-Scene Segmentation via Instance Selective Whitening](https://arxiv.org/abs/2103.15597)

	- Robustnet을 읽으면서 든 생각은 
  1. 해당 논문은 CNN의 feature를 기준으로 한 기법인데 ViT의 feature space에서는 어떤 양상인지 Vision Transformer를 이용한 style transfer논문을 찾아봐야 겠다. 
  22. 사실 해당 논문에서는 gaussian blurring, color    jittering 이라는 domain shift 문제를 해결하려고 하지만 사실 이 transform외에도 다양한 domain shift 양상이 존재할 수 있다. 따라서 AdaIN으로 넘어가는 논리를 adaptation할 수 있을지 생각해야한다. 
  23. 3. 해당 논문에서는 DG를 semantic segmentation task에 적용했지만 3D Object Detection에 적용해봐야겠다. 또한 해당 논문이 있는지 찾아보자(2D도 찾아보자.) 또한 3D Object Detection에 적용한다면 Lidar feature는 또 어떻게 다뤄야할지도 고려해보자



