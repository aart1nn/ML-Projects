<div align="center">

# 🪙 Customer Churn Prediction
### Random Forest Classification — Telco Customer Churn Dataset

![Python](https://img.shields.io/badge/Python-1a0533?style=for-the-badge&logo=python&logoColor=c4b5fd)
![Scikit-Learn](https://img.shields.io/badge/Scikit--Learn-1a0533?style=for-the-badge&logo=scikit-learn&logoColor=c4b5fd)
![Pandas](https://img.shields.io/badge/Pandas-1a0533?style=for-the-badge&logo=pandas&logoColor=c4b5fd)
![Matplotlib](https://img.shields.io/badge/Matplotlib-1a0533?style=for-the-badge&logo=python&logoColor=c4b5fd)

</div>

---

## 📌 Overview
Predicting customer churn using **Random Forest Classification**.
Includes handling class imbalance with `class_weight='balanced'` to maximize Recall — critical for business decisions.

---

## 📂 Dataset
| Property | Value |
|----------|-------|
| Source | Kaggle — Telco Customer Churn |
| Rows | 7,043 |
| Features | 19 |
| Target | Churn (0: No Churn, 1: Churn) |

---

## 🔄 Data Cleaning Highlights
- **TotalCharges** converted from string to numeric
- **11 missing values** in TotalCharges filled with median
- **customerID** dropped — not a meaningful feature

---

## 🔤 Encoding
Used **LabelEncoder** for categorical features — suitable for tree-based models like Random Forest which don't assume ordinal relationships between values.

---

## ⚙️ Pipeline
Raw Data ──► Cleaning ──► Encoding ──► Feature Selection ──► Train ──► Evaluate ──► Visualize

---

## ⚖️ Class Imbalance
Dataset was imbalanced — more "No Churn" than "Churn" samples.
Used `class_weight='balanced'` to give higher weight to minority class (Churn).

| Without balanced | With balanced |
|-----------------|---------------|
| Recall: 0.45 | Recall: 0.86 ✅ |
| Accuracy: 0.80 | Accuracy: 0.76 |

---

## 📈 Results
| Metric | Score |
|--------|-------|
| ✅ Accuracy | 0.76 |
| 🎯 Precision | 0.52 |
| 🔁 Recall | 0.86 |

> **Recall** was prioritized — missing a churning customer costs more than a false alarm 💜

---

## 💡 Key Insights
- **Contract type** was the most important feature for predicting churn
- **Tenure** and **OnlineSecurity** also played major roles
- `class_weight='balanced'` significantly improved Recall from 45% to 86%
- LabelEncoder was preferred over One-Hot Encoding for tree-based models ✅