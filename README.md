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
📊 Dataset

Dataset

Kaggle Chest X-Ray Images (Pneumonia)

Dataset contains

Normal Chest X-rays
Pneumonia Chest X-rays

Training, validation, and testing sets are used for model development.

⚙️ Technologies Used
Backend
Python
FastAPI
Scikit-Learn
Frontend
HTML
CSS
JavaScript
Tailwind CSS
Machine Learning
HOG
LBP
Random Forest
SVM
Gradient Boosting
SHAP
🚀 Installation

Clone repository

git clone https://github.com/username/Pneumonia-Detection-System.git

cd Pneumonia-Detection-System

Create virtual environment

python -m venv venv

Activate

Windows

venv\Scripts\activate

Linux

source venv/bin/activate

Install dependencies

pip install -r requirements.txt
🏃 Training
python src/train.py
🔍 Inference
python src/inference.py
📈 Performance
Metric	Score
Accuracy	93.9%
Precision	94.6%
Recall	97.1%
F1 Score	95.8%
ROC-AUC	98.2%
📸 Screenshots

Add screenshots here.

Home Page

Upload Interface

Prediction Result

Severity Analysis

SHAP Visualization
🔮 Future Improvements
Multi-class disease detection
COVID-19 Detection
Tuberculosis Detection
Mobile Application
PACS Integration
Cloud Deployment
👨‍💻 Authors

Developed as a B.Tech Final Year Project.

📜 License

This project is released under the MIT License.
