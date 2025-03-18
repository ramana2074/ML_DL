# Project Overview
This project implements a Handwritten Digit Recognition model using the MNIST dataset. It employs a Convolutional Neural Network (CNN) to classify handwritten digits (0–9) with high accuracy.

## Dataset
Dataset Used: MNIST (Modified National Institute of Standards and Technology)
Training Samples: 60,000 images
Test Samples: 10,000 images
Image Size: 28 x 28 pixels (grayscale)

## Model Architecture
The CNN model includes the following layers:

Conv2D: 32 filters, kernel size = 3x3, activation = ReLU
MaxPooling2D: Pool size = 2x2
Dropout: 25%
Conv2D: 64 filters, kernel size = 3x3, activation = ReLU
MaxPooling2D: Pool size = 2x2
Dropout: 25%
Flatten: Converts data to a 1D vector
Dense: Fully connected layer with 128 neurons, activation = ReLU
Dense: Output layer with 10 neurons (representing digits 0–9), activation = Softmax

## Preprocessing
Reshaped input images to (28, 28, 1)
Normalized pixel values to [0, 1] range
One-hot encoding applied to labels
Training and Evaluation
Loss Function: Categorical Crossentropy
Optimizer: Adam
Metrics: Accuracy

## Results
Achieved high accuracy on test data
Included visualization of training progress using matplotlib