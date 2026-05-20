# Cybersecurity Incident Response Predictor

## Overview

This project predicts the appropriate response action for cybersecurity incidents based on attack characteristics. It was developed as part of AI/ML practice focused on cybersecurity applications.

Current status: Work in progress. The baseline model currently achieves approximately 25% accuracy, which is close to random guessing for a four-class classification problem.

---

## Problem Statement

Given cybersecurity incident attributes such as attack type, severity, timestamp, and data exfiltration status, predict the most suitable response action.

### Response Classes

* Eradicated — Threat completely removed
* Contained — Threat isolated but still present
* Recovered — Systems restored after incident
* Blocked — Attack prevented before impact

---

## Dataset

* Synthetic cybersecurity incident dataset
* 10,000+ incident records
* Includes:

  * Attack Type
  * Attack Severity
  * Data Exfiltrated
  * Timestamp
* Target variable:

  * Response Action

---

## Technologies Used

* Python
* Pandas
* NumPy
* Scikit-learn
* Matplotlib
* Seaborn

---

## Current Performance

| Metric            | Value             |
| ----------------- | ----------------- |
| Accuracy          | 25%               |
| Baseline Accuracy | 25%               |
| Status            | Under Improvement |

---

## Key Learnings

* Baseline accuracy for a four-class classification problem is 25%
* Class imbalance affects model performance significantly
* Feature engineering is important for improving predictions
* Adding more features does not always improve results
* Proper preprocessing and feature selection are critical

---

## Improvement Roadmap

* Handle class imbalance using class weights
* Perform feature selection
* Implement cross-validation using StratifiedKFold
* Compare multiple algorithms:

  * Logistic Regression
  * Decision Tree
  * Random Forest
  * XGBoost
* Perform hyperparameter tuning with GridSearchCV
* Add time-based feature engineering

---

## Project Workflow

1. Data preprocessing
2. Handling missing values
3. Encoding categorical features
4. Feature engineering
5. Train-test split
6. Model training
7. Model evaluation
8. Performance improvement

---

## Future Enhancements

* Real-time threat prediction system
* Deployment using Flask or Streamlit
* Integration with SIEM tools
* Deep learning-based anomaly detection
* Real cybersecurity datasets for benchmarking

---

## Project Structure

```text
Cybersecurity-incident-response/
│
└── ai_ml_cybersecurity_dataset.csv
│
└── cybersecurity_model.ipynb
│
├── confusion_matrix.png
├── class_distribution.png
└── feature_importance.png
│
├── README.md
```
