<div align="center">

# 💉 Diabetes Prediction
### Logistic Regression — Pima Indians Diabetes Dataset

![Python](https://img.shields.io/badge/Python-1a0533?style=for-the-badge&logo=python&logoColor=c4b5fd)
![Scikit-Learn](https://img.shields.io/badge/Scikit--Learn-1a0533?style=for-the-badge&logo=scikit-learn&logoColor=c4b5fd)
![Pandas](https://img.shields.io/badge/Pandas-1a0533?style=for-the-badge&logo=pandas&logoColor=c4b5fd)
![Matplotlib](https://img.shields.io/badge/Matplotlib-1a0533?style=for-the-badge&logo=python&logoColor=c4b5fd)

</div>

---

## 📌 Overview
Predicting diabetes using **Logistic Regression** — the first **Classification** project in this repo.
Includes handling of hidden missing values and full classification evaluation metrics.

---

## 📂 Dataset
| Property | Value |
|----------|-------|
| Source | UCI / Kaggle — Pima Indians Diabetes Database |
| Rows | 768 |
| Features | 8 |
| Target | Outcome (0: No Diabetes, 1: Diabetes) |

---

## 🎯 Features Used
| Feature | Correlation with Outcome |
|---------|---------------------------|
| Glucose | 🥇 Highest |
| BMI | 🥈 Second |
| Age | 🥉 Third |
| Pregnancies | Moderate |
| SkinThickness | Moderate |
| DiabetesPedigreeFunction | Moderate |
| BloodPressure | Low |
| Insulin | Low |

---

## ⚙️ Pipeline
Raw Data ──► Hidden Missing Values ──► Feature Selection ──► Scaling ──► Train ──► Evaluate ──► Visualize

---

## 🧹 Data Cleaning Highlight
Several columns contained **biologically impossible zeros** (e.g. Glucose=0, BMI=0),
which were treated as missing values and replaced with the **median**.

| Column | Zero Count |
|--------|------------|
| Insulin | 374 |
| SkinThickness | 227 |
| BloodPressure | 35 |
| BMI | 11 |
| Glucose | 5 |

---

## 📈 Results
| Metric | Score |
|--------|-------|
| ✅ Accuracy | 0.77 |
| 🎯 Precision | 0.68 |
| 🔁 Recall | 0.65 |

---

## 💡 Key Insights
- **Glucose** was the strongest predictor of diabetes
- Hidden missing values (encoded as 0) significantly affect model performance if not handled
- This was the first **Classification** project — introducing Accuracy, Precision, Recall, and Confusion Matrix