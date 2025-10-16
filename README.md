# 🧠 AI Job Market Insights — Predicting Job Growth in AI/ML Sector

![Python](https://img.shields.io/badge/Python-3.12-blue?logo=python)
![Machine Learning](https://img.shields.io/badge/Machine%20Learning-Project-orange?logo=scikitlearn)
![Status](https://img.shields.io/badge/Status-Completed-success)

---

## 📘 Project Overview
The **AI Job Market Insights** project analyzes current AI job trends and predicts **job growth projections** for various AI-related roles.  
The goal is to help professionals, recruiters, and companies understand **which AI skill sets and positions** are most likely to grow in the near future.

This end-to-end project demonstrates skills in:
- Data preprocessing and encoding  
- Exploratory Data Analysis (EDA)  
- Model training and hyperparameter tuning  
- Model evaluation and feature importance visualization  

---

## 📂 Dataset Description

**Dataset Name:** `ai_job_market_insights.csv`

| Column Name | Description |
|--------------|-------------|
| `Salary` | Average salary for AI roles (numeric) |
| `Experience_Required` | Required years of experience |
| `Skill_Level` | Skill proficiency (Beginner / Intermediate / Expert) |
| `Company_Size` | Size of company (Small / Medium / Large) |
| `Job_Type` | Job category (e.g., Data Scientist, ML Engineer, AI Analyst) |
| `Location` | Job location (City/Region) |
| `Job_Growth_Projection` | Target variable — job growth trend (0 = Low, 1 = Medium, 2 = High) |

> 🔹 Only `Salary` is numeric; all others are categorical.  
> 🔹 The target variable (`Job_Growth_Projection`) is multiclass.

---

## 🧩 Project Workflow

### **1️⃣ Data Preprocessing**
- Checked and handled missing values  
- Encoded categorical features using **OneHotEncoder**  
- Scaled numeric features where needed  
- Split the dataset into training and testing sets  

### **2️⃣ Exploratory Data Analysis**
- Visualized distributions and job trends  
- Analyzed correlation between `Salary` and target variable  
- Checked target class balance  

### **3️⃣ Model Development**
Models applied:
- **Logistic Regression**
- **Random Forest Classifier**
- **XGBoost Classifier**

Techniques used:
- `Pipeline()` for preprocessing and modeling  
- `GridSearchCV()` for hyperparameter tuning  
- `StratifiedKFold()` for balanced cross-validation  

### **4️⃣ Model Evaluation**
Metrics used:
- Accuracy  
- Precision, Recall, F1-score  
- Confusion Matrix  

| Model | Accuracy |
|--------|-----------|
| Logistic Regression | 0.36 |
| Random Forest | 0.35 |
| XGBoost | 0.41 ✅ |

### **5️⃣ Feature Importance**
- Extracted feature importance from XGBoost  
- Visualized top 20 influential features using Seaborn bar plots  

---

## 🛠️ Tools & Technologies

| Category | Tools Used |
|-----------|-------------|
| Programming | Python 3.12 |
| Libraries | pandas, numpy, scikit-learn, seaborn, matplotlib, xgboost |
| Environment | Jupyter Notebook |
| Version Control | Git, GitHub |

---

## 💻 How to Run the Project

1. **Clone the Repository**
```bash
git clone https://github.com/YourUsername/AI_Job_Market_Insights.git
cd AI_Job_Market_Insights 
pip install -r requirements.txt
jupyter notebook AI_Job_Market_Insights.ipynb

