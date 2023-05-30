# Vision-based Vehicle Speed Estimation

CIVIL-459 Final Project: Vision-based Vehicle Speed Estimation

This work is a part of ”Building AV Autopilot” Project of CIVIL-459 course at EPFL.

This work is aim to solve this problem by estimating the ego vehicle speed using only frames from a single front-facing monocular camera with a mask of the lane to preserve spatiotemporal features as input and receive high performance of vehicle speed estimation as output.

## Prediction Result

<div style="display: flex; justify-content: center;">
<video align="center" width="640" height="480" controls>
    <source src="./data/prediction.mp4" type="video/mp4">
</video>
</div>

## Validation Loss

<p align="center">
<img width="600" src="./mse_loss.jpeg"/>
<p align="center">mean square error loss on both train dataset and validation dataset</p>
</p>

## Files Structure:

    ego-vehicle-speed-estimation
    |
    |____data
    |      |
    |      |____weights.h5          - wights of the pre-trained model
    |      |
    |      |____test.mp4            - test video
    |      |
    |      |____train.mp4           - train video
    |      |
    |      |____test_pred.txt       - model prediction of test data
    |
    |____Speed_Estimation.ipynb     - 3DCNN model with preprocessing pipeline
    |
    |____labels.txt                 - ground truth of train data (train.mp4).
    |
    |____cnn_network.png            - architecture of 3DCNN model
    |
    |____requirements.txt           - required libraries
    |
    |____mse_loss.png               - graphic of mse loss on train and validation data

## 3D CNN Architecture

<p align="center">
<img width="600" src="./cnn_network.png"/>
<p align="center">the architecture of best model: 3D CNN</p>
</p>
