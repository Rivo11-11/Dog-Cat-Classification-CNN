# Dog-Cat-Classification-CNN

## Link to Kaggle : https://www.kaggle.com/code/rafik11/cnn-data-augmentation/notebook
This repository contains a complete pipeline for identifying dog-cats from images using deep learning techniques. The project uses CNN + Image Augmentation
## Table of Contents

1. [Data Exploration & Analysis](#data-exploration--analysis)
2. [Data Preprocessing](#data-preprocessing)
3. [Model Training](#model-training)
4. [Evaluation & Prediction](#evaluation--prediction)
5. [Submission](#submission)

## Data Exploration & Analysis

The dataset consists of images labeled dog and cat as the name of the file image. The exploration includes:
- Analyzing the distribution of the 2 class.
- Visualizing a subset of images to understand the data.
- Encoding labels for model training 1 (dog) 0 (cat) .



## Data Preprocessing

Data preprocessing involves:
- Loading and resizing images to a standard size (224x224 pixels).
- Label encoding the class names.
- using data generator

The `load_data` function processes images and labels, preparing them for model training and validation.

## Model Training

The model training involves:
- Creating a data augmentation pipeline using `ImageDataGenerator` to improve model generalization.
- Training a deep learning model via CNN  convolution net (extracting features of image) Dense net (last layer a single neuron sigmoid).

The training process includes:
- Configuring and compiling the model.
- Using data augmentation to improve performance.
- Monitoring training and validation loss and accuracy using callbacks.

## Evaluation & Prediction

After training, the model is evaluated on a validation set and predictions are generated for test images. Key steps include:
- Loading and preprocessing test images.
- Generating predictions using the trained model.
- Displaying some predictions along with the images.
