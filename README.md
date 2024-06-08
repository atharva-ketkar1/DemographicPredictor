# DemographicPredictor

This project aims to develop a deep learning model to predict the age, gender, and race of individuals based on their facial images. The model is trained on a dataset containing labeled images of faces with corresponding age, gender, and race information.

## Project Overview

The project consists of the following components:

- **Dataset**: I used this [dataset](https://www.kaggle.com/datasets/jangedoo/utkface-new/data) from Kaggle to train my model of over 20,000 faces that were prelabeled with age, gender, and race
  
- **Model Training**: Defines and trains the deep learning model using TensorFlow and Keras. The model architecture includes convolutional layers followed by fully connected layers for predicting age, gender, and race.

- **Prediction**: Provides functionality to make predictions on new facial images using the trained model. The predictions include estimated age, gender (male or female), and race (e.g., white, black, Asian).

## Results

FIRST IMPLEMENTATION:
CNN with 3 Convolutional Blocks with Conv2D and MaxPooling.It then Flattens and goes to 3 Fully Connected Layers(Age, Gender, Race) with Dropout(0.3) to try and combat overfitting.

results:
148/148 [==============================] - 7s 49ms/step - loss: 97.0403 - age_output_loss: 95.8356 - gender_output_loss: 0.3320 - race_output_loss: 0.8728 - age_output_mae: 7.3400 - gender_output_accuracy: 0.8676 - race_output_accuracy: 0.7128

~ This means that the model is able to predict the age of a person where the age is off by approximately 7.34 years. Gender accuracy is 86.8% and Race accuracy is 71.3%

SECOND IMPLEMENTATION:
CNN with 4 Convolutional Blocks with Conv2D, BatchNormalization, and MaxPooling. It then Flattens and goes to 3 Fully Connected Layers(Age, Gender, Race) with Dropout(0.5) to try and combat overfitting.

148/148 [==============================] - 6s 43ms/step - loss: 72.3999 - age_output_loss: 71.8970 - gender_output_loss: 0.1238 - race_output_loss: 0.3790 - age_output_mae: 6.6578 - gender_output_accuracy: 0.9502 - race_output_accuracy: 0.8790

~ This means that the model is able to predict the age of a person where the age is off by approximately 6.66 years. Gender accuracy is 95.0% and Race accuracy is 87.9%
