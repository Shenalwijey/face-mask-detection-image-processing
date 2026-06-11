# face-mask-detection-image-processing
# 😷 Face Mask Detection using Image Processing & Machine Learning

---

## 📌 Overview

This project implements an automated **Face Mask Detection System** using traditional **Image Processing** and **Machine Learning** techniques.

The system analyzes facial images and classifies them into two categories:

- 😷 Mask
- 😀 No Mask

Instead of deep learning, this project uses a combination of **HOG Features**, **Color Histograms**, and a **Support Vector Machine (SVM)** classifier to achieve reliable mask detection with low computational cost.

---

## 📂 Dataset

The dataset used in this project was obtained from Kaggle.

🔗 Source:
https://www.kaggle.com/datasets/omkargurav/face-mask-dataset

Dataset Statistics:

- 😷 With Mask: 3,725 images
- 😀 Without Mask: 3,828 images
- 📊 Total Images: 7,553

The dataset contains face images of individuals wearing and not wearing face masks under different lighting conditions, facial poses, and backgrounds.

---

## 🎯 Features

- 😷 Detects whether a person is wearing a face mask
- 🖼️ Image preprocessing pipeline for noise reduction
- 📊 HOG (Histogram of Oriented Gradients) feature extraction
- 🎨 Color Histogram feature extraction
- 🤖 SVM classifier with RBF kernel
- 📈 Achieved **88.75% classification accuracy**
- ⚡ Lightweight solution without requiring GPU support

---

## 🧠 How It Works

### 1️⃣ Image Preprocessing

Each image undergoes several preprocessing steps:

- 📏 Resize images to **64 × 64 pixels**
- ⚫ Convert RGB images to grayscale
- 🌫️ Apply Gaussian Blur for noise reduction
- 📊 Perform Histogram Equalization for contrast enhancement
- ✨ Detect edges using Canny Edge Detection

---

### 2️⃣ Feature Extraction

Instead of using raw pixel values, meaningful features are extracted.

#### 📊 HOG Features

Histogram of Oriented Gradients captures:

- Face structure
- Edge information
- Texture patterns

These features help distinguish masked and unmasked faces.

#### 🎨 Color Histograms

Color Histogram features capture:

- Color distribution
- Intensity variations
- Mask color patterns

#### 🔗 Feature Fusion

Both feature sets are combined into a single:

**1664-dimensional feature vector**

---

### 3️⃣ Classification

#### 🤖 Support Vector Machine (SVM)

An SVM with an RBF Kernel is used to classify images.

Why SVM?

- ✅ Excellent binary classification performance
- ✅ Handles high-dimensional feature spaces
- ✅ Strong generalization capability
- ✅ Computationally efficient

---

### 4️⃣ Prediction

The trained model predicts:

- 😷 Mask
- 😀 No Mask

along with confidence scores for each prediction.

---

## 📈 Results & Insights

### 🎯 Test Accuracy

**88.75%**

### 📊 Confusion Matrix Summary

| Class | Correct | Incorrect |
|---------|---------|-----------|
| 😷 Mask | 676 | 69 |
| 😀 No Mask | 665 | 101 |

### 🔍 Key Observations

- ✅ Balanced performance across both classes
- ✅ HOG features effectively capture mask boundaries
- ✅ Color Histograms improve classification accuracy
- ⚡ Traditional machine learning achieves strong results without deep learning

---

## 🛠️ Tech Stack

- 🐍 Python
- 👁️ OpenCV
- 🔢 NumPy
- 🤖 Scikit-Learn
- 📊 Matplotlib
- 🖼️ Scikit-Image
- 📓 Jupyter Notebook

---

## 🚀 Applications

- 🏥 Hospitals and Healthcare Centers
- 🎓 Schools and Universities
- ✈️ Airports and Public Transportation
- 🏢 Workplace Safety Monitoring
- 🎥 Surveillance Systems

---

## 📚 Key Concepts

- Image Processing
- Histogram Equalization
- Canny Edge Detection
- HOG Feature Extraction
- Color Histograms
- Support Vector Machine (SVM)
- Binary Image Classification

---

## ⚠️ Limitations

- ❌ Does not locate faces before classification
- ❌ Cannot detect incorrectly worn masks
- ❌ Sensitive to extreme lighting conditions
- ❌ Resizing may remove fine facial details

---

## 🔮 Future Improvements

- 🚀 Real-time webcam-based mask detection
- 😀 Face Detection before classification
- 🧠 CNN-based feature extraction
- 📹 Live video stream monitoring
- 🎯 Mask position and correctness detection
- ⚡ Deep Learning models such as MobileNet and ResNet

---

## 🙌 Acknowledgements

- Kaggle Dataset Contributors
- OpenCV Documentation
- Scikit-Learn Documentation
- Computer Vision Research Community

---

## ⭐ Support

If you found this project useful, consider giving it a ⭐ on GitHub!

---
