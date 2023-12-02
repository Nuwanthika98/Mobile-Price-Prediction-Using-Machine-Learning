# Mobile-Price-Prediction-Using-Machine-Learning

## Overview:        
This repository contains two implementations for predicting the price range of mobile phones: A Multi-layer Neural Network and a K-Nearest Neighbors (KNN) algorithm.         
The dataset used for training and testing is sourced from 'Mobile_Dataset.csv'.

## Multi-layer Neural Network:            

### Architecture:        
The neural network architecture consists of three layers:        
Input layer with 20 features.        
Two hidden layers with 32 neurons each, ReLU activation, and L2 regularization to prevent overfitting.        
Dropout layers with a dropout rate of 0.3 to further reduce overfitting.        
Output layer with 4 neurons using the softmax activation function.        

### Training:
The model is trained using Stochastic Gradient Descent (SGD) as the optimizer and sparse categorical crossentropy as the loss function. Training is conducted over 1000 epochs with a batch size of 64.

### Evaluation:        
The model's performance is evaluated on a test dataset, providing both loss and accuracy metrics. Training and testing accuracy/loss curves are visualized for analysis.


## K-Nearest Neighbors Algorithm:

### Data Preprocessing:        
The dataset is standardized using the StandardScaler from scikit-learn.

### Model Training:        
The K-Nearest Neighbors algorithm is employed, and the optimal number of neighbors is determined by assessing error rates across a range of values (1 to 200). The model is then trained with the selected optimal value.

### Prediction and Evaluation:        
The trained model is used to make predictions on the test dataset, and performance metrics such as classification report and confusion matrix are provided.
