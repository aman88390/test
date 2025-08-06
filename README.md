# Image Classification for Flora and Fauna

This project aims to classify images of animals and plants into 10 distinct categories. The goal is to achieve the best possible **weighted F1 score** on the test dataset.

**Important Note:** The solution is developed from scratch, without using transfer learning or transformer models, as per competition rules.

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
