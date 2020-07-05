# Car-Damage-DetectionV0
AI methods for Car Damage Detection with Mask-RCNN

Run a baseline for instance segmentation on car damage detection.

python custom.py train --dataset=./customImages/ --weights=coco

python custom.py train --dataset=./customImages/ --weights=last

# Car-Damage-DetectionV1
## Annotate the new car dataset with labelimg：

Steps:

```
pip install labelimg
python labelImg.py
```

More usage detail could be linked to [this article](https://medium.com/deepquestai/object-detection-training-preparing-your-custom-dataset-6248679f0d1d)

## Be familiar with 

