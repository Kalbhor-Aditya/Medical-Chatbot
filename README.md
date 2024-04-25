# Medical Chatbot

## Introduction

This project is about a Medical Chatbot that uses a deep learning model to understand and respond to user queries related to medical information (Mental Health).The chatbot is trained on a dataset of intents and their corresponding responses.

## Model Description

The main model of the chatbot is a Sequential model built using Keras. The model architecture is as follows:

1. **Input Layer**: A Dense layer with 128 neurons and 'relu' activation function. The input shape corresponds to the length of `train_x[0]`.

2. **Dropout Layer**: A Dropout layer with a dropout rate of 0.5 to prevent overfitting.

3. **Hidden Layer**: A Dense layer with 64 neurons and 'relu' activation function.

4. **Dropout Layer**: Another Dropout layer with a dropout rate of 0.5.

5. **Output Layer**: A Dense layer with neurons equal to the length of `train_y[0]` and 'softmax' activation function for multi-class classification.

The model is compiled with the loss function as 'categorical_crossentropy', optimizer as SGD (with learning rate 0.01, momentum 0.9, and Nesterov enabled), and metrics as 'accuracy'.

The model is trained for 200 epochs with a batch size of 5. The trained model is saved as 'medical_chatbot_model.hs'.

## Dataset

The model is trained on a dataset derived from an intents JSON file. This file contains various user intents and their corresponding responses which the chatbot is expected to provide.

## Usage

1] Simply Git clone.

2] Run the notebook.


## Future Work

Future improvements can include expanding the dataset for more diverse queries, tuning the model for better performance, and deploying the chatbot on a web server for easy access and usage.



