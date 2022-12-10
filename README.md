# Comprehensive Yoga Training System with Pose Detection and Feedback Generation 

Dataset used for the project : https://www.kaggle.com/datasets/niharika41298/yoga-poses-dataset 

In order to run this project follow the below instructions. 

Files contained in the project :-

1. main.py - this file contains all the details of the model. This includes the below modules 
1.a). Getting input from the images using movenet. 

1.b). Extracting points using movenet model

1.c). Preprocessing the movenet output and saving to dataset.csv file

1.d). Reading the custom trained model .h5 and .json file which has the model references. 

1.e). Taking the input from the webcam 

1.f). Extracting frames from the input and using those frames to preprocess the details. 

1.g). Predicting the user pose using pretrained model for the points extracted using movenet.

1.h). Providing user feedback about the pose. Currently it supports the provision of the pose for the user for only one pose. i.e. Downdog. This process is only for prototyping. For downdog position. 

2. custom_points_model.py
2.a) This file contains code for EDA on the movenet generated points 
2.b) These points are then used to train a custom Deep Neural Network for the model prediction
2.c) The hyperparameter tuning and all the necessary outputs for the metrics for our model is contained in this file.

3. research_cnn_model.py
3.a) Preprocessing the image files that are taken from the movenet model. 
3.b) The preprocessed files are passed to the model. 

4. research_transfer_learning.py 
< > 

Steps to produce the model
1. Run "Points Generation" section in main.py to generate dataset.csv
2. Generate the model using custom_points_model.py
3. Run "OpenCV Extraction" section in main.py by correctly referensing the model.h5 and model.json files 

Expected output
1. The user can make any o the below poses to obtain the requested output
2. The output obtained by the user would be then predicted by the model that is trained on the yoga dataset initiall on the points seciton.


