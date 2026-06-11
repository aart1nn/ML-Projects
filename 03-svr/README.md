<div align="center">

# 💎 Diamond Price Prediction
### Support Vector Regression (SVR) — Diamonds Dataset

![Python](https://img.shields.io/badge/Python-1a0533?style=for-the-badge&logo=python&logoColor=c4b5fd)
![Scikit-Learn](https://img.shields.io/badge/Scikit--Learn-1a0533?style=for-the-badge&logo=scikit-learn&logoColor=c4b5fd)
![Pandas](https://img.shields.io/badge/Pandas-1a0533?style=for-the-badge&logo=pandas&logoColor=c4b5fd)
![Matplotlib](https://img.shields.io/badge/Matplotlib-1a0533?style=for-the-badge&logo=python&logoColor=c4b5fd)

</div>

---

## 📌 Overview
Predicting diamond prices using **Support Vector Regression (SVR)**.
A complete ML pipeline including encoding, scaling on both X and y, training, evaluation and visualization.

---

## 📂 Dataset
| Property | Value |
|----------|-------|
| Source | Kaggle — Diamonds Dataset |
| Rows | 53,940 |
| Features | 10 |
| Target | Price (USD) |

---

## 🎯 Features Selected
| Feature | Type | Description |
|---------|------|-------------|
| carat | Numerical | Weight of the diamond |
| x | Numerical | Length (mm) |
| y | Numerical | Width (mm) |
| z | Numerical | Depth (mm) |
| cut | Categorical | Quality of the cut |
| color | Categorical | Diamond color grade |
| clarity | Categorical | Clarity grade |

---

## ⚙️ Pipeline
Raw Data ──► Encoding ──► Feature Selection ──► Scaling (X & y) ──► Train ──► Evaluate ──► Visualize

---

## 📈 Results
| Metric | Score |
|--------|-------|
| ✅ R2 Score | 0.88 |
| 📉 RMSE | ~35% of mean price |

---

## 💡 Key Insights
- **Carat** and **dimensions (x, y, z)** had the strongest correlation with price
- Scaling **y** alongside **X** significantly improved SVR performance
- Error distribution was roughly symmetric around zero ✅