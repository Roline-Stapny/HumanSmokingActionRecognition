# Human_Smoking_Action_Recognition

This project mainly aims to identify human smoking actions from videos. LRCN architecture is applied to identify human smoking actions from videos. This work was motivated and referenced from https://github.com/doronharitan/human_activity_recognition_LRCN. 

HMDB51 and STAIR Actions dataset are used in this project
datasets can be downloaded at 
https://serre-lab.clps.brown.edu/resource/hmdb-a-large-human-motion-database/#Downloads https://actions.stair.center/videos.html

The project is sectioned into 3 parts. 
1. Pre-processing
2. Training
3. Finding Moments

The first step is to download the dataset and preprocess it. After downloading the dataset use 'data_preprocess.py' file to preprocess the dataset. Make sure to change the path appropriately. This code takes the videos as input and samples them and creates videos with 15 frames. 


Run the training.py file to train the network using the sampled videos obtained from after preprocessing. Make sure to change the path names appropriately. You can also change the values of the hyperparameters to improve the model performance. This code saves the model checkpoints, the loss values and other results in the specified folder.


Finally use findMoments.py file to predict the moments from youtube video. You have to specify the model checkpoint path and the test video path here. This file will predict the moments and save them in the json format which could be uploaded on the ilab website.
