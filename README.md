# CS893-Semantic-Segmentation
Semantic Segmentation is the classification of images on pixel level. The purpose is to understand and recognize what is in the image in pixel level. Semantic Segmentation has wide range of applications such as Robot Vision and Understanding, Autonomous Driving and Medical Purposes.
In this project, I am doing semantic segmentation on MonuSeg Dataset using different segmentation techniques/architectures which are U-Net, Segnet and DeepLab-v3.

## 1. U-Net
(Modified the original implementation at https://github.com/hlamba28/UNET-TGS/blob/master/TGS%20UNET.ipynb for this dataset)

###### Model Diagram:
![model plot](unet_model_plot.png)

###### Training Settings
* Optimizer: SGD
* Learning Rate: 0.001
* Batch Size: 5

###### Evaluation
* Accuracy (on Test Data) = 0.82
* Dice Score = 0.41

###### Learning Curve:
![Learning Curve](unet_learning_curve.png)

## 2. SegNet
## 3. DeepLab-v3
