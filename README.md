# Credit Card Fraud Detection (Machine Learning)

This project builds a machine learning model to detect fraudulent credit card transactions using a highly imbalanced dataset.

## Problem

Fraud detection is challenging due to extreme class imbalance; less than 0.2% of transactions are fraudulent.  
A model can achieve high accuracy by predicting all transactions as non-fraud, but this fails in practice.

The goal of this project is to correctly identify fraudulent transactions while minimising missed fraud cases.

---

## Dataset

The dataset is publicly available on Kaggle:

https://www.kaggle.com/datasets/mlg-ulb/creditcardfraud

- 284,000+ transactions  
- Highly imbalanced (fraud ≈ 0.17%)  

---

## Approach

- Data exploration and preprocessing  
- Feature scaling (Amount column)  
- Train-test split with stratification  
- Built two models:
  - Logistic Regression (baseline)
  - Random Forest (improved model)  
- Evaluated performance using:
  - Precision
  - Recall
  - F1-score
  - Confusion matrix  

---

## Results

- Logistic Regression struggled to detect fraud due to class imbalance  
- Random Forest significantly improved recall (fraud detection rate)  
- Achieved:
  - Recall ≈ 76%  
  - Precision ≈ 99%  

---

## Key Insight

Accuracy is not a reliable metric for imbalanced datasets.  
In fraud detection, recall is more important because missing fraudulent transactions is more costly than false positives.

---

## How to Run

1. Download the dataset from Kaggle link above  
2. Place `creditcard.csv` in the project folder  
3. Open and run `fraud_detection.ipynb`

---

## Technologies Used

- Python  
- Pandas  
- NumPy  
- scikit-learn  
- Matplotlib  
