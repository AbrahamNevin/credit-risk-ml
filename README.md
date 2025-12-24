# 🏦 Scalable Credit Risk Prediction System with MLOps

An end-to-end **production-grade machine learning pipeline** for predicting credit default risk using structured financial data.  
This project demonstrates **data engineering, classical ML, MLOps, fairness auditing, and SQL integration**, aligned with real-world credit risk modeling practices used in banks and fintech companies.

---

## 📌 Problem Statement

Credit institutions must assess the likelihood that a customer will default on their credit payments.  
This is a **binary classification problem** with:
- Highly **imbalanced classes**
- **Regulatory and fairness constraints**
- Strong dependence on **behavioral and financial patterns**

The goal of this project is to build a **scalable, auditable, and explainable ML system** for credit default prediction.

---

## 🧠 Key Highlights

- End-to-end ML pipeline (raw data → model → evaluation)
- Domain-driven **credit risk feature engineering**
- Baseline + Gradient Boosting models
- **MLflow experiment tracking**
- **Fairness & bias analysis** (Gender, Age, Education)
- **SQL-based data integration**
- Clean Git-based workflow

---



yaml
Copy code

---

## 📊 Dataset

**UCI Credit Card Default Dataset**

- 30,000 customers
- Financial, demographic, and behavioral attributes
- Target: `default payment next month`

---

## 🔍 Exploratory Data Analysis (EDA)

- Target class imbalance analysis
- Demographic default trends
- Feature correlations
- Business-driven problem framing

📓 Notebook: `01_eda_credit_default.ipynb`

---

## 📈 Baseline Model

- **Logistic Regression**
- Standardized features
- Class imbalance handled via `class_weight="balanced"`
- Metrics:
  - ROC-AUC
  - Precision / Recall
  - Confusion Matrix

📓 Notebook: `02_baseline_model.ipynb`

---

## 🛠 Feature Engineering (Credit-Risk Driven)

Key engineered features include:
- Credit utilization ratios
- Payment-to-bill ratios
- Delinquency frequency & severity
- Payment consistency & volatility
- Bill amount trends

📓 Notebook: `03_feature_engineering.ipynb`

---

## 🌲 Tree-Based Models

- **XGBoost**
- **LightGBM**

Both models significantly outperform the baseline in ROC-AUC.

📓 Notebook: `04_tree_models.ipynb`

---

## 🧪 MLOps with MLflow

- Experiment tracking
- Parameter logging
- Metric comparison
- Model artifact versioning

📓 Notebook: `05_mlflow_tracking.ipynb`

Run MLflow UI:
```bash
mlflow ui
⚖️ Fairness & Bias Analysis
Model performance evaluated across:

Gender

Age groups

Education level

Metrics:

TPR / FPR

Default rate

ROC-AUC by subgroup

📓 Notebook: 06_fairness_analysis.ipynb

🗄 SQL Integration
Feature-engineered data stored in SQLite

Model training performed using SQL queries

Simulates real-world ML pipelines

📓 Notebook: 07_sql_integration.ipynb

🧰 Tech Stack
Python

Pandas, NumPy

Scikit-learn

XGBoost, LightGBM

MLflow

SQLite

Git & GitHub

Jupyter Notebook

🚀 How to Run
bash
Copy code
git clone https://github.com/AbrahamNevin/credit-risk-ml.git
cd credit-risk-ml
python -m venv venv
venv\Scripts\activate
pip install -r requirements.txt
Run notebooks in order: 01 → 07.

👤 Author
Nevin Abraham
Computer Science & Engineering
Machine Learning | Fintech | Data Science

📌 Disclaimer
This project is for educational and demonstration purposes only and should not be used for real credit decisions without regulatory approval.

yaml
Copy code

---

## ✅ STEP 4 — Commit the README

```powershell
git add README.md
git commit -m "docs: add comprehensive project README"
git push origin main
