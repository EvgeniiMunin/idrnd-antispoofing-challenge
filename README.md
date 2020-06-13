# Kaggle IDR&D Antispoofing Challenge

The competition organized on the platform DataSouls has the objective to develop the algorithm detection of spoofing attacks in face recognition.

## Hardware
- GPU: 1xTesla K80

## Data format
The images are represented in the form of frames in video sequence having the following attributes: ```label, path, video```.

## Solution
The solution represents:
- model: ResNet50
- validation metrics: ```minC = FP / (FP + TN) + 19*FN / (FN + TP)```
- augmentations: RandomHorizontalFlip, RandomResizedCrop, ColorJitter
- optimizer: Adam
- loss: BCELoss
- batch size: 64
