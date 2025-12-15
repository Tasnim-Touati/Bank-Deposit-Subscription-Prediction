# 🏦 Bank Deposit Subscription Prediction

[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/Tasnim-Touati/Bank-Deposit-Subscription-Prediction/main?filepath=bank_marketing_prediction.ipynb)

## Overview

This repository contains a Jupyter Notebook for a mini-project focused on predicting whether a client will subscribe to a bank term deposit (`y = yes/no`).  

The project uses the well-known **Bank Marketing Dataset** (UCI) and addresses real-world machine learning challenges:

- Binary classification with severe class imbalance (~88.3% "no" vs ~11.7% "yes")
- Mixed data types (categorical + numerical)
- Hidden missing values labeled as "unknown"
- Data leakage risk (the `duration` feature cannot be used in production)
- Business-oriented optimization of marketing campaigns

The workflow includes:
- Exploratory data analysis
- Data preprocessing
- SVM modeling with hyperparameter tuning (GridSearchCV)
- Threshold optimization to maximize F1-score on the minority class
- Business interpretation of results

**Final model performance** (SVM with RBF kernel, C=10, gamma=0.1):  
- Optimal decision threshold: **0.19**  
- F1-score: **0.61**  
- Precision: **0.54**  
- Recall: **0.70**

Author: **Touati Tasnim** 

Dataset source: [UCI Bank Marketing Dataset](https://archive.ics.uci.edu/dataset/222/bank+marketing)
