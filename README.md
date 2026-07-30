# 🧠 Remote Work & Mental Health Prediction

A Machine Learning pipeline designed to predict the mental health status of remote employees, helping organizations provide early interventions, reduce burnout, and foster a healthier work-life balance.

---

## 📌 Project Overview
While remote work offers flexibility and autonomy, it also introduces challenges such as social isolation, blurred work-life boundaries, and heightened workplace stress. Left unaddressed, these factors can lead to burnout, decreased productivity, and employee turnover.

This project leverages Machine Learning techniques on employee survey data to classify and predict mental wellness levels, enabling organizations to offer timely support and proactive interventions.

---

## 📊 Dataset Details
- **Total Records (Rows):** 2,358
- **Total Features (Columns):** 15
- **Target Variable:** `Mental Health Status`


---

## ⚙️ Data Preprocessing & Pipeline Workflow
To ensure high model reliability and efficiency, the raw dataset goes through a structured 6-stage preprocessing pipeline:

1. **Handling Missing Data:** Cleaned missing and incomplete entries to preserve dataset integrity.
2. **Outliers Removal:** Identified and handled extreme statistical outliers to prevent model bias.
3. **Feature Creation:** Engineered custom, high-impact features from raw data attributes.
4. **Encoding Categorical Variables:** Converted nominal/ordinal categorical fields into numerical representations.
5. **Z-Score Scaling:** Normalized feature ranges using Standard Deviation (Z-score) for consistent model input.
6. **Feature Selection:** Filtered and isolated the top predictors to optimize model training and accuracy.

---

## 👥 Group Members & Individual Roles

| Student ID | Member Name | Technical Responsibility |
| :--- | :--- | :--- |
| **IT24104181** | Alhakoon A.M.D.S. | Handling Missing Data |
| **IT24102876** | Nawarathna I.G.D.S. | Outliers Removal |
| **IT24102770** | Leelarathna G.N.P. | Feature Creation |
| **IT24102944** | Dasanayake U.R.N.P.K. | Encoding Categorical Variables |
| **IT24103652** | Ilham M.H.M. | Z-score Scaling |
| **IT24103159** | Athauda K.K.A.M.S.R.V.B. | Feature Selection |

---

## 🛠️ Tech Stack & Tools
- **Language:** Python
- **Libraries:** Pandas, NumPy, Scikit-Learn, Matplotlib, Seaborn
- **Environment:** Jupyter Notebook / Google Colab / VS Code

---

## 🚀 Getting Started

### 1. Clone the Repository
```bash
git clone [https://github.com/your-username/remote-work-mental-health.git](https://github.com/your-username/remote-work-mental-health.git)
cd remote-work-mental-health
