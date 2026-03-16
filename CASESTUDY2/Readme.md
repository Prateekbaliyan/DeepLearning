# Case Study 2: CNN-based Image Classification on CIFAR-10

## Project Overview
This project implements a Convolutional Neural Network (CNN) to classify images from the CIFAR-10 dataset. 
The model learns visual features from images and predicts the correct category among ten classes.

## Dataset
The CIFAR-10 dataset contains 60,000 RGB images of size 32×32×3.

Dataset split:
- 50,000 training images
- 10,000 testing images

Classes in the dataset:
1. Airplane
2. Automobile
3. Bird
4. Cat
5. Deer
6. Dog
7. Frog
8. Horse
9. Ship
10. Truck

The dataset is loaded directly using the TensorFlow/Keras datasets API.

## Model Architecture

Input: 32×32×3

Conv2D (32 filters, 3×3) → ReLU  
MaxPooling (2×2)

Conv2D (64 filters, 3×3) → ReLU  
MaxPooling (2×2)

Conv2D (64 filters, 3×3) → ReLU

Flatten

Dense (128 neurons) → ReLU

Output Layer (10 neurons) → Softmax

## Training Details
Optimizer: Adam  
Loss Function: Sparse Categorical Crossentropy  
Epochs: 10  
Evaluation Metric: Accuracy

## Libraries Used
- TensorFlow
- Keras
- NumPy
- Matplotlib

## Learning Outcomes
- Understanding CNN architecture
- Image feature extraction
- Training deep learning models
- Evaluating classification performance