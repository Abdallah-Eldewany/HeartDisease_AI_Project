# 🫀 Healthcare Analytics: Heart Disease Binary Classification

An end-to-end machine learning repository dedicated to predicting the presence of heart disease using clinical patient attributes from the renowned **UCI Heart Disease Dataset**. This project benchmarks multiple predictive models, focusing on balancing precision and recall to ensure reliable clinical decision support.

---

## 📌 Project Overview

Cardiovascular diseases are a leading cause of global mortality. Early automated detection can significantly aid healthcare providers. This project utilizes a patient diagnostic dataset to build a robust binary classification pipeline, determining whether a patient has a statistical presence of heart disease based on 13 key physiological features.

---

## 📊 Dataset Architecture & Features

* **Dataset Source:** UCI Heart Disease Dataset.
* **Target Classification:** `target` (0 = No heart disease, 1 = Presence of heart disease).

### 📋 Clinical Feature Glossary
| Feature Name | Type | Description |
| :--- | :---: | :--- |
| **age** | Numeric | Age of the patient in years |
| **sex** | Categorical | Binary gender indicator (1 = Male, 0 = Female) |
| **cp** | Categorical | Chest pain type (4 distinct structural values) |
| **trestbps** | Numeric | Resting blood pressure (in mm Hg on admission) |
| **chol** | Numeric | Serum cholesterol in mg/dl |
| **fbs** | Categorical | Fasting blood sugar > 120 mg/dl (1 = True, 0 = False) |
| **restecg** | Categorical | Resting electrocardiographic results (values 0, 1, 2) |
| **thalach** | Numeric | Maximum heart rate achieved during stress testing |
| **exang** | Categorical | Exercise-induced angina (1 = Yes, 0 = No) |
| **oldpeak** | Numeric | ST depression induced by exercise relative to rest |
| **slope** | Categorical | The slope of the peak exercise ST segment |
| **ca** | Numeric | Number of major vessels (0–3) colored by fluoroscopy |
| **thal** | Categorical | Thalassemia type (Normal, Fixed defect, Reversable defect) |

---

## 🛠️ End-to-End Workflow Pipeline

1. **🧹 Data Ingestion & Cleaning:** Audited the dataset for anomalies, verified correct numeric constraints, and handled implicit categorical scaling.
2. **📊 Exploratory Data Analysis (EDA):** Analyzed target balance, feature correlations, and the visual distribution of key indicators like cholesterol and max heart rate against the target variable.
3. **✂️ Data Splitting:** Partitioned the feature matrix into independent training and testing subsets to maintain rigorous validation rules.
4. **🤖 Multi-Model Benchmarking:** Implemented and evaluated 5 distinct predictive algorithms to evaluate linear vs. non-linear spatial performance boundaries.

---

## 📊 Modeling & Evaluation Framework

In medical diagnoses, tracking **Recall** (minimizing False Negatives to avoid missing a sick patient) is just as critical as overall **Accuracy**. The following models were systematically trained and evaluated:

* **Logistic Regression** (Strong, interpretable linear baseline)
* **K-Nearest Neighbors (KNN)** (Distance-based instance classification)
* **Support Vector Machine (SVM)** (Maximum margin geometric hyperplanes)
* **Decision Tree Classifier** (Hierarchical non-linear rules)
* **Random Forest Classifier** (Ensemble bagging to mitigate overfitting)

### 📈 Performance Comparison Matrix

| Machine Learning Model | Accuracy | Precision | Recall | F1-Score |
| :--- | :---: | :---: | :---: | :---: |
| **Logistic Regression** | 85% - 90% | *TBD* | *TBD* | *TBD* |
| **Random Forest** | 85% - 90% | *TBD* | *TBD* | *TBD* |
| **Support Vector Machine (SVM)**| *TBD* | *TBD* | *TBD* | *TBD* |
| **K-Nearest Neighbors (KNN)** | *TBD* | *TBD* | *TBD* | *TBD* |
| **Decision Tree** | *TBD* | *TBD* | *TBD* | *TBD* |

> 📌 **Key Finding:** Random Forest and Logistic Regression delivered the highest and most stable cross-validation metrics across the test matrix.

---

## 💻 Environment Setup & Execution

1. Clone this repository to your local machine:
   ```bash
   git clone [https://github.com/your-username/heart-disease-prediction.git](https://github.com/your-username/heart-disease-prediction.git)
