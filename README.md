# Custom CNN for Image Classification

This project implements a custom Convolutional Neural Network (CNN) to classify images of flora and fauna into 10 categories. The solution is designed to be run in a Kaggle environment.

## Goal

The objective is to classify images from the provided dataset and achieve a high **weighted F1 score**, which is the evaluation metric for the competition. The solution is built from scratch, without the use of pre-trained weights or transformer models.

## Dependencies

The following Python libraries are required to run this code. These are standard packages that are typically pre-installed in Kaggle notebooks.

```python
import os
import cv2
import numpy as np
import pandas as pd
from sklearn.model_selection import train_test_split
from sklearn.metrics import f1_score
import tensorflow as tf
from tensorflow.keras.models import Sequential
from tensorflow.keras.layers import Conv2D, MaxPooling2D, Flatten, Dense, Dropout
from tensorflow.keras.preprocessing.image import ImageDataGenerator
```

## Methodology

### Data Preparation
The code uses `ImageDataGenerator` to handle the dataset. This utility preprocesses the images by normalizing pixel values and performing data augmentation (such as rotation and flipping) to improve the model's ability to generalize.

### Model Architecture
A Convolutional Neural Network (CNN) is used for image classification. This model is built from scratch and consists of several convolutional, pooling, and dense layers designed to learn and identify features in the images.

## How to Run

This code is designed for a Kaggle notebook environment.

1.  **Dataset:** Ensure the competition dataset is available at `/kaggle/input/deep-learning-practice-week-9-may-2025`.
2.  **Run Code:** Copy the Python script into a Kaggle notebook cell and execute it.
3.  **Output:** The script will train the model, make predictions, and generate a submission file named `21F3003230.csv`.

## Output File

* `21F3003230.csv`: Your prediction file in the required format (`Image_ID`, `Label`).
