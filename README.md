<h1> Comprehensive Yoga Training System with Pose Detection and Feedback Generation <h1>

<h2> Architecture </h2>

Generating Data 


![alt text](https://github.com/vritansh/poseestimation/blob/main/GeneratingDatasetArchitecture.png?raw=true)


Dataset used for the project : https://www.kaggle.com/datasets/niharika41298/yoga-poses-dataset 

Note:- Please point to the above dataset wherever the references are provided in the .ipynyb files.

In order to run this project follow the below instructions sequence 

1. Run the file   deep-learning-project.ipynb  for below sections :- 

1.a) Code for Movenet

a.b) Code for extracting points for model training

Output - dataset.csv is generated

2. After the dataset.csv is generated from the above step use it train the Custom DNN model using below file 
 File for generating model.h5 and model.json :- custom_points_model.ipynb

Output - model.h5 & model.json

3. Run deep-learning-project.ipynb part 3
. 
Output - Running section 3 should show a webcam and user can select the mode as guided in the GUI. 

Research Based Files :- 

1. research_cnn_model_custom.ipynb - For custom CNN model 
2. research_resnet_transferl_learning.ipynb - For Transfer Learning based Model
