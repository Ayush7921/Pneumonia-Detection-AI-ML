# 🫁 Pneumonia Detection System using Chest X-Rays through Machine Learning

Project website: [PNEUMONIA DETECTION](https://pneumonia-detector-pearl.vercel.app/#)


An intelligent web-based application that detects pneumonia from chest X-ray images using classical Machine Learning techniques. The system combines image preprocessing, handcrafted feature extraction, ensemble classification, and explainable AI to provide accurate, fast, and interpretable predictions.

---

## 📖 Overview

Pneumonia is one of the leading causes of respiratory-related deaths worldwide, especially among children and elderly patients. Accurate diagnosis from chest X-rays requires experienced radiologists, which may not always be available in rural or resource-constrained healthcare facilities.

This project provides an AI-assisted diagnosis system that analyzes chest X-ray images and predicts whether a patient is suffering from pneumonia. Unlike many deep learning-only approaches, this project focuses on an interpretable and lightweight machine learning pipeline that can be deployed efficiently without requiring high-end GPU infrastructure.

---

## ✨ Key Features

- 🩻 Chest X-ray image upload
- ✅ Four-layer X-ray validation system
- 🎨 CLAHE-based image enhancement
- 📊 HOG (Histogram of Oriented Gradients) feature extraction
- 🧩 LBP (Local Binary Pattern) feature extraction
- ⚖️ Feature normalization using StandardScaler
- 🤖 Ensemble Machine Learning classifier
- 📈 Pneumonia severity scoring
- 🔍 SHAP-based explainability
- 📄 PDF report generation
- 🌐 FastAPI backend
- 💻 Responsive web interface
- ☁️ Serverless deployment

---

# 🏗️ System Workflow

```
Chest X-ray Upload
        │
        ▼
4-Layer Image Validation
        │
        ▼
Image Preprocessing (CLAHE)
        │
        ▼
Feature Extraction
(HOG + LBP + Statistical Features)
        │
        ▼
Feature Scaling
(StandardScaler)
        │
        ▼
Ensemble Classifier
(SVM + Random Forest + Gradient Boosting)
        │
        ▼
Prediction
        │
        ▼
Severity Analysis
        │
        ▼
SHAP Explainability
        │
        ▼
Result & PDF Report
```

---

# 🧠 Machine Learning Pipeline

### Image Preprocessing

- Grayscale Conversion
- Image Resizing
- CLAHE Contrast Enhancement
- Image Normalization

### Feature Extraction

The model extracts multiple handcrafted features including:

- Histogram of Oriented Gradients (HOG)
- Local Binary Patterns (LBP)
- Multi-region LBP
- Statistical Features
- Lung Symmetry Features
- Gradient Energy Features

### Classification

The final prediction is generated using a Soft Voting Ensemble consisting of:

- Support Vector Machine (SVM)
- Random Forest
- Gradient Boosting Classifier

---

# 📊 Dataset

**Dataset Used**

Kaggle Chest X-Ray Images (Pneumonia)

The dataset contains chest X-ray images categorized into:

- Normal
- Pneumonia

The model is trained using separate training, validation, and testing datasets.

---

# 💻 Technology Stack

### Programming Language

- Python

### Backend

- FastAPI

### Frontend

- HTML
- CSS
- JavaScript
- Tailwind CSS

### Machine Learning

- Scikit-learn
- OpenCV
- NumPy
- Pandas
- SHAP

---

# 📁 Repository Structure

readMe file
Main Project Report (39+ pages) – complete methodology, architecture, HOG + LBP, Random Forest, SHAP, FastAPI, results, etc.
Layman Guide (12 pages) – project ko simple language me explain karta hai, end-to-end pipeline ke saath.
Abstract/Report Copy – detailed report with objectives, methodology, implementation, and evaluation.
Technical Summary (7 pages) – concise summary of dataset, preprocessing, ensemble model, performance metrics, deployment, and tech stack.
---

# 🚀 Installation

Clone the repository

```bash
git clone https://github.com/your-username/Pneumonia-Detection-System.git
```

Move into the project directory

```bash
cd Pneumonia-Detection-System
```

Create a virtual environment

```bash
python -m venv venv
```

Activate the environment

### Windows

```bash
venv\Scripts\activate
```

### Linux / macOS

```bash
source venv/bin/activate
```

Install all dependencies

```bash
pip install -r requirements.txt
```

---

# ▶️ Run the Project

### Train the Model

```bash
python src/train.py
```

### Run Inference

```bash
python src/inference.py
```

### Start FastAPI Server

```bash
uvicorn api:app --reload
```

---

# 📈 Performance

| Metric | Value |
|----------|--------|
| Accuracy | 93.92% |
| Precision | 94.65% |
| Recall | 97.16% |
| F1 Score | 95.89% |
| ROC-AUC | 98.26% |

---

# 📸 Project Screenshots

> Add screenshots of your application here.

- Home Page
  <img width="2520" height="1432" alt="image" src="https://github.com/user-attachments/assets/c1bf50a3-75cf-4d7a-9383-692bf2492ac3" />

- Upload Interface
- Prediction Result
- Severity Analysis
- Explainability Heatmap

---

# 🌍 Future Improvements

- Multi-class disease detection
- COVID-19 detection
- Tuberculosis detection
- Mobile application
- PACS integration
- Cloud deployment
- Real-time hospital integration

---

# 🤝 Contributors

Developed as a B.Tech Major Project.

---

# 📜 License

This project is intended for educational and research purposes.

---

## ⭐ If you found this project useful, don't forget to star the repository.
