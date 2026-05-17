# Computer Vision Problem Formulation and CNN Prototype

## Project Overview
This project focuses on building a basic Convolutional Neural Network (CNN) model for an image-based dataset. The objective is to understand how CNNs process images using convolution, pooling, activation functions, and dense layers to classify images into different categories.

## Problem Type
The dataset represents an **Image Classification** problem.

The images are organized into four separate classes:
- dent
- normal
- scratch
- stain

Since each image belongs to exactly one category, the task is to classify the input image into one of these classes.

## Dataset Exploration
The dataset contains four classes:
- dent
- normal
- scratch
- stain

Each class contains image samples of surface conditions. The dataset was explored by:
- Counting number of classes
- Counting number of images per class
- Displaying sample images
- Checking image dimensions
- Observing dataset balance

The dataset is balanced because all classes contain similar numbers of images.

## Image Preprocessing
The following preprocessing steps were applied:
- Resized all images to 128 × 128 pixels
- Normalized pixel values to range 0–1
- Split data into training and validation sets
- Applied data augmentation such as rotation, zoom, and horizontal flip

## CNN Model Architecture
A CNN model was built using TensorFlow/Keras.

The model includes:
- Convolution layers
- ReLU activation function
- MaxPooling layers
- Flatten layer
- Dense layer
- Softmax output layer

## Model Training and Evaluation
The CNN model was trained on the image dataset and evaluated on validation data.

Evaluation included:
- Training accuracy and loss
- Validation accuracy and loss
- Confusion matrix
- Sample predictions on test images

The model successfully learned image patterns and classified the four categories.

## CNN Concept Explanation

### What is convolution?
Convolution is the process of applying filters to images to detect patterns such as edges, textures, and shapes.

### Why is pooling used?
Pooling reduces image size while preserving important features, which improves efficiency.

### Why is ReLU commonly used?
ReLU introduces non-linearity and helps the model learn complex patterns faster.

### Why are CNNs better than regular feed-forward networks for image data?
CNNs automatically learn spatial features from images and require fewer parameters than traditional neural networks.

## Business Use Case Mapping
This computer vision solution can be applied in manufacturing.

For example, in automobile manufacturing, CNN models can automatically detect defects such as dents, scratches, and stains on vehicle surfaces. This improves quality inspection and reduces manual effort.

## Files Included
- notebook.ipynb
- README.md
- requirements.txt
- results/

## Technologies Used
- Python
- TensorFlow
- Keras
- NumPy
- Matplotlib
- Pandas
- Scikit-learn
