# Mask Images Classification

This project is a convolutional neural network (CNN) based image classifier that identifies whether a person 
in the image is wearing a mask or not.

## Installation

To run this project, you'll need to have the following dependencies installed:

- TensorFlow
- imghdr
- Matplotlib
- os

You can install these dependencies using pip:

pip install tensorflow imghdr matplotlib


## Usage

1. Download the provided model file ('maskdetectionmodel.h5`) and notebook (`image_classifier.ipynb`).
2. Upload the model file into your notebook environment.
3. Use the notebook to load the model and make predictions on images.

## Dataset

The dataset used for training this model is the FaceMask Dataset from Kaggle, supplemented with images from Unsplash.

## Model Architecture

The model architecture is a CNN with the following layers:
- Input layer: 16 filters, input size (256,256,3)
- Second layer: 32 filters
- Third layer: 16 filters with (3,3) kernel size
- Flatten layer
- Dense layer with 256 nodes, using "relu" activation
- Output layer with "sigmoid" activation for binary classification

## Training

The model was trained using the Adam optimizer and binary cross-entropy loss function.

## Evaluation

The model's performance was evaluated using accuracy, recall, and precision metrics.

# Results
this model classifies the images with or without mask with 99% accuracy 