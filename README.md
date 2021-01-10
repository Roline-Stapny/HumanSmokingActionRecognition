# Human_Smoking_Action_Recognition
LSTM+CNN architecture is applied to identify human smoking actions from videos

This code was executed in google colab

The reference code was taken from https://github.com/doronharitan/human_activity_recognition_LRCN

datasets can be found at :
https://serre-lab.clps.brown.edu/resource/hmdb-a-large-human-motion-database/#Downloads
https://actions.stair.center/videos.html

data_preprocess.py - has the code to preprocess the data.

training.py - has the code to train the model.

findMoments.py - has the code get the moments from the youtube video.

First preprocess the video dataset using data_preprocess.py. The output of this will be sampled video frames.
Use the sampled video frames to train the LRCN model. The code is present in training.py. Change the parameters according to your requirements in this file. The model is saved in the specified location.
Finally use the trained model to generate moments from youtube videos. The code is present in findMoments.py file.
