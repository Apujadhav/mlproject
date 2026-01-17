# 🎓 Student Performance Prediction System

**Academic Machine Learning Project – End-to-End Implementation**

A complete **Machine Learning–powered prediction system** that estimates **student academic performance** using demographic, social, and educational attributes, with a fully modular ML pipeline and web-based inference.

---

## 📖 Project Overview

This project simulates a real-world **education analytics system** where understanding and predicting student outcomes is critical.

The system ensures:
- Structured data analysis through EDA
- Training and comparison of multiple ML models
- Selection of the best-performing model
- Persistent storage of trained artifacts
- Real-time prediction via a web application

All components are designed following **industry-aligned ML engineering practices**.

---

## 🧠 Problem Statement

Student academic performance is influenced by multiple interdependent factors such as:
- Parental education level
- Test preparation status
- Gender and socio-economic background

The objective of this project is to **predict a student’s final score** using supervised machine learning and provide predictions through a user-friendly interface.

---

## 🔍 Exploratory Data Analysis (EDA)

EDA was conducted to understand feature distributions, correlations, and performance drivers.

### Key Observations:
- Students completing **test preparation courses** perform significantly better
- **Parental education level** shows strong correlation with student scores
- Math, Reading, and Writing scores are highly correlated
- Score distributions are approximately normal with minimal outliers

EDA includes:
- Univariate and multivariate analysis
- Correlation heatmaps
- Distribution plots and boxplots

---

## 🤖 Machine Learning Implementation

### 🔹 ML Task
- **Type:** Regression
- **Target Variable:** Student Final Score

### 🔹 Models Implemented
- Linear Regression
- Decision Tree Regressor
- Random Forest Regressor
- Gradient Boosting Regressor
- AdaBoost Regressor
- XGBoost Regressor
- CatBoost Regressor

### 🔹 Model Selection Strategy
- Hyperparameter tuning performed using grid-based search
- Models evaluated using **R² score**
- Best-performing model selected and persisted for inference

---

## 🚀 Web Application

A **Flask-based web application** enables real-time prediction of student performance.

### Features:
- Clean HTML-based user interface
- Real-time prediction results
- Trained model loaded from saved artifacts
- Modular preprocessing and inference pipeline

---

## 🛠️ Technology Stack

| Layer | Technologies |
|------|-------------|
| Language | Python |
| Data Analysis | Pandas, NumPy |
| Visualization | Matplotlib, Seaborn |
| Machine Learning | Scikit-learn, CatBoost, XGBoost |
| Backend | Flask |
| Frontend | HTML (Jinja Templates) |
| Packaging | setup.py, requirements.txt |
| Deployment | AWS (Planned) |

---

## 📂 Project Structure

mlproject/
├── artifacts/ # Trained models & preprocessors
├── catboost_info/ # CatBoost training logs
├── notebook/ # EDA & model training notebooks
│ ├── EDA STUDENT PERFORMANCE.ipynb
│ └── MODEL TRAINING.ipynb
├── src/ # Modular ML pipeline
├── templates/ # HTML templates
├── app.py # Flask application
├── application.py # App entry point
├── requirements.txt
├── setup.py
└── README.md

yaml
Copy code

---

## ⚙️ Setup & Run Instructions

### 🔹 Prerequisites
- Python 3.8+
- pip
- Git

---

### 🔹 Local Setup

```bash
git clone https://github.com/Apujadhav/mlproject.git
cd mlproject
python -m venv venv
Activate virtual environment:

Windows

bash
Copy code
venv\Scripts\activate
Install dependencies:

bash
Copy code
pip install -r requirements.txt
Run the application:

bash
Copy code
python app.py
Application runs at:

cpp
Copy code
http://127.0.0.1:5000
📈 Results
Achieved strong R² score on test data

Ensemble and boosting models outperformed baseline regression models

Selected model demonstrates stable and consistent predictions

End-to-end pipeline is deployment-ready

🧩 Future Enhancements
☁️ AWS Elastic Beanstalk deployment

🐳 Docker containerization

📊 Model monitoring and logging

📈 Performance visualization dashboard

👤 Author
Apurva Jadhav
Final Year Computer Engineering Student
