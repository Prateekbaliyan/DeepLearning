# Case Study 3: Brain Tumor Detection using CNN

## Project Overview
This project implements a Convolutional Neural Network (CNN) to classify brain MRI images into two categories:
- Tumor
- No Tumor

The model analyzes MRI scans and predicts whether a brain tumor is present.

## Dataset
The dataset used is Brain MRI Images for Brain Tumor Detection.

Dataset structure:

brain_tumor_dataset/
    yes/
    no/

yes → MRI images with tumor  
no → MRI images without tumor

Images are resized to 224×224×3 before training.

## Data Preprocessing
- Image resizing to 224×224
- Pixel normalization (values between 0 and 1)
- Training-validation split using ImageDataGenerator

## Model Architecture

Input: 224×224×3

Conv2D (32 filters, 3×3) → ReLU  
MaxPooling (2×2)

Conv2D (64 filters, 3×3) → ReLU  
MaxPooling (2×2)

Conv2D (128 filters, 3×3) → ReLU  
MaxPooling (2×2)

Flatten

Dense (128 neurons) → ReLU

Output Layer (2 neurons) → Softmax

## Training Details
Optimizer: Adam  
Loss Function: Categorical Crossentropy  
Epochs: 10  
Evaluation Metric: Accuracy

## Libraries Used
- TensorFlow
- Keras
- NumPy
- Matplotlib

## Learning Outcomes
- CNN for medical image classification
- Image preprocessing techniques
- Training deep learning models
- Evaluating classification performance