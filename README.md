Neural Network Implementation on Synthetic Data

This project demonstrates the implementation of a basic neural network with three hidden layers using NumPy. The network is trained on a synthetic dataset with 5 classes, and various performance metrics are plotted to evaluate the model.
Table of Contents

    Overview
    Dataset
    Neural Network Architecture
    Requirements
    Usage
    Results
    License

Overview

This project implements a neural network from scratch using NumPy for the purpose of multi-class classification. The neural network is trained on a synthetic dataset generated with specific ranges for each class. It includes the following components:

    Data generation
    Neural network definition with forward and backpropagation
    Training the network
    Evaluating the model performance using metrics like confusion matrix and ROC curve

Dataset

A synthetic dataset is generated with 500 samples, divided into 5 classes. Each class has distinct ranges for two features, X1 and X2.

    Features: Two numerical features (X1 and X2)
    Classes: 5 classes, each represented with a unique label

Neural Network Architecture

The neural network implemented in this project consists of:

    An input layer with 2 neurons (corresponding to the two features)
    Three hidden layers with 12, 10, and 8 neurons respectively
    An output layer with 5 neurons (corresponding to the number of classes)

Activation Functions:

    Hidden layers: Sigmoid and ReLU
    Output layer: Softmax

Loss Function:

    Mean Squared Error (MSE) is used to measure the performance of the network during training.

Optimization:

    Gradient descent with a fixed learning rate for backpropagation.

Requirements

To run this project, you'll need the following libraries:

    NumPy
    tqdm
    Seaborn
    Matplotlib
    Scikit-learn

Install the necessary packages using:

bash

pip install numpy tqdm seaborn matplotlib scikit-learn

Usage

    Clone this repository.
    Ensure all the required libraries are installed.
    Run the Python script to train the neural network and generate the results.

bash

python neural_network.py

Code Breakdown
1. Importing Libraries

The script begins by importing necessary libraries for data generation, manipulation, visualization, and machine learning tasks.
2. Generating the Synthetic Dataset

The dataset is created using numpy by generating random values within specified ranges for 5 classes.
3. Visualizing the Dataset

A scatter plot is generated to visualize the distribution of the synthetic data.
4. Preprocessing

The labels are one-hot encoded, and the data is split into training and testing sets.
5. Neural Network Implementation

A neural network class is defined, which includes:

    Initializing weights and biases
    Defining activation functions
    Implementing forward propagation
    Implementing backpropagation

6. Training the Neural Network

The network is trained using 2500 epochs, and the training error is plotted.
7. Evaluating Model Performance

After training, the model's performance is evaluated using:

    Classification report
    Confusion matrix
    ROC curve

Results

The results include:

    A plot of the training error over epochs.
    A confusion matrix to show the model's classification performance.
    ROC curves for each class to visualize the model's ability to discriminate between different classes.

License

This project is licensed under the MIT License - see the LICENSE file for details.
