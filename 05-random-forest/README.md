<div align="center">

# 🏥 Medical Insurance Cost Prediction
### Random Forest Regression — Insurance Dataset

![Python](https://img.shields.io/badge/Python-1a0533?style=for-the-badge&logo=python&logoColor=c4b5fd)
![Scikit-Learn](https://img.shields.io/badge/Scikit--Learn-1a0533?style=for-the-badge&logo=scikit-learn&logoColor=c4b5fd)
![Pandas](https://img.shields.io/badge/Pandas-1a0533?style=for-the-badge&logo=pandas&logoColor=c4b5fd)
![Matplotlib](https://img.shields.io/badge/Matplotlib-1a0533?style=for-the-badge&logo=python&logoColor=c4b5fd)

</div>

---

## 📌 Overview
Predicting medical insurance costs using **Random Forest Regression** — an ensemble of decision trees.
This project explores **ensemble learning** and compares feature importance against simple correlation.

---

## 📂 Dataset
| Property | Value |
|----------|-------|
| Source | Kaggle — Medical Cost Personal Dataset |
| Rows | 1,338 |
| Features | 6 |
| Target | charges (USD) |

---

## 🎯 Features Used
| Feature | Type | Correlation with Charges |
|---------|------|---------------------------|
| smoker | Categorical | 🥇 Highest |
| age | Numerical | 🥈 Second |
| bmi | Numerical | 🥉 Third |
| children | Numerical | Low |
| sex | Categorical | Low |
| region | Categorical | Low |

> All features were kept — Random Forest automatically handles low-importance features

---

## ⚙️ Pipeline
Raw Data ──► Encoding ──► Feature Selection ──► Train (100 Trees) ──► Evaluate ──► Visualize

---

## 📈 Results
| Metric | Score |
|--------|-------|
| ✅ R2 Score | 0.87 |
| 📉 RMSE | $4,451 |

---

## 💡 Key Insights
- **smoker** and **bmi** were the most important features for predicting cost
- **sex** and **region** had minimal impact — confirmed by both correlation and Feature Importance
- Random Forest required **no feature scaling** ✅
- Ensemble of 100 trees provided a stable, high-accuracy result