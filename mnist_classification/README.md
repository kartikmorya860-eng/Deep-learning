# MNIST Classification

This project contains a Jupyter Notebook that builds and trains a simple neural network on the MNIST handwritten digits dataset using TensorFlow and Keras.

## Notebook

- `mnist_classification.ipynb`

## Overview

The notebook performs the following steps:

1. Load the MNIST dataset from `tensorflow.keras.datasets.mnist`
2. Normalize pixel values to the range `[0, 1]`
3. Display sample digit images using `matplotlib`
4. Define a sequential Keras model with:
   - `Flatten` input layer for 28x28 grayscale images
   - Dense layer with 128 units and ReLU activation
   - Dense layer with 32 units and ReLU activation
   - Output Dense layer with 10 units and softmax activation
5. Compile the model with `sparse_categorical_crossentropy`, the Adam optimizer, and accuracy metrics
6. Train the model for 25 epochs with a validation split
7. Predict on the test set and compute accuracy using `sklearn.metrics.accuracy_score`
8. Plot training/validation loss and accuracy curves
9. Display a sample test image and its predicted label

## Requirements

- Python 3.7+ (recommended)
- TensorFlow
- matplotlib
- scikit-learn

## Installation

```bash
pip install tensorflow matplotlib scikit-learn
```

## Usage

1. Open `mnist_classification.ipynb` in Jupyter Notebook or JupyterLab.
2. Run each cell in order.
3. Inspect the model summary, training history, evaluation accuracy, and prediction output.

## Notes

- The model uses a simple fully connected neural network and is intended as a basic MNIST classification example.
- For improved accuracy, consider experimenting with convolutional layers, dropout, or a larger network.
