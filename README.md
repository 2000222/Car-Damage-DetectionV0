# Project Descriptions
In industries like car rental, both owners and renters, are at-risk of being a victim of fraud. To help aid in the claims process for insurance carriers, there needs to be a way to detect car damages from photos pre/post rental trip. This project aims to develop an accurate, reliable, and efficient algorithm for detecting all new damages by comparing both pre-trip and post-trip images, as well as evaluating the severity of them. We have >1000 images taken from Google Image search result and labeled with bounding boxes of different types of damages, such as scratches and dents. An easy solution is to develop a standard object detection model to find all damages from both pre-trip and post-trip images, then use traditional algorithm to find perspective transformation between both images, which will be used to find correspondences of all the detected bounding boxes. This algorithm will be the baseline for this project and we are trying to find better performed algorithms.

This work as part of "Car Damage Detection and Patch-to-Patch Self-supervised Image Alignment" project has been accepted by 2021 NeurIPS WiML Workshop. 

# Car-Damage-DetectionV0
AI methods for Car Damage Detection with Mask-RCNN

Run a baseline for instance segmentation on car damage detection.

```
python custom.py train --dataset=./customImages/ --weights=coco
```

Resume a pre-trained model to train. (Make Sure the model at the folder)
```
python custom.py train --dataset=./customImages/ --weights=last
```


# Car-Damage-DetectionV1
## Annotate the new car dataset with labelimg：

Steps:

```
pip install labelimg
python labelImg.py
```

More usage detail could be linked to [this article](https://medium.com/deepquestai/object-detection-training-preparing-your-custom-dataset-6248679f0d1d)

## Be familiar with image alignment and find homography opencv function.

[Tutorial](https://www.learnopencv.com/homography-examples-using-opencv-python-c/) for find homography openCV.

# Car-Damage-DetectionV1
## New ideas with Contrastive Learning or 3D computer vision.

1. Contrastive learning paper: SimCLR;  

2. PointNet:  https://github.com/charlesq34/pointnet

https://github.com/fxia22/pointnet.pytorch  Classification + Segmentation.

# Car-Damage-DetectionV2
## Need to improve the training speed and change the augmentation issue.  

## Propose a new self-supervised Patch-to-patch image alignment method with contrastive learning. 
Need to design a scientific self-supervised evaluation method with T-SNE. 
