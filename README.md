# 🫁 Pneumonia Detection System using Chest X-Rays through Machine Learning

Project website: [PNEUMONIA DETECTION](https://pneumonia-detector-pearl.vercel.app/#)


An AI-powered web application for detecting pneumonia from chest X-ray images using classical machine learning techniques. The system combines advanced image preprocessing, handcrafted feature extraction, ensemble learning, and explainable AI to provide fast, reliable, and interpretable predictions.

---

## 📌 Overview

Pneumonia is one of the leading causes of death worldwide, particularly among children and elderly patients. Early diagnosis is essential but requires experienced radiologists.

This project provides an automated decision support system that analyzes chest X-ray images and predicts whether pneumonia is present.

Unlike deep learning-only approaches, this system combines handcrafted image descriptors with ensemble machine learning to improve interpretability while maintaining high accuracy.

---

## ✨ Features

- Chest X-ray upload
- Image validation pipeline
- CLAHE image enhancement
- Histogram of Oriented Gradients (HOG)
- Local Binary Pattern (LBP)
- Feature normalization
- Ensemble Machine Learning classifier
- Pneumonia severity estimation
- Explainable AI (SHAP)
- FastAPI backend
- Responsive web interface
- PDF report generation
- Serverless deployment

---

## 🏗️ System Pipeline

```

Upload Chest X-ray
↓
Image Validation
↓
CLAHE Preprocessing
↓
Feature Extraction
(HOG + LBP)
↓
Feature Scaling
↓
Ensemble Classifier
↓
Prediction
↓
Severity Analysis
↓
SHAP Explainability
↓
Generate Report

```

---

## 🧠 Machine Learning Pipeline

### Image Preprocessing

- Convert to grayscale
- Resize images
- CLAHE enhancement
- Normalization

---

### Feature Extraction

The model extracts multiple handcrafted features including

- Histogram of Oriented Gradients (HOG)
- Local Binary Pattern (LBP)
- Statistical Features
- Lung Symmetry Features
- Gradient Energy Features

---

### Classification

Ensemble Model consisting of

- Support Vector Machine
- Random Forest
- Gradient Boosting

Final prediction is obtained using Soft Voting.

---

## 📂 Project Structure

```

Pneumonia-Detection-System/
│
├── README.md
├── requirements.txt
├── .gitignore
│
├── src/
│ ├── train.py
│ ├── inference.py
│ ├── preprocess.py
│ ├── features.py
│ ├── model.py
│ ├── dataset.py
│ ├── validation.py
│ └── utils.py
│
├── data/
│ ├── download_data.py
│ ├── preprocess.py
│ └── README.md
│
├── models/
│
├── notebooks/
│
└── tests/

