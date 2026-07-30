# 🧠 FlexHealth AI: Remote Work & Mental Health Prediction

An end-to-end Machine Learning prediction pipeline designed to classify the mental health status of remote employees, helping organizations provide early interventions, reduce burnout, and foster a healthier work-life balance.

> **Institution:** SLIIT | **Module:** IT2011 - Artificial Intelligence and Machine Learning  
> **Group ID:** 2025-Y2-S1-KU-40

---

## 📌 Project Overview
While remote work offers flexibility and autonomy, it also introduces challenges such as social isolation, blurred work-life boundaries, and heightened workplace stress. Left unaddressed, these factors can lead to burnout, decreased productivity, and employee turnover.

**FlexHealth AI** leverages Machine Learning techniques on post-pandemic employee survey data to classify and predict mental wellness levels across 6 diagnoses, enabling organizations to offer timely support and proactive interventions.

---

## 📊 Dataset Details
- **Total Records (Rows):** 3,175
- **Total Features (Columns):** 14
- **Target Variable:** `Mental_Health_Status` *(6 Multi-class Labels: Stress Disorder, ADHD, Anxiety, Burnout, Depression, PTSD)*

---

## ⚙️ Data Preprocessing & Pipeline Workflow
To ensure high model reliability and efficiency, the raw dataset goes through a structured pipeline:

1. **Target Cleaning:** Filtered out `'None'` records to frame a diagnostic multi-class classification challenge.
2. **Handling Missing Data:** Applied ML-based imputation using `RandomForestClassifier` for missing values in physical health attributes.
3. **Outliers Removal:** Identified and handled extreme statistical outliers to prevent model bias.
4. **Feature Creation:** Engineered custom features including continuous salary midpoints (`Average_Salary`) and physical health metrics (`Physical_Issue_Count`).
5. **Encoding Categorical Variables:** Applied `OneHotEncoder` for nominal fields and `LabelEncoder` for ordinal burnout attributes.
6. **Z-Score Scaling:** Normalized feature ranges using `StandardScaler` (Z-score Normalization).
7. **Feature Selection:** Filtered and isolated the top 15 predictors using Random Forest Feature Importance.

---

## 🤖 Model Evaluation & Benchmarking
We trained and evaluated 6 classification algorithms to find the optimal model for multi-class prediction:

| Model | Precision | Recall | F1-Score | Accuracy | Status |
| :--- | :---: | :---: | :---: | :---: | :--- |
| **XGBoost Classifier** | **0.59** | **0.60** | **0.59** | **0.60** | 🏆 **Top Performer** |
| **K-Nearest Neighbors (KNN)** | 0.52 | 0.58 | 0.54 | 0.58 | 🥈 Runner-Up |
| **Decision Tree** | 0.21 | 0.21 | 0.21 | 0.21 | Baseline |
| **Random Forest Classifier** | 0.16 | 0.21 | 0.15 | 0.21 | Baseline |
| **Support Vector Machine (SVM)**| 0.18 | 0.19 | 0.18 | 0.19 | Baseline |
| **Logistic Regression** | 0.18 | 0.18 | 0.18 | 0.18 | Baseline |

---

## 🛠️ Tech Stack & Tools
- **Language:** Python
- **ML Frameworks & Libraries:** XGBoost, Scikit-Learn, Pandas, NumPy, Matplotlib, Seaborn
- **Environment:** Jupyter Notebook / VS Code

---

## 👥 Group Members & Individual Roles

| Student ID | Member Name | Technical Responsibility |
| :--- | :--- | :--- |
| **IT24104181** | Alahakoon A.M.D.S. | Handling Missing Data (RF Imputation) |
| **IT24102876** | Nawarathna I.G.D.S. | Outliers Removal |
| **IT24102770** | Leelarathna G.N.P. | Feature Creation & Engineering |
| **IT24102944** | Dasanayake U.R.N.P.K. | Categorical Encoding |
| **IT24103652** | Ilham M.H.M. | Z-score Feature Scaling |
| **IT24103159** | Athauda K.K.A.M.S.R.V.B. | Feature Selection |
