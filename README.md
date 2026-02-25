# Bank Marketing Classifier Comparison

## Overview

This project compares multiple classification models to predict whether a contacted client will subscribe to a term deposit using the UCI Bank Marketing dataset.

The goal is to evaluate model performance and identify the most effective approach for improving marketing efficiency.

---

## Business Objective

The objective of this project is to build a classification model that predicts whether a contacted client will subscribe to a term deposit (`y`). 

By accurately identifying likely subscribers, the bank can:
- Improve campaign efficiency  
- Reduce unnecessary outreach  
- Allocate marketing resources more effectively  

---

## Dataset

- Source: UCI Machine Learning Repository  
- Portuguese bank telemarketing campaigns  
- 17 campaigns (May 2008 to November 2010)  
- 41,188 observations  
- Highly imbalanced (~12% positive class)

---

## Data Preparation

### Convert Target Variable

```python
y = df['y'].map({'no': 0, 'yes': 1})
