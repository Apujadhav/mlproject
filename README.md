# 🎓 Student Performance Prediction System

**End-to-End Machine Learning Project | Academic & Placement Portfolio**

A complete **Machine Learning-based prediction system** that estimates **student academic performance** using demographic, social, and educational attributes.  
This project follows the **full ML lifecycle** from **EDA and model training** to **web-based inference using Flask**.

---

## 📖 Project Overview

This project simulates a real-world **education analytics system** where understanding and predicting student outcomes is critical.

The system includes:
- Exploratory Data Analysis (EDA)
- Data ingestion and preprocessing pipelines
- Training and comparison of multiple ML models
- Hyperparameter tuning and model selection
- Persistent storage of trained artifacts
- Real-time prediction using a Flask web application

---

## 🧠 Problem Statement

Student academic performance is influenced by multiple factors such as:
- Parental education level
- Test preparation status
- Gender and socio-economic background

The objective is to **predict a student’s final score** using supervised machine learning and expose predictions through a user-friendly web interface.

---

## 🔍 Exploratory Data Analysis (EDA)

EDA was conducted to understand feature distributions and relationships.

### Key Insights:
- Students completing **test preparation courses** perform better
- **Parental education level** has a strong impact on scores
- Math, Reading, and Writing scores are highly correlated
- Score distributions are approximately normal

EDA notebooks are available inside the `notebook/` directory.

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
- Hyperparameter tuning for ensemble models
- Evaluation using **R² Score**
- Best-performing model saved as an artifact

---

## 🚀 Web Application

A **Flask-based web application** allows users to input student details and receive real-time performance predictions.

### Features:
- Simple HTML-based UI
- Real-time prediction output
- Model and preprocessor loaded from saved artifacts
- Modular prediction pipeline

---

## 🛠️ Tech Stack

| Layer | Technologies |
|------|-------------|
| Language | Python |
| Data Analysis | Pandas, NumPy |
| Visualization | Matplotlib, Seaborn |
| Machine Learning | Scikit-learn, CatBoost, XGBoost |
| Backend | Flask |
| Packaging | setup.py, requirements.txt |
| Deployment | AWS (Planned) |

---

## 📂 Project Structure

```text
mlproject/
├── .ebextensions/
│   └── python.config
├── artifacts/
│   ├── data.csv
│   ├── train.csv
│   ├── test.csv
│   ├── model.pkl
│   └── preprocessor.pkl
├── catboost_info/
├── logs/
├── notebook/
│   ├── 1. EDA STUDENT PERFORMANCE.ipynb
│   └── 2. MODEL TRAINING.ipynb
├── src/
│   ├── components/
│   │   ├── data_ingestion.py
│   │   ├── data_transformation.py
│   │   └── model_trainer.py
│   ├── pipeline/
│   │   ├── train_pipeline.py
│   │   └── predict_pipeline.py
│   ├── exception.py
│   ├── logger.py
│   └── utils.py
├── templates/
│   ├── home.html
│   └── index.html
├── app.py
├── requirements.txt
├── setup.py
└── README.md
⚙️ Setup & Run Instructions
🔹 Prerequisites
Python 3.8+

pip

Git

🔹 Local Setup
bash
Copy code
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

Ensemble and boosting models outperformed baseline regressors

Stable and consistent predictions

End-to-end ML pipeline ready for deployment

🧩 Future Enhancements
☁️ AWS Elastic Beanstalk deployment

🐳 Docker containerization

📊 Model monitoring and logging

📈 Performance dashboard

👤 Author
Apurva Jadhav
Final Year Computer Engineering Student
