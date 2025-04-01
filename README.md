# 🩺 Cirrhosis Outcome Classification and Deployment

## 📌 Project Overview
This project aims to predict patient outcomes for cirrhosis based on clinical features using supervised machine learning models. The goal is to build a reliable, interpretable, and deployable model that can help in early prognosis and guide treatment planning.

**Project features:**
- Data preprocessing and feature engineering
- Multi-class classification modeling (Random Forest, LightGBM)
- Model evaluation and SHAP explainability
- REST API via Flask
- Interactive frontend with React
- Docker containerization and AWS EC2 deployment

---

## 📊 Dataset
The dataset is derived from a public clinical study on liver cirrhosis. It contains:
- **Demographics**: Age, Sex  
- **Clinical data**: Bilirubin, Albumin, Prothrombin Time  
- **Target**: Patient outcome (multi-class label)

---

## 🧠 Model Development
- **Algorithms**: Random Forest, LightGBM  
- **Techniques**: ML-based missing value imputation, log/Box-Cox transformations, hyperparameter tuning  
- **Evaluation**: Accuracy, Macro F1  
- **Result**: Achieved ~25% improvement over baseline

---

## ⚙️ MLOps & Engineering
- **API**: Flask RESTful service for real-time predictions  
- **Experiment Tracking**: MLflow for logging and version control  
- **Containerization**: Docker for backend packaging  
- **Deployment**: Hosted on AWS EC2

---

## 🌐 Frontend
Built with **React**, the web app allows users to:
- Input patient clinical features
- View predicted outcome and class probabilities
- Visualize feature importance via SHAP

---

## 🔍 Model Explainability
- SHAP integrated for interpreting model decisions
- Interactive feature contribution plots on the web interface

---

## 🚀 Quick Start

### Clone and Run Backend
```bash
git clone https://github.com/RobertWei3/cirrhosis-end-to-end.git
cd cirrhosis-classification-app/backend

# Build Docker image
docker build -t cirrhosis-api .

# Run the API
docker run -p 5000:5000 cirrhosis-api
