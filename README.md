
# Sampling Assignment – Credit Card Fraud Detection

## Objective
The objective of this assignment is to understand the importance of **sampling techniques** in handling **imbalanced datasets** and to analyze how different sampling strategies affect the performance of various machine learning models.

---

## Dataset Description
- Dataset: `Creditcard_data.csv`
- Target Variable: `Class`
  - `0` → Non-Fraud Transaction
  - `1` → Fraud Transaction
- Nature of Dataset: **Highly Imbalanced**

Imbalanced datasets can bias machine learning models toward the majority class, leading to misleading accuracy scores.

---

## Why Sampling is Required
In real-world fraud detection:
- Fraud cases are very rare
- Models trained on imbalanced data tend to ignore minority classes
- Sampling helps balance the dataset and improve detection of fraud cases

---

## Sampling Techniques Used

| Sampling Code | Technique |
|--------------|----------|
| Sampling1 | Random Oversampling |
| Sampling2 | Random Undersampling |
| Sampling3 | SMOTE |
| Sampling4 | SMOTE + ENN |
| Sampling5 | SMOTE + Tomek Links |

---

## Machine Learning Models Used

| Model Code | Algorithm |
|----------|-----------|
| M1 | Logistic Regression |
| M2 | Random Forest |
| M3 | Decision Tree |
| M4 | Naive Bayes |
| M5 | Support Vector Machine (SVM) |

---

## Accuracy Results

| Model | Sampling1 | Sampling2 | Sampling3 | Sampling4 | Sampling5 |
|------|----------|----------|----------|----------|----------|
| M1 | 50.10 | 52.24 | 63.18 | 69.23 | 70.12 |
| M2 | 59.25 | 65.27 | 68.72 | 28.36 | 30.25 |
| M3 | 90.45 | 72.41 | 32.17 | 42.58 | 41.85 |
| M4 | 78.25 | 56.24 | 47.23 | 33.44 | 40.12 |
| M5 | 81.25 | 12.85 | 57.36 | 32.25 | 52.74 |

---

## Best Sampling Technique per Model

| Model | Best Sampling Technique |
|-----|-------------------------|
| Logistic Regression (M1) | Sampling5 |
| Random Forest (M2) | Sampling3 |
| Decision Tree (M3) | Sampling1 |
| Naive Bayes (M4) | Sampling1 |
| SVM (M5) | Sampling1 |

---

## Key Observations
- Oversampling techniques work well with tree-based models
- SMOTE improves generalization for ensemble models
- Undersampling may lead to loss of important data
- No single sampling technique is universally optimal

---

## Conclusion
Sampling techniques play a crucial role in handling imbalanced datasets. The effectiveness of a sampling method depends on the machine learning model used. Selecting the right combination of sampling strategy and model leads to better fraud detection performance.

---

## Submission
- All code and results are available in this GitHub repository
- Assignment submitted as per university guidelines

---
