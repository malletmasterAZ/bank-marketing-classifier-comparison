# Bank Marketing Classifier Comparison

## Overview
This project compares multiple classification models to predict whether a contacted client will subscribe to a term deposit using the UCI Bank Marketing dataset. The goal is to evaluate model performance and identify the most effective approach for improving marketing efficiency.

---

## Business Objective
The objective of this project is to build a classification model that predicts whether a contacted client will subscribe to a term deposit (y). By accurately identifying likely subscribers, the bank can improve campaign efficiency, reduce unnecessary outreach, and allocate marketing resources more effectively.

---

## Dataset
- Source: UCI Machine Learning Repository
- 17 marketing campaigns (May 2008 to November 2010)
- 41,188 observations
- Highly imbalanced (~12% positive class)

---

## Baseline Performance
Baseline accuracy (predicting the majority class) ≈ 88.7%.
All models were required to outperform this baseline.

---

## Models Compared
- Logistic Regression
- K-Nearest Neighbors (KNN)
- Decision Tree
- Support Vector Machine (SVM)

---

## Results

Test Accuracy:
- Logistic Regression: 0.9098
- SVM: 0.9058
- KNN: 0.8984
- Decision Tree: 0.8732

Logistic Regression achieved the highest overall test accuracy.

---

## Model Evaluation (Beyond Accuracy)

ROC AUC (Logistic Regression): 0.917

Classification Report (Positive Class):
- Precision: 0.69
- Recall: 0.37

Although overall accuracy is high, recall for actual subscribers is low due to class imbalance.

---

## Key Insights
- The dataset is highly imbalanced.
- Accuracy alone is not an ideal metric.
- Logistic Regression provides the best balance of performance and stability.
- Decision Trees showed clear overfitting under default settings.

---

## Recommendations
- Optimize for recall or F1 score instead of accuracy.
- Apply class weighting or resampling methods to address imbalance.
- Remove the duration feature for a more realistic predictive model.
- Explore ensemble methods such as Random Forest or Gradient Boosting.

---

## Technologies Used
- Python
- Pandas
- Scikit-learn
- Jupyter Notebook
