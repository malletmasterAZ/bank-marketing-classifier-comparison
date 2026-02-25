# bank-marketing-classifier-comparison
Bank Marketing Classifier Comparison
Business Objective
The goal of this project is to build and compare multiple classification models to predict whether a contacted client will subscribe to a term deposit. The objective is to improve marketing efficiency by identifying likely subscribers and reducing unnecessary outreach.
Dataset
UCI Bank Marketing Dataset (Portuguese bank telemarketing campaigns, 17 campaigns from 2008–2010).
Models Compared
Logistic Regression
K-Nearest Neighbors
Decision Tree
Support Vector Machine
Key Findings
Logistic Regression achieved the highest test accuracy (≈ 91%).
The dataset is highly imbalanced (~12% positive class).
ROC AUC (≈ 0.92) provided a better performance measure than accuracy.
Decision Trees showed overfitting under default settings.
Recommendations
Use recall or AUC instead of accuracy for evaluation.
Consider class weighting or resampling to improve recall.
Remove the duration feature for a realistic predictive model.
