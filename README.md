# AI-based Tool for Preliminary Diagnosis of Dermatological Manifestations

## Smart India Hackathon 2023

### Team: Data_Riders_KGP

- Ritam Mondal (Team Leader)
- Soumyadip Biswas
- Chiradip Biswas
- Devodita Chakravarty
- Shamik Bhattacharjee
- Shalin Chakraborty

## Project Overview

This project aims to develop an AI-based tool for the preliminary diagnosis of dermatological manifestations. We are using Convolutional Neural Networks (CNN) to analyze dermatoscopic images and provide initial assessments of skin conditions.

## Dataset

We are using the HAM10000 dataset from Kaggle, which consists of 10,015 dermatoscopic images. The dataset is divided into three segments:

1. Train
2. Test
3. Cross-Validation

## Image Processing

Our image processing pipeline includes:

1. Loading the image using OpenCV's imread function
2. Preprocessing techniques to standardize images for CNN compatibility
3. Feature extraction (when necessary)
4. Reshaping and formatting images into 28x28x3 matrices (3 channels for RGB)

## Data Augmentation

We implement data augmentation techniques to artificially increase our dataset size and improve model performance. This is achieved using the Keras preprocessing image library in TensorFlow, which includes functions for rotation, zoom, flip, and contrast adjustments.

Benefits of data augmentation include:
- Enhanced model performance by reducing overfitting
- Improved model robustness
- Reduced data collection costs

## Convolutional Neural Network (CNN)

We chose to use a CNN for this project due to its advantages in image classification:

1. Reduced number of input nodes
2. Tolerance for small shifts in images
3. Utilization of pixel correlations for classification
4. Lower memory usage compared to traditional networks

Our CNN implementation includes:
- Input data processing
- Application of filters (kernels)
- Convolution operations
- Summation of results
