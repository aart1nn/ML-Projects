<div align="center">

# 🚲 Bike Rental Prediction
### Decision Tree Regression — Bike Sharing Dataset

![Python](https://img.shields.io/badge/Python-1a0533?style=for-the-badge&logo=python&logoColor=c4b5fd)
![Scikit-Learn](https://img.shields.io/badge/Scikit--Learn-1a0533?style=for-the-badge&logo=scikit-learn&logoColor=c4b5fd)
![Pandas](https://img.shields.io/badge/Pandas-1a0533?style=for-the-badge&logo=pandas&logoColor=c4b5fd)
![Matplotlib](https://img.shields.io/badge/Matplotlib-1a0533?style=for-the-badge&logo=python&logoColor=c4b5fd)

</div>

---

## 📌 Overview
Predicting daily bike rental counts using **Decision Tree Regression**.
This project includes a hands-on exploration of **data leakage** and **hyperparameter tuning** (max_depth).

---

## 📂 Dataset
| Property | Value |
|----------|-------|
| Source | UCI / Kaggle — Bike Sharing Dataset |
| Rows | 731 |
| Features | 16 |
| Target | cnt (Total Daily Rentals) |

---

## 🎯 Features Selected
| Feature | Description |
|---------|-------------|
| atemp | Feels-like temperature |
| temp | Actual temperature |
| yr | Year (0: 2011, 1: 2012) |
| season | Season of the year |
| mnth | Month |

> ⚠️ **registered**, **casual**, and **instant** were excluded to prevent **data leakage**

---

## ⚙️ Pipeline
Raw Data ──► Exploration ──► Leakage Check ──► Feature Selection ──► Train ──► Tune Depth ──► Evaluate ──► Visualize

---

## 🔧 Hyperparameter Tuning (max_depth)
| max_depth | R2 Score | RMSE |
|-----------|----------|------|
| 5 | 0.740 | 1018 |
| 8 | 0.680 | 1119 |
| **4** ✅ | **0.749** | **1002** |

---

## 📈 Final Results
| Metric | Score |
|--------|-------|
| ✅ R2 Score | 0.749 |
| 📉 RMSE | 1002 |

---

## 💡 Key Insights
- **Temperature** was the most important feature for predicting bike rentals 🌡️
- **registered** and **casual** were removed since `cnt = registered + casual` (data leakage)
- **max_depth=4** gave the best balance — higher depths caused overfitting
- Decision Trees require **no feature scaling** ✅