# CNN-with-Fashion-MNIST-Dataset
This project implements a Convolutional Neural Network (CNN) to classify Fashion images  using PyTorch.

## Dataset
Fashion-MNIST is a dataset of Zalando's article images—consisting of a training set of 60,000 examples and a test set of 10,000 examples. Each example is a 28x28 grayscale image, associated with a label from 10 classes.
Dataset was downloaded directly from torch library. 

## Dependencies
torch
torchvision
matplotlib
pandas
Numpy

## Pre-processing

Pixel Values was scaled to values between 0 and 1 and then standardization done using mean and std

## Training
2 convolutional layers- of 48 and 96 filter kernels
2 Max-pooling Layers
30% dropped out to prevent Over fitting
2 Fully connected Layers
Adam Optimizer for back propagation
Cross Entropy loss as loss function
Trained over 10 Epochs
Accuracy used as evaluation metric

## Limitations
Validation loss rises after 7th epoch indicating its better to have stopped earlier though accuracy is still 91.04% at 10th epoch which is not really  bad

## Further Evaluation
Further Evaluation was done using K-fold algorithm to observe model performance on entire dataset for the sake of generalization. Avarage Accuracy across of folds lies at over 90% which is close to training the entire dataset at once. 
