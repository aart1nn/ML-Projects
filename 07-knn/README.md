<div align="center">

# 🫀 Heart Disease Prediction
### K-Nearest Neighbors (K-NN) — Heart Disease Dataset

![Python](https://img.shields.io/badge/Python-1a0533?style=for-the-badge&logo=python&logoColor=c4b5fd)
![Scikit-Learn](https://img.shields.io/badge/Scikit--Learn-1a0533?style=for-the-badge&logo=scikit-learn&logoColor=c4b5fd)
![Pandas](https://img.shields.io/badge/Pandas-1a0533?style=for-the-badge&logo=pandas&logoColor=c4b5fd)
![Matplotlib](https://img.shields.io/badge/Matplotlib-1a0533?style=for-the-badge&logo=python&logoColor=c4b5fd)

</div>

---

## 📌 Overview
Predicting heart disease using **K-Nearest Neighbors (K-NN) Classification**.
Includes finding the optimal K value through error rate analysis.

---

## 📂 Dataset
| Property | Value |
|----------|-------|
| Source | Kaggle — Heart Disease Dataset |
| Rows | 1,025 |
| Features | 13 |
| Target | target (0: No Disease, 1: Heart Disease) |

---

## 🎯 Features Used
| Feature | Description |
|---------|-------------|
| oldpeak | ST depression induced by exercise |
| exang | Exercise induced angina |
| cp | Chest pain type |
| thalach | Maximum heart rate achieved |
| ca | Number of major vessels |
| slope | Slope of peak exercise ST segment |
| thal | Thalassemia |
| sex | Sex |
| age | Age |
| trestbps | Resting blood pressure |
| restecg | Resting ECG results |
| chol | Cholesterol |
| fbs | Fasting blood sugar |

---

## ⚙️ Pipeline
Raw Data ──► Exploration ──► Feature Selection ──► Scaling ──► Find Best K ──► Train ──► Evaluate ──► Visualize

---

## 🔍 Finding Best K
Tested K values from 1 to 29 — **K=3** gave the best balance between bias and variance.

---

## 📈 Results
| Metric | Score |
|--------|-------|
| ✅ Accuracy | 0.94 |
| 🎯 Precision | 0.92 |
| 🔁 Recall | 0.95 |

---

## 💡 Key Insights
- **K=3** was selected after analyzing error rates across K=1 to K=29
- Feature scaling was essential — K-NN is distance-based and sensitive to scale
- Achieved **94% accuracy** — best result across all projects so far 🏆