# Maize Leaf Disease Detection Using Deep Convolutional Neural Networks

> A deep learning-powered computer vision system that automatically detects and classifies maize leaf diseases from images using TensorFlow and Convolutional Neural Networks (CNNs).

![Python](https://img.shields.io/badge/Python-3.10+-blue)
![TensorFlow](https://img.shields.io/badge/TensorFlow-Deep%20Learning-orange)
![Keras](https://img.shields.io/badge/Keras-CNN-red)

---

# Overview

Plant diseases significantly reduce agricultural productivity and crop yield worldwide. Early detection enables farmers to prevent disease spread and improve harvest quality.

This project develops a **deep learning image classification model** capable of recognizing multiple maize leaf diseases from images using **Convolutional Neural Networks (CNNs)**.

The model learns visual patterns directly from thousands of labeled maize leaf images without manual feature extraction.

---

# Features

- Automatic maize leaf disease detection
- Deep Convolutional Neural Network
- Multi-class image classification
- Image preprocessing pipeline
- Data augmentation
- Confidence-based predictions
- Model evaluation on unseen data
- TensorFlow/Keras implementation

---

# Dataset

The model was trained using the **Corn or Maize Leaf Disease Dataset** published on Kaggle by **Smaranjit Ghose**.

The dataset contains approximately **4,188 labeled maize leaf images** across four classes:

| Class | Number of Images |
|--------|-----------------:|
| Common Rust | 1,306 |
| Gray Leaf Spot | 574 |
| Blight | 1,146 |
| Healthy | 1,162 |
| **Total** | **4,188** |

Images were automatically loaded using TensorFlow's `image_dataset_from_directory()` API.

### Dataset Preprocessing

The preprocessing pipeline includes:

- Image resizing
- Pixel normalization
- Dataset shuffling
- Data augmentation
- Train/Validation/Test split (80% / 10% / 10%)
- Dataset caching and prefetching for faster training

The dataset is derived from the **PlantVillage** and **PlantDoc** datasets and is widely used for research in plant disease classification.

**Dataset Link**

https://www.kaggle.com/datasets/smaranjitghose/corn-or-maize-leaf-disease-dataset

---

# Deep Learning Pipeline

```

Image Dataset

↓

Image Preprocessing

↓

Data Augmentation

↓

CNN Model

↓

Training

↓

Evaluation

↓

Disease Prediction

```

---

# CNN Architecture

The model consists of:

- Input Layer
- Convolution Layers
- ReLU Activation
- Max Pooling Layers
- Dense Fully Connected Layers
- Softmax Output Layer

The network automatically extracts disease-related visual features from maize leaf images.

---

# Data Preprocessing

The preprocessing pipeline includes:

- Image resizing
- Pixel normalization
- Dataset caching
- Prefetching
- Random image augmentation
- Dataset splitting

---

# Model Training

Training configuration includes:

- TensorFlow/Keras
- Adam Optimizer
- Sparse Categorical Crossentropy Loss
- Accuracy Metric
- 50 Training Epochs

---

# Model Evaluation

The trained model was evaluated on previously unseen images to measure classification performance.

Evaluation metrics include:

- Classification Accuracy
- Validation Accuracy
- Prediction Confidence

---

# Results

The trained CNN demonstrated strong performance on the maize leaf disease classification task.

| Metric | Value |
|--------|------:|
| Training Accuracy | **93%** |
| Dataset Size | **4,188 Images** |
| Classes | **4** |
| Framework | **TensorFlow / Keras** |

The model successfully learned discriminative visual features from maize leaf images, enabling accurate classification of healthy leaves and multiple disease categories.

# Prediction

The trained CNN predicts the disease class of a maize leaf image and returns:

- Predicted Disease
- Prediction Confidence
- Class Probability

---

# Technologies Used

- Python
- TensorFlow
- Keras
- NumPy
- Matplotlib
- Jupyter Notebook

---

# Project Structure

```

Maize-Leaf-Disease-Detection/

│

├── Maize\_Leaf\_Detection.ipynb

├── Dataset/

├── Models/

├── Images/

└── README.md

```

---

# Installation

Clone the repository

```bash
git clone https://github.com/OsimeSado/Plant-Disease-Detection.git

cd Plant-Disease-Detection
```

Install dependencies

```bash
pip install tensorflow matplotlib numpy
```

Launch Jupyter Notebook

```bash
jupyter notebook
```

Open

```
Maize_Leaf_Detection.ipynb
```

---

# 📷 Sample Workflow

```

Leaf Image

↓

CNN Model

↓

Feature Extraction

↓

Disease Classification

↓

Prediction Confidence

```

---

# Future Improvements

- Mobile application deployment
- Real-time camera disease detection
- Transfer Learning (EfficientNet / ResNet)
- Larger disease datasets
- Web application interface
- Cloud deployment

---

# Author

**Osimeozemeokhai T. Sado**

Computer Engineer • Machine Learning Engineer • AI Enthusiast

GitHub: https://github.com/OsimeSado

---
