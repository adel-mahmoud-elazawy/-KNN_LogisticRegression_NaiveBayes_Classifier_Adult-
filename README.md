# Adult Income Prediction (My 2nd ML Project) 📊

A Machine Learning classification project predicting whether an individual's annual income exceeds **$50,000/year** based on UCI Census demographic data.

---

## 📌 Overview

This is my second hands-on Machine Learning project. After building a Linear Regression model in my first project, I moved on to explore **Binary Classification** algorithms: **K-Nearest Neighbors (KNN)**, **Logistic Regression**, and **Gaussian Naive Bayes**.

---

## 📅 Dataset

* **Records:** 48,842 rows
* **Target:** `income` (`<=50K` vs `>50K`)

---

## ⚙️ Key Steps Implemented

1. **Data Cleaning:** Handled missing values (`?`) and removed duplicates.
2. **Feature Engineering:** Created `net_capital` (`capital_gain - capital_loss`) and simplified complex categorical columns.
3. **Train/Test Split:** Applied a stratified split (80% train / 20% test).
4. **Preprocessing:** Scaled numerical features using `RobustScaler` and encoded categorical attributes, strictly fitted on the training set to prevent data leakage.
5. **Model Tuning:** Used `GridSearchCV` with 5-fold cross-validation to select the optimal $K$ value for KNN.
6. **Model Evaluation:** Evaluated models using Accuracy, Precision, Recall, F1-Score, and ROC-AUC curves.

---

## 📊 Results Summary

| Model | Tuning / Method | Accuracy | ROC-AUC |
| :--- | :--- | :--- | :--- |
| **K-Nearest Neighbors** | $K=31$ (GridSearchCV) | **86.27%** | **0.915** |
| **Logistic Regression** | Default | 84.00% | 0.896 |
| **Gaussian Naive Bayes** | Default | 81.68% | 0.864 |

---

## 💡 Key Learnings

* How to choose the right evaluation metrics for imbalanced datasets (focusing on ROC-AUC & F1-Score instead of accuracy alone).
* The importance of keeping preprocessing (scaling/encoding) fitted only on the training data.
* How to tune hyperparameters using Cross-Validation instead of evaluating directly on test data.

---

## 👤 Author
* **Developer:** [Adel Mahmoud]
* **LinkedIn:** [https://www.linkedin.com/in/adel-mahmoud-elazawy-b35256378?utm_source=share_via&utm_content=profile&utm_medium=member_android]
* **GitHub:** [https://github.com/adel-mahmoud-elazawy]

