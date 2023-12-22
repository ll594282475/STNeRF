# STNeRF
This is the implementation of "STNeRF: Single-View Novel View Synthesis using Symmetric Triplane Neural Radiance Fields".

This paper presents STNeRF, a method for reconstructing 3D information of a target from a single 2D image without the need for any 3D ground truth data, such as point clouds, depth maps, CAD models, etc., as prior knowledge. An important challenge in this task is that the characteristics of CNNs and the utilization of local features may result in a flattened representation of the synthesized image when trained and validated using images from a single viewpoint. Existing approaches often neglect local features and rely on global features throughout the entire reconstruction process, potentially causing the loss of fine-grained details in the synthesized image. To address this issue, this paper introduces the symmetric triplane neural radiance fields (STNeRF) framework. STNeRF employs a spatially consistent triplane feature extractor to extend 2D image features into 3D. This decouples the appearance component, which includes local features, and the shape component, which comprises global features, and utilizes them to construct a neural radiance field. These neural priors are employed for rendering new perspective images. Furthermore, STNeRF leverages the target's symmetry property, allowing the appearance component to be independent of the original viewpoint and tending to align with the target's spatial symmetry. This enhances the network's capability to represent invisible regions. Qualitative and quantitative evaluations demonstrate that STNeRF outperforms existing solutions in terms of both geometry and appearance reconstruction.

# Framework
![framework.png](https://github.com/ll594282475/STNeRF/blob/main/pic/framework_new.png)

# Results
 | Ori  |  Output |
| ------------ | ------------ |
|  <img src="pic/003512_00_patch.png" alt="drawing" width="200"/> | <img src="pic/vis1.gif" alt="drawing" width="200"/> |


![result_1.png](https://github.com/ll594282475/STNeRF/blob/main/pic/result_1.png)


# The code is coming soon.
