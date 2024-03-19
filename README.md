# Dental X-ray Image Segmentation using U-Net
This repository contains a TensorFlow implementation of a U-Net model for segmenting inferior alveolar nerve and third molars in dental panoramic X-ray images.

## Overview
Dental panoramic X-ray images are crucial for diagnosing various dental conditions. Automated segmentation of anatomical structures in these images can aid in accurate diagnosis and treatment planning. This project focuses on segmenting the inferior alveolar nerve and third molars using a U-Net model, a popular architecture for semantic segmentation tasks.

## Model Architecture
The implemented U-Net model consists of a contracting path (encoding) and an expanding path (decoding) to capture features at different levels of abstraction. The model is built using TensorFlow's Keras API. Here's a brief overview of the architecture:

Contracting Path: This part of the model captures the context and reduces the spatial dimensions of the input image through a series of convolutional blocks.

Expanding Path: This section upsamples the feature maps and combines them with feature maps from the contracting path to produce high-resolution segmentation masks.

## Usage
Dataset Preparation: Ensure your dataset containing dental panoramic X-ray images and corresponding segmentation masks is structured properly. Update the image_path and mask_path variables in the code to point to the directories containing images and masks, respectively.

**Model Configuration**: You can adjust various parameters of the U-Net model, such as input size, number of filters, and number of classes, according to your requirements.

**Training**: Configure training parameters such as number of epochs, batch size, and buffer size. Then, run the training script to train the U-Net model on your dataset.

**Evaluation**: Evaluate the trained model using appropriate metrics to assess its performance on segmentation tasks.

## Dependencies
TensorFlow 2.x 
NumPy 
Matplotlib
