# Capstone Project for Bangkit 2022 Program from BoemBoe Team (C22-PS069)

## Project Domain ##
Problem being highlighted in this project is in **Food & Agriculture** domain. Based on my team experience, we often found that it's hard to distinguish one spice to another. It's simply because many of them have similar shape and colour. That's why this project being conducted to help beginner cooks or people to distinguish spice based on its image in simple way.

## Business Understanding ##
#### Problem Statement ####
"How to build a system to detect type of spice based on its image?"
#### Goal ####
"Making of machine learning model to detect type of spice based on its image."
#### Solution Statements ####
Build a ML model using pre-trained model with some modification

## Data Understanding ##
Dataset being used in this project is a self-made dataset. It has 1506 images for training and 300 images for testing from 6 different type of spices. It's gained from personal documentation and Google Images, so my team don't claim any copyrights of it. <br>
This dataset can be retrieved [here](https://github.com/ahmdxrzky/capstone-bangkit-2022/tree/main/dataset/spices.zip).
#### Data Preprocessing ####
Because images gained from various sources, they have different size and format in the beginning. To make the ML model easy to learn about the images, preprocessing stage should be applied. So, the images are being converted to jpg format and resized to 224 x 224 pixel. Last but not least, they are packed up as a zip file and uploaded to github for easier further use. <br>
Script for this processes can be accessed [here](https://github.com/ahmdxrzky/capstone-bangkit-2022/blob/main/script/script_for_preprocessing.ipynb).

## Modeling ##
Model in this project were built using InceptionV3 pre-trained model up to 'mixed7' layer. Additional dense and output layer being added after 'mixed7' layer to adjust with the condition needed in the project (6 categories of detection). Dataset in the zip file is being extracted and used for train the model. After being trained to certain desired level, export the model as tflite model to be used in the android application. Script for this processes can be accessed [here](https://github.com/ahmdxrzky/capstone-bangkit-2022/blob/main/script/script_for_model.ipynb).

## Evaluation ##
Evaluation metric used here is accuracy. Formula for accuracy metric is shown below. <br>
![Accuracy Formula](https://user-images.githubusercontent.com/99194827/181746873-dc624763-ae3d-4c10-8815-c8f24ee69aa5.png) <br>
Accuracy score of model in this project is 98% for training and 85% for testing data. With this very high accuracies, we can certain that this model is very good to fulfill our objective.
