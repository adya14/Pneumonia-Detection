# Pneumonia Detection Using Convolutional Neural Networks

This project detects pneumonia in chest X-ray images using a Convolutional Neural Network (CNN). The model is trained and evaluated on the **Chest X-Ray Images (Pneumonia)** dataset sourced from Kaggle. It classifies images as either `NORMAL` or `PNEUMONIA`.

## Table of Contents
- [Dataset](#dataset)
- [Project Workflow](#project-workflow)
- [Model Architecture](#model-architecture)
- [Results](#results)
- [Achievements](#achievements)

## Dataset

The dataset is obtained from Kaggle: [Chest X-Ray Images (Pneumonia)](https://www.kaggle.com/paultimothymooney/chest-xray-pneumonia).

- **Classes:** `NORMAL` and `PNEUMONIA`
- **Train/Test/Validation Split:** Predefined in the dataset
- **Image Size:** Resized to 224x224 pixels for uniformity

## Project Workflow

1. **Data Preprocessing**: Images were resized to (224, 224) and normalized.
2. **Model Development**: A CNN was built using TensorFlow/Keras with layers for feature extraction and classification.
3. **Training**: The model was trained using a `categorical_crossentropy` loss function and `Adam` optimizer for 20 epochs.
4. **Evaluation**: Performance metrics such as accuracy and loss were calculated on the test set.
5. **Visualization**: Confision Matrix.

## Model Architecture

The CNN architecture consists of:
- Convolutional layers for feature extraction with ReLU activation.
- MaxPooling layers to downsample the feature maps.
- Flatten layer to convert 2D features into a 1D vector.
- Dense layers for classification with Dropout for regularization.
- Output layer with a Softmax activation for binary classification.

### Model Summary
- `Conv2D` -> `MaxPooling2D` -> `Conv2D` -> `MaxPooling2D` -> `Conv2D` -> `Flatten` -> `Dense` -> `Dropout` -> `Dense`

## Results

- **Training Accuracy:** 99%
- **Test Accuracy:** 95%

## Achievements

This model provides a robust solution for detecting pneumonia in chest X-ray images, helping healthcare professionals quickly identify patients at risk. With high accuracy, it can assist in early diagnosis, leading to timely treatment and potentially saving lives, especially in resource-limited settings.


