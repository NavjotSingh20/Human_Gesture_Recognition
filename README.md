# 🖊️ Handwritten Digit Recognition using Machine Learning & Deep Learning

This project implements and compares multiple machine learning and deep learning models for handwritten digit recognition using the **MNIST dataset**.

The objective of this project is to analyze the impact of different algorithms and hyperparameter settings on image classification performance.

The implemented models include:

- K-Nearest Neighbors (KNN)
- Support Vector Machine (SVM)
- Convolutional Neural Network (CNN)

Each model was trained with different configurations and evaluated using test accuracy and confusion matrices.

---

## 📌 Project Overview

Handwritten digit recognition is a classic computer vision problem where a model learns to classify grayscale images of handwritten digits (0-9).

This project explores how traditional machine learning approaches compare with deep learning methods for image classification.

---

## 🛠️ Technologies Used

- Python
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- TensorFlow / Keras
- Jupyter Notebook

---

## 🧪 Dataset

### MNIST Handwritten Digit Dataset

- **Total Images:** 70,000
- **Training Images:** 60,000
- **Testing Images:** 10,000
- **Image Size:** 28 × 28 pixels
- **Image Type:** Grayscale
- **Classes:** Digits 0-9

Each image is represented as pixel intensity values and classified into one of the ten digit categories.

---

## ⚙️ Data Preprocessing

The following preprocessing steps were performed:

- Normalization of pixel values to the range **[0,1]**
- Train-test split for model evaluation
- Reshaping images for CNN input
- One-hot encoding of labels for CNN training

---

# 🤖 Models Implemented

## 1. K-Nearest Neighbors (KNN)

Two different values of k were tested:

| Configuration | Value |
|---|---|
| Model 1 | k = 3 |
| Model 2 | k = 7 |

KNN classifies images based on similarity with neighboring data points.

---

## 2. Support Vector Machine (SVM)

Different kernels and regularization values were evaluated:

| Configuration | Value |
|---|---|
| Model 1 | Linear Kernel, C = 1 |
| Model 2 | RBF Kernel, C = 10 |

SVM was used to analyze the performance of linear and non-linear decision boundaries.

---

## 3. Convolutional Neural Network (CNN)

A CNN model was implemented using TensorFlow/Keras.

Configurations tested:

| Configuration | Parameters |
|---|---|
| Model 1 | 32 convolution filters, Adam optimizer |
| Model 2 | 64 convolution filters, Learning Rate = 0.0005 |

CNN learns spatial patterns from image pixels and achieves higher classification performance compared to traditional ML models.

---

# 📊 Evaluation Metrics

Each model was evaluated using:

### Accuracy Score

Measures the percentage of correctly classified images.

### Confusion Matrix

Used to analyze:
- Correct predictions
- Misclassified digits
- Class-wise model performance

---

# 🏆 Results Summary

| Model | Configuration | Test Accuracy |
|---|---|---|
| KNN | k = 3 | **97.0%** |
| KNN | k = 7 | 96.8% |
| SVM | Linear Kernel, C = 1 | 91.0% |
| SVM | RBF Kernel, C = 10 | **96.7%** |
| CNN | 32 Filters | **98.7%** |
| CNN | 64 Filters | 98.55% |

---

# 📈 Observations

- KNN achieved strong performance due to the similarity-based nature of handwritten digits.
- RBF kernel SVM performed significantly better than Linear SVM due to its ability to capture non-linear patterns.
- CNN achieved the highest accuracy by automatically extracting important image features.

---
