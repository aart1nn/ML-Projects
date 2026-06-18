<div align="center">

# 🍷 Wine Quality Prediction
### Support Vector Machine (SVM) — Red Wine Quality Dataset

![Python](https://img.shields.io/badge/Python-1a0533?style=for-the-badge&logo=python&logoColor=c4b5fd)
![Scikit-Learn](https://img.shields.io/badge/Scikit--Learn-1a0533?style=for-the-badge&logo=scikit-learn&logoColor=c4b5fd)
![Pandas](https://img.shields.io/badge/Pandas-1a0533?style=for-the-badge&logo=pandas&logoColor=c4b5fd)
![Matplotlib](https://img.shields.io/badge/Matplotlib-1a0533?style=for-the-badge&logo=python&logoColor=c4b5fd)

</div>

---

## 📌 Overview
Predicting red wine quality using **Support Vector Machine (SVM) Classification**.
Includes binary target transformation, kernel comparison, and full classification evaluation.

---

## 📂 Dataset
| Property | Value |
|----------|-------|
| Source | Kaggle — Red Wine Quality Dataset |
| Rows | 1,599 |
| Features | 11 |
| Target | quality (0: Low, 1: High) |

---

## 🔄 Target Transformation
Original quality scores (3-8) were converted to binary:
- **0** → Low Quality (quality ≤ 5)
- **1** → High Quality (quality > 5)

| Class | Count |
|-------|-------|
| High Quality (1) | 855 |
| Low Quality (0) | 744 |

---

## 🎯 Features Used
| Feature | Correlation |
|---------|-------------|
| alcohol | 🥇 Highest |
| volatile acidity | 🥈 Second |
| sulphates | 🥉 Third |
| citric acid | Moderate |
| total sulfur dioxide | Moderate |
| + 6 more features | Low |

---

## ⚙️ Pipeline
Raw Data ──► Target Transformation ──► Feature Selection ──► Scaling ──► Kernel Comparison ──► Train ──► Evaluate ──► Visualize

---

## 🔍 Kernel Comparison
| Kernel | Accuracy |
|--------|----------|
| linear | 0.73 |
| **rbf** ✅ | **0.77** |
| poly | 0.77 |
| sigmoid | 0.68 |

> **rbf** selected — best balance of accuracy and stability

---

## 📈 Results
| Metric | Score |
|--------|-------|
| ✅ Accuracy | 0.77 |
| 🎯 Precision | 0.81 |
| 🔁 Recall | 0.77 |

---

## 💡 Key Insights
- **alcohol** had the strongest correlation with wine quality
- Binary transformation balanced the classes well (855 vs 744)
- **rbf kernel** performed best among all tested kernels
- SVM required feature scaling due to distance-based margin optimization ✅