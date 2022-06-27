# Capstone Project for Bangkit 2022 Program from BoemBoe Team (C22-PS069)

This repository contains a [dataset](https://github.com/ahmdxrzky/capstone-bangkit-2022/tree/main/dataset/spices.zip) used in the research for my Bangkit team's capstone project. <br>
It is contains 1506 images for training and 300 images for testing, collected from:
* Google Images (we don't own these pictures), and
* Personal Documentation

All images have been preprocessed so they have same size (224 x 224), formatted in RGB, and saved as jpg. <br><br>

This repository also contains script for [preprocess](https://github.com/ahmdxrzky/capstone-bangkit-2022/blob/main/script/script_for_preprocessing.ipynb) and [train the ML model](https://github.com/ahmdxrzky/capstone-bangkit-2022/blob/main/script/script_for_model.ipynb). <br>
After we train the model, we export the model as tflite file. <br>
We also add metadata to the tflite file, according to the way this [web](https://www.tensorflow.org/lite/models/convert/metadata) told us. <br>
The tflite file with its metadata can be found [here](https://drive.google.com/file/d/1-BiDa8ioQTW489EEME6zxkRHugZwiJ7d/view?usp=drivesdk).
