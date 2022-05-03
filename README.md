# Phase 4 Project


## Project Overview

In this project, I chosen image classification of chest xray images to see whether it is belonging to a healthy person or a patient with pneumonia(https://www.kaggle.com/datasets/paultimothymooney/chest-xray-pneumonia). 

It is to design classification model to solve a binary classification problem. 

After comparing different neural network and deep learning models with different plays of the data, give suggestions about the classification model that could achieve good accuracy for image classification. 

## Business Problem

* Q: Who are the stakeholders in this project? Who will be directly affected by the creation of this project?
* A: This project is try to develop a deep learning model that could dertermine whether a chest xray image is
*    belonging to a healthy person or a patient with pneumonia
* Q: What data sources are available to us?
* A: the images were downloaded from https://www.kaggle.com/datasets/paultimothymooney/chest-xray-pneumonia


### The Data

The data is download from Kaggle (https://www.kaggle.com/datasets/paultimothymooney/chest-xray-pneumonia), which has been saved in the folder: /figures/, with three folders corresponding to Train, Val, and Test set


### Data Understanding

#### The data I loaded from the website has already been splitted into three subfolders holding the train, test and validation dataset

#####  Some examples of images from three folders are shown below

![figure of xchestimage](figures/xchestimage.png)

#### I also count the number of images in each folder and found that there are only 8 images in the original validation folder for normal and pneumonia. Therefore, I moved 150 images from training folder to make the following count of images in each set:

![figure of numimagesfinal](figures/numimagesfinal.png)


### Image Classification

I have tried a total of 9 different models with different settings and the results for them are displayed in the following figure:

![figure of modelcomp_testlossacc](figures/modelcomp_testlossacc.png)

It seems that the cnnvgg models are slight better, though they are generally similar among all deep learning models.

#### I chose cnnvgg1 as the final model to see the final classification results

The confusion matrix is shown below:

![figure of FinalModel_conf](figures/FinalModel_conf.png)


## Summary

- It achieves above 90% accuracy with the use of pretrained VGG19 model
- With more adjustment and more data, the accuracy could be further improved