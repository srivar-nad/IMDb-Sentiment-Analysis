# 🎬 IMDb Movie Review Sentiment Analysis

**Authors:** Srikar Varma Nadimpalli & Ruthwick Reddy Podduturi  
**Tools Used:** RapidMiner, k-NN, SVM, Cross-Validation Techniques  
**Domain:** Text Mining · Sentiment Analysis · Marketing Analytics  

---

## 📌 Project Overview

This project focuses on classifying IMDb movie reviews as **positive or negative** using **text mining techniques**. We aimed to derive actionable insights from user feedback to help **marketers**, **filmmakers**, and **production companies** understand audience sentiment and optimize decision-making.

---

## 🎯 Objectives

- Extract sentiment from unstructured review text.
- Build a classification model to label reviews as positive or negative.
- Evaluate model performance using various cross-validation strategies.
- Demonstrate how text analytics can drive marketing and production decisions.

---

## 🧾 Dataset

- **Source:** Kaggle – IMDb Reviews Dataset
- **Attributes:**
  - `review_text`: User-written content
  - `movie_title`: Title of the film
  - `user_rating`: Numerical score (1–10)
  - `review_date`: Timestamp of submission
- **Target Variable:** `sentiment` (positive / negative)

---

## ⚙️ Methodology

### 🔹 Text Preprocessing
- **Tokenization**
- **Stop Word Removal**
- **Case Normalization**
- **Stemming**

### 🔹 Feature Engineering
- Selection of key attributes using RapidMiner's "Select Attributes" operator
- Role assignment for input and output variables

### 🔹 Modeling Techniques
- **k-Nearest Neighbors (k-NN)** with varying distance metrics:
  - Euclidean
  - Manhattan
- **Support Vector Machine (SVM)** for linear classification

### 🔹 Model Evaluation
- 3-fold, 20-fold, and 200-fold **cross-validation**
- Accuracy measurement and performance trade-off analysis

---

## 📊 Key Findings

| Model | Distance | Folds | Performance |
|-------|----------|-------|-------------|
| k-NN  | Euclidean | 3     | Good baseline |
| k-NN  | Manhattan | 20    | Better generalization |
| k-NN  | Euclidean | 200   | **Best accuracy** |
| SVM   | —        | —     | Competitive performance |

- **Lower k**: High sensitivity, risk of overfitting
- **Higher k**: Greater stability, better generalization
- **More folds**: Improved reliability, higher compute cost

---

## 💡 Business Value

- Marketers can leverage **positive reviews** to enhance campaigns.
- **Negative feedback** pinpoints areas for product or storytelling improvement.
- Enables **data-driven decision-making** for customer engagement strategies.

---
