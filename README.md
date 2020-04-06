# CS893-Semantic-Segmentation
Semantic Segmentation is the classification of images on pixel level. The purpose is to understand and recognize what is in the image in pixel level. Semantic Segmentation has wide range of applications such as Robot Vision and Understanding, Autonomous Driving and Medical Purposes.
In this project, I am doing semantic segmentation on MonuSeg Dataset using different segmentation techniques/architectures which are U-Net, Segnet and DeepLab-v3.

## 1. U-Net
(Modified the original implementation at https://github.com/hlamba28/UNET-TGS/blob/master/TGS%20UNET.ipynb for this dataset)

###### Model Diagram
![model plot](unet_model_plot.png)

###### Training Settings
* Optimizer: SGD
* Learning Rate: 0.001
* Batch Size: 5

###### Evaluation
* Accuracy (on Test Data) = 0.82
* Dice Score = 0.41

###### Learning Curve
![Learning Curve](unet_learning_curve.png)

###### Visualization
![demo1](unet_demo1.png)
![demo2](unet_demo2.png)

## 2. SegNet
For this network I have used 256x256 size images for training which are actually patches of original 1000x1000 size image.

###### Model Diagram
![model plot](segnet-model-diagram.png)

###### Training Settings
* Optimizer: Adam
* Batch Size: 16

###### Evaluation
* Accuracy = 0.58
* Dice Score = 0.35
* F1-Score = 0.43
* Loss (Binary Crossentropy) = 0.82

###### Learning Curve
![Learning Curve Loss](segnet-loss-curve.png)
![Learning Curve Acc](seget-acc-curve.png)

###### Visualization
![demo1](segnet-demo1-test.png)
![demo2](segnet-demo2-test.png)

## 3. DeepLab-v3
