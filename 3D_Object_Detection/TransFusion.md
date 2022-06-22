paper :[TransFusion: Robust LiDAR-Camera Fusion for 3D Object Detection with Transformers](https://arxiv.org/pdf/2203.11496.pdf)


related works


2. They first find a hard association between LiDAR points and image pixels based on calibration matrices, and then augment LiDAR
features with the segmentation scores


3. or CNN features of the associated pixels through point-wise concatenation.


4. adopt a center-based representation for 3D objects, largely simplifying the 3D detection pipeline


5. The concurrent works adopt transformer as a detection head but focus on indoor scenarios and extending these methods to outdoor scenes is non-trivial.
