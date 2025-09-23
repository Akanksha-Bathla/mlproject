# Student Performance Prediction - MLOps Web Application

A machine learning web application that predicts student performance based on various academic and demographic factors. Built with Flask and following MLOps best practices for reproducibility and deployment.

![Python](https://img.shields.io/badge/Python-3.8%252B-blue)
![Flask](https://img.shields.io/badge/Flask-2.0%252B-green)
![MLOps](https://img.shields.io/badge/MLOps-Enabled-orange)
![Scikit--learn](https://img.shields.io/badge/Scikit--learn-1.0%252B-yellow)

## 📌 Table of Contents
- [📖 Overview](#-overview)
- [✨ Features](#-features)
- [📂 Project Structure](#-project-structure)
- [🧑‍💻 Tech Stack](#%E2%80%8D-tech-stack)
- [⚙️ Installation & Setup](#%EF%B8%8F-installation--setup)
- [🚀 Usage](#-usage)
- [📊 Dataset](#-dataset)
- [🔧 MLOps Integration](#-mlops-integration)
- [📈 Model Performance](#-model-performance)
- [📸 Screenshots](#-screenshots)
- [🤝 Contributing](#-contributing)
- [📜 License](#-license)

## 📖 Overview

This project uses the Kaggle Student Performance Dataset to train a regression model that predicts students’ Math scores based on various factors like reading/writing scores, parental education, test preparation, and more.

The model is deployed as a Flask web app where users can input student details and instantly get a predicted math score.

## ✨ Features

- ✅ Data preprocessing & EDA
- ✅ Multiple ML models compared (Linear Regression, Random Forest, etc.)
- ✅ Final model saved using Pickle.
- ✅ Flask-based web interface for predictions
- ✅ MLOps features:
  - Version control (Git + GitHub)
  - Model versioning & reproducibility
  - Logging & monitoring hooks

## 📂 Project Structure
```
Student-Performance-Predictor/
│-- data/                  # Raw & processed datasets
│-- notebooks/             # Jupyter notebooks for EDA & experiments
│-- src/                   # Source code
│   │-- __init__.py
│   │-- data_preprocessing.py
│   │-- train.py           # Training pipeline
│   │-- evaluate.py
│-- models/                # Saved trained models
│-- templates/             # HTML templates for Flask
│-- static/                # CSS/JS files
│-- app.py                 # Flask app entry point
│-- requirements.txt       # Python dependencies
│-- Dockerfile             # For containerization
│-- .github/workflows/     # CI/CD pipelines
│-- README.md              # Project documentation
```

## 🧑‍💻 Tech Stack
- **Programming**: Python, Flask
- **ML Libraries**: Scikit-learn, Pandas, NumPy, Matplotlib, Seaborn
- **MLOps Tools**: GitHub Actions, Docker, Logging
- **Deployment**: Flask app (local & cloud-ready)

## ⚙️ Installation & Setup

1. Clone the Repository
```git clone https://github.com/bathlahimanshi/MathsScorePredictor.git
cd MathsScorePredictor
```

2. Create Virtual Environment
```python -m venv venv
source venv/bin/activate   # for Linux/Mac
venv\Scripts\activate      # for Windows
```
3. Install Dependencies
```
pip install -r requirements.txt
```
4. Run the Flask App
```python app.py

App will run on http://127.0.0.1:5000/
```

## 🚀 Usage

- Open the Flask web app in your browser.
- Fill in student details (gender, parental education, test prep, reading/writing scores, etc.).
- Click Predict to get the math score prediction.

## 📊 Dataset
- Dataset: Kaggle - Student Performance
- Target Variable: math_score
- Features: Gender, parental education level, lunch, test preparation, reading score, writing score, etc.

## 🔧 MLOps Integration
- Version Control: GitHub for code + dataset tracking
- Logging & Monitoring: Model performance logs and app monitoring hooks

## 📈 Model Performance
- Evaluated models: Linear Regression, Random Forest, Gradient Boosting
- Selected Model: Random Forest (best accuracy & generalization)
- Metrics: R², MAE, RMSE
- Model	R² Score	RMSE
- Linear Regression	0.82	5.3
- Random Forest	0.89	4.1
- Gradient Boosting	0.87	4.4

## 📸 Screenshots

👉 <img width="792" height="911" alt="Screenshot 2025-09-24 002345" src="https://github.com/user-attachments/assets/fad578d2-7bfa-4a96-b253-1ce01a09f971" />


## 🤝 Contributing
Contributions are welcome!

#### Fork the repo
Create a new branch (feature-xyz)

#### Commit changes
Submit a Pull Request

## 📜 License
This project is licensed under the MIT License.
