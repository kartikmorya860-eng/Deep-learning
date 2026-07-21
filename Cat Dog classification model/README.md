# Dogs vs Cats Classification Model

This project contains a Jupyter Notebook that builds and trains a Convolutional Neural Network (CNN) to classify images as either cats or dogs using TensorFlow and Keras.

## Notebook

- `Dogs_vs_Cats_Classification_model.ipynb`

## Overview

The notebook performs the following steps:

1. Download the Dogs vs Cats dataset from Kaggle.
2. Extract the dataset into the working environment.
3. Load the training and validation image datasets from directories.
4. Normalize image pixel values from `[0, 255]` to `[0, 1]`.
5. Build a CNN model with convolutional, batch normalization, pooling, flattening, and dense layers.
6. Train the model for 10 epochs using binary cross-entropy.
7. Plot training and validation accuracy/loss curves.
8. Run inference on a sample image to predict whether it is a cat or a dog.

## Requirements

Make sure you have the following installed:

- Python 3.8+
- TensorFlow
- Keras
- matplotlib
- OpenCV
- Kaggle API credentials (`kaggle.json`)

## Installation

Install the required Python packages:

```bash
pip install tensorflow keras matplotlib opencv-python
```

## Setup

Before running the notebook, place your Kaggle API key file named `kaggle.json` in the working environment or upload it to the runtime.

The notebook uses the Kaggle dataset:

- `salader/dogs-vs-cats`

## Usage

1. Open `Dogs_vs_Cats_Classification_model.ipynb` in Jupyter Notebook or JupyterLab.
2. Run each cell in order.
3. Make sure the dataset is downloaded and extracted successfully.
4. Update the image path in the inference section to test your own image.

## Notes

- The notebook uses a simple CNN architecture suitable for learning image classification tasks.
- The model is trained for a basic demonstration and may be improved with more epochs, data augmentation, or a larger network.
- For inference, replace `/content/cat.jpg` with the actual path of your test image.
