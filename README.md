# CIFAR-10 Image Classification with CNN

A custom convolutional neural network built and trained with PyTorch to classify images from the CIFAR-10 dataset into 10 categories.

## Project Overview

This project implements an end-to-end image classification pipeline, including data preprocessing, augmentation, model development, training, validation, checkpoint saving, and final test evaluation.

## Dataset

The CIFAR-10 dataset contains 60,000 color images across 10 classes.

* Training set: 45,000 images
* Validation set: 5,000 images
* Test set: 10,000 images
* Image size: 32 × 32 pixels

## Model Architecture

The custom CNN contains:

* Three convolutional blocks
* 32, 64, and 128 output channels
* Batch Normalization
* ReLU activation
* Max Pooling
* Fully connected classifier
* Dropout for regularization
* 10-class output layer

## Data Preprocessing

The training pipeline uses:

* Random cropping with padding
* Random horizontal flipping
* Tensor conversion
* Image normalization

Validation and test images are normalized without augmentation.

## Training

* Loss function: Cross-Entropy Loss
* Optimizer: Adam
* Learning rate: 0.001
* Batch size: 64
* Number of epochs: 20
* The best model checkpoint was selected using validation accuracy.

## Results

| Metric                   | Accuracy |
| ------------------------ | -------: |
| Best validation accuracy |   82.74% |
| Test accuracy            |   82.44% |

## Technologies

* Python
* PyTorch
* Torchvision
* NumPy
* Matplotlib
* Jupyter Notebook

## Repository Contents

* `cifar10_cnn_image_classification.ipynb` — data preparation, CNN implementation, training, validation, and test evaluation.
