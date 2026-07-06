<div align="center">

# 💳 Credit Card Customer Segmentation
### KMeans Clustering — Credit Card Dataset

![Python](https://img.shields.io/badge/Python-1a0533?style=for-the-badge&logo=python&logoColor=c4b5fd)
![Scikit-Learn](https://img.shields.io/badge/Scikit--Learn-1a0533?style=for-the-badge&logo=scikit-learn&logoColor=c4b5fd)
![Pandas](https://img.shields.io/badge/Pandas-1a0533?style=for-the-badge&logo=pandas&logoColor=c4b5fd)
![Matplotlib](https://img.shields.io/badge/Matplotlib-1a0533?style=for-the-badge&logo=python&logoColor=c4b5fd)
![Seaborn](https://img.shields.io/badge/Seaborn-1a0533?style=for-the-badge&logo=python&logoColor=c4b5fd)

</div>

---

## 📌 Overview
Segmenting credit card customers based on their financial behavior using **KMeans Clustering**.  
Helps banks identify distinct customer groups for targeted marketing and risk management.  
First **unsupervised learning** project — no labels, no target column, just patterns in data.

---

## 📂 Dataset
| Property | Value |
|----------|-------|
| Source | Kaggle — Credit Card Dataset for Clustering |
| Rows | 8,950 |
| Features | 18 |
| Target | None (Unsupervised) |

---

## 🧹 Data Cleaning
- **MINIMUM_PAYMENTS** — 313 missing values filled with median
- **CREDIT_LIMIT** — 1 missing value filled with median
- **CUST_ID** dropped — identifier column, not a meaningful feature
- Median preferred over mean — financial data is sensitive to outliers

---

## ⚙️ Pipeline
Raw Data ──► Cleaning ──► Scaling ──► Optimal K ──► KMeans ──► Analyze ──► Visualize

---

## 🔍 Finding Optimal K
Used two methods together for a reliable decision:

| Method | Result |
|--------|--------|
| Elbow Method | Inconclusive — between K=4 and K=5 |
| Silhouette Score | K=3 → 0.2510 ✅ |

> Silhouette Score confirmed **K=3** as the optimal number of clusters

---

## 📊 Cluster Profiles

| Cluster | Profile | Customers | Key Behavior |
|---------|---------|-----------|--------------|
| 0 | 🟢 Active & Reliable | 1,275 | High purchases, high payments, high credit limit |
| 1 | 🟡 Cautious | 6,114 | Low activity, low balance, typical user |
| 2 | 🔴 High Risk | 1,561 | Heavy cash advances, minimal purchases, low repayment |

---

## 📈 Results

| Metric | Value |
|--------|-------|
| 🔢 Optimal K | 3 |
| 📐 Best Silhouette Score | 0.2510 |
| 👥 Total Customers | 8,950 |

---

## 💡 Key Insights
- **Cluster 1** contains 68% of customers — typical low-activity users
- **Cluster 0** are the most valuable customers — high purchases, high payments, high credit limit
- **Cluster 2** rely heavily on cash advances with minimal purchases — high financial risk indicator
- **Silhouette Score of 0.25** is expected for high-dimensional financial data — not a weakness of the model
- **Elbow Method** alone was inconclusive — always combine with Silhouette Score for reliable results
- **PCA** confirmed clear visual separation between the three customer segments