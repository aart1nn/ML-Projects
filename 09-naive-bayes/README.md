<div align="center">

# 📧 Spam Detection
### Naive Bayes — SMS Spam Collection Dataset

![Python](https://img.shields.io/badge/Python-1a0533?style=for-the-badge&logo=python&logoColor=c4b5fd)
![Scikit-Learn](https://img.shields.io/badge/Scikit--Learn-1a0533?style=for-the-badge&logo=scikit-learn&logoColor=c4b5fd)
![Pandas](https://img.shields.io/badge/Pandas-1a0533?style=for-the-badge&logo=pandas&logoColor=c4b5fd)
![Matplotlib](https://img.shields.io/badge/Matplotlib-1a0533?style=for-the-badge&logo=python&logoColor=c4b5fd)

</div>

---

## 📌 Overview
Detecting spam messages using **Naive Bayes Classification** combined with **Bag of Words (NLP)**.
A unique project that bridges classical ML with text processing techniques.

---

## 📂 Dataset
| Property | Value |
|----------|-------|
| Source | Kaggle — SMS Spam Collection |
| Rows | 5,572 |
| Features | Text messages |
| Target | label (0: Ham, 1: Spam) |

---

## 🔄 Target Transformation
| Label | Value | Count |
|-------|-------|-------|
| Ham (normal) | 0 | 4,825 |
| Spam | 1 | 747 |

---

## ⚙️ Pipeline
Raw Text ──► Label Encoding ──► Bag of Words ──► Train Test Split ──► Train ──► Evaluate ──► Visualize

---

## 🧠 Bag of Words
Used **CountVectorizer** to convert raw text into numerical features:
- **5,572** messages → matrix of shape **(5572, 8672)**
- Each message becomes a vector of word counts across **8,672 unique words**

---

## 📈 Results
| Metric | Score |
|--------|-------|
| ✅ Accuracy | 0.98 |
| 🎯 Precision | 0.91 |
| 🔁 Recall | 0.93 |

---

## 💡 Key Insights
- **Naive Bayes** is highly effective for text classification tasks
- Words like **"free"**, **"call"**, **"win"**, **"txt"** were top spam indicators
- **Bag of Words** successfully converted raw text into ML-ready features
- No feature scaling needed — Naive Bayes works with probabilities ✅