# Brain Tumor Classification Challenge

A deep learning model for classifying brain MRI images into four categories: **Glioma**, **Meningioma**, **Pituitary**, or **No Tumor**, built using PyTorch.

## Overview

This project was developed as part of the **Sprint AI Training for African Medical Imaging Knowledge Translation Challenge**. The dataset contains labeled MRI scans, and the goal was to train a model capable of generalizing to unseen data.

## Task

- Classify MRI images into one of the following categories:
  - `0` - Glioma
  - `1` - Meningioma
  - `2` - No Tumor
  - `3` - Pituitary Tumor

## Dataset

MRI scan images with corresponding labels for tumor classification. Data was provided as part of the competition and preloaded in the Kaggle environment.

## Approach

- **Data Preprocessing**: Image resizing, normalization, and augmentation using `torchvision.transforms`.
- **Model Architecture**: A custom Convolutional Neural Network built with PyTorch.
- **Training**: CrossEntropyLoss and Adam optimizer.
- **Evaluation Metrics**: Accuracy and F1 Score.

## Results

The final model achieved:

- **Accuracy**: `0.97` on the private leaderboard
- **Evaluation Metric**: F1 Score (harmonic mean of precision and recall)

## Submission Format

Predictions were submitted in the following CSV format:

```csv
image_name,label
img_001.jpg,0
img_002.jpg,3
img_003.jpg,2
...
