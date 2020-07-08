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


