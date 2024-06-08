# DemographicPredictor

This project aims to develop a deep learning model to predict the age, gender, and race of individuals based on their facial images. The model is trained on a dataset containing labeled images of faces with corresponding age, gender, and race information.

## Project Overview

The project consists of the following components:

- **Dataset**: I used this [dataset](https://www.kaggle.com/datasets/jangedoo/utkface-new/data) from Kaggle to train my model of over 20,000 faces that were prelabeled with age, gender, and race
  
- **Model Training**: Defines and trains the deep learning model using TensorFlow and Keras. The model architecture includes convolutional layers followed by fully connected layers for predicting age, gender, and race.

- **Prediction**: Provides functionality to make predictions on new facial images using the trained model. The predictions include estimated age, gender (male or female), and race (e.g., white, black, Asian).

## Getting Started

To get started with the project, follow these steps:

1. **Dataset Preparation**: Ensure that you have downloaded the dataset.

2. **Model Training**: Use the training part in `main.ipynb` to define and train the deep learning model on the prepared dataset.

3. **Prediction**: After training the model, you can use the last part of main.ipynb to make predictions on whatever faces you like. Provide the path to the image file as input, and the script will output the predicted age, gender, and race.

## Usage

Make sure that you have requirements.txt installed:

```bash
pip install -r requirements.txt
