<div align="center">

# 🚗 Car Fuel Consumption Prediction
### Polynomial Regression Model — Auto MPG Dataset

![Python](https://img.shields.io/badge/Python-1a0533?style=for-the-badge&logo=python&logoColor=c4b5fd)
![Scikit-Learn](https://img.shields.io/badge/Scikit--Learn-1a0533?style=for-the-badge&logo=scikit-learn&logoColor=c4b5fd)
![Pandas](https://img.shields.io/badge/Pandas-1a0533?style=for-the-badge&logo=pandas&logoColor=c4b5fd)
![Matplotlib](https://img.shields.io/badge/Matplotlib-1a0533?style=for-the-badge&logo=python&logoColor=c4b5fd)

</div>

---

## 📌 Overview
Predicting car fuel consumption (**MPG**) using both **Linear** and **Polynomial Regression**.
A side-by-side comparison to show why Polynomial fits non-linear data better.

---

## 📂 Dataset
| Property | Value |
|----------|-------|
| Source | UCI — Auto MPG |
| Rows | 398 |
| Features | 8 |
| Target | MPG (Miles Per Gallon) |

---

## 🎯 Features Selected
| Feature | Description |
|---------|-------------|
| weight | Weight of the car |
| displacement | Engine displacement |
| cylinders | Number of cylinders |
| model year | Year of manufacture |
| origin | Country of origin |

---

## ⚙️ Pipeline
Raw Data ──► Exploration ──► Feature Selection ──► Scaling ──► Train ──► Evaluate ──► Visualize

---

## 📈 Results
| Metric | Linear Regression | Polynomial Regression |
|--------|-------------------|----------------------|
| ✅ R2 Score | 0.84 | 0.86 |
| 📉 RMSE | 2.90 | 2.60 |

---

## 💡 Key Insight
**Polynomial Regression (degree=2)** outperformed Linear Regression,
confirming that the relationship between car features and fuel consumption is **non-linear**.