<div align="center">

# 🛒 Market Basket Optimization
### Association Rule Learning — Apriori Algorithm

![Python](https://img.shields.io/badge/Python-1a0533?style=for-the-badge&logo=python&logoColor=c4b5fd)
![Mlxtend](https://img.shields.io/badge/Mlxtend-1a0533?style=for-the-badge&logo=python&logoColor=c4b5fd)
![Pandas](https://img.shields.io/badge/Pandas-1a0533?style=for-the-badge&logo=pandas&logoColor=c4b5fd)
![Data Mining](https://img.shields.io/badge/Data_Mining-✓-7c3aed?style=for-the-badge)

</div>

---

## 📌 Overview
Uncovering hidden patterns in consumer behavior using **Association Rule Learning (Apriori)**.  
This project acts as a **Business Problem Solver** by identifying which products are frequently bought together, enabling retail managers to optimize store layouts, design cross-selling strategies, and build targeted recommendation systems.

---

## 📂 Dataset
| Property | Value |
|----------|-------|
| Source | Kaggle — Market Basket Optimization |
| Transactions | 7,501 |
| Max Items/Transaction | 20 |
| Learning Type | Association Rules (Unsupervised) |

---

## ⚙️ Pipeline
Raw Data ──► List Extraction ──► Transaction Encoding ──► Apriori (Support) ──► Rule Generation (Lift) ──► Network & Heatmap Visualization

---

## 🔍 Core Metrics Explained
- **Support:** How frequently the itemset appears in the dataset (min_support = 0.003).
- **Confidence:** How often the rule has been found to be true.
- **Lift:** The strength of the rule. A `Lift > 1` means items are highly dependent on each other.

---

## 📊 Business Insights & Visualizations

| Visual Tool | Purpose | Key Insight |
|-------------|---------|-------------|
| **Bar Chart** | Baseline Sales | Identified Top 20 best-selling individual items. |
| **Scatter Plot** | Rule Strength | Highlighted rules with High Support and High Lift (colored by strength). |
| **Network Graph** | Path Mapping | Mapped clear directional paths from Antecedents to Consequents. |
| **Lift Heatmap** | Cross-Selling Matrix | Provided a 2D grid identifying the strongest pairwise associations instantly. |

### 🔥 Top Actionable Rule
- **Rule:** `Herbs` ──► `Ground Beef`
- **Lift:** `3.66` (Customers buying herbs are 3.6x more likely to buy ground beef).
- **Action:** Bundle these items with a slight discount to maximize revenue.

---
<div align="center">
<h3>📊 "Data isn't just numbers; it's a map of human behavior."</h3>
</div>