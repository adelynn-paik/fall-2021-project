# fall-2021-project

This project seeks to classify images on the basis of whether or not they depict a family. My exploration consists of a two part approach: one, determining whether two faces are related and two, determining if a group photo is that of a family according to their body language. The former is well-documented in a 2019 Kaggle competition hosted by Northeastern's SMILE Lab, where I found my baseline convolutional neural network model. The latter involved more design on my part. It begins with multi-person pose estimation using the OpenPose tool, then the outputs are fed into a recurrent neural network. I conclude the posing work with ablation studies testing K-nearest neighbors and support-vector machine classifiers on the same problem.

Base code for the face models can be found here: https://github.com/CVxTz/kinship_prediction/blob/master/code/vgg_face.py  

Base code for OpenPose can be found here: https://github.com/spmallick/learnopencv/tree/master/OpenPose-Multi-Person 

VGGFace: https://www.robots.ox.ac.uk/~vgg/software/vgg_face/ 
