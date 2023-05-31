# Vision-based Vehicle Speed Estimation

CIVIL-459 Final Project: Vision-based Vehicle Speed Estimation

This work is a part of ”Building AV Autopilot” Project of CIVIL-459 course at EPFL.

This work is aim to solve this problem by estimating the ego vehicle speed using only frames from a single front-facing monocular camera with a mask of the lane to preserve spatiotemporal features as input and receive high performance of vehicle speed estimation as output.

## Prediction Result

https://github.com/vita-student-projects/vision-based_vehicle_speed_estimation_gr26/assets/99803920/ae21e893-207d-4c84-a186-b83329f63e8c

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
    |      |____weights.h5              - wights of the final model (3D CNN)
    |      |
    |      |____c3d-sports1M_weights.h5 - wights of the pre-trained model
    |      |
    |      |____test.mp4                - test video
    |      |
    |      |____train.mp4               - train video
    |      |
    |      |____test_pred.txt           - model prediction of test data
    |
    |____Speed_Estimation.ipynb         - final pipeline (includes 3D CNN)
    |
    |____Speed_Estimation_v1.0.ipynb    - pipeline with more debug details
    |
    |____labels.txt                     - ground truth of train data (train.mp4).
    |
    |____cnn_network.png                - architecture of 3DCNN model
    |
    |____requirements.txt               - required libraries
    |
    |____mse_loss.png                   - graphic of mse loss on train and validation data

## Dataset

to do

## Augmentation train data

to do

## Piplines

to do

## The Best Model: 3D CNN Architecture

<p align="center">
<img width="300" src="./cnn_network.png"/>
<p align="center">the architecture of best model: 3D CNN</p>
</p>

## Contributions:
