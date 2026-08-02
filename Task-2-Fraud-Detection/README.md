# Task 2: Supervised Learning Fraud Detection Pipeline(WEEK-2)
## Project Title
**Supervised Learning Fraud Detection Pipeline**

## Project Overview

This project focuses on building a supervised machine learning pipeline to detect fraudulent credit card transactions. The objective is to analyze transaction data, handle class imbalance, train classification models, and identify the best-performing model for fraud detection.

The project follows a complete machine learning workflow, including data preprocessing, handling imbalanced data using SMOTE, model training, evaluation, comparison, and saving the final trained model.

## Problem Statement

Fraudulent transactions are difficult to detect because they represent a very small percentage of total transactions. This project aims to develop a machine learning solution that can accurately identify fraudulent activities while reducing incorrect predictions.

## Dataset

**Credit Card Fraud Detection Dataset**

The dataset contains transaction-related features with a target variable that classifies transactions as:

* Fraudulent transactions
* Legitimate transactions

The dataset is highly imbalanced, making fraud detection a challenging classification problem.

## Technologies & Tools Used

**Programming Language**

* Python

**Development Environment**

* Google Colab / Jupyter Notebook

**Libraries**

* Pandas – Data processing and analysis
* NumPy – Numerical operations
* Matplotlib – Data visualization
* Scikit-learn – Machine learning algorithms and evaluation
* Imbalanced-learn (SMOTE) – Handling class imbalance
* Joblib – Saving the trained model

## Machine Learning Workflow

The project was implemented through the following steps:

1. Data loading and exploration
2. Data preprocessing and preparation
3. Handling class imbalance using SMOTE
4. Splitting data into training and testing sets
5. Training classification models
6. Evaluating models using performance metrics
7. Comparing models and selecting the best model
8. Saving the final trained model

## Models Implemented

### 1. Logistic Regression

A baseline classification model used to identify fraudulent transactions.

### 2. Random Forest Classifier

An ensemble learning algorithm used to improve fraud detection performance by combining multiple decision trees.

## Model Evaluation Metrics

The models were evaluated using:

* **Precision:** Measures the correctness of fraud predictions.
* **Recall:** Measures the ability to detect actual fraudulent transactions.
* **F1-Score:** Provides a balance between precision and recall.
* **ROC-AUC Score:** Measures the model's ability to distinguish between fraud and legitimate transactions.

## Model Comparison & Result

After comparing both models:

* Logistic Regression achieved higher Recall and ROC-AUC.
* Random Forest achieved better Precision and F1-score.

Since fraud detection requires a balance between detecting fraud cases and reducing false alarms, **Random Forest was selected as the final model.**

## Final Model

**Selected Model:** Random Forest Classifier

The final trained model was saved as:

`fraud_detection_random_forest.pkl`

This saved model can be used for future fraud prediction applications.

## Project Files

```
Task 2/
│
├── Fraud_Detection.ipynb
├── fraud_detection_random_forest.pkl
└── README.md
```

## Future Enhancements

The project can be further improved by:

* Performing hyperparameter tuning using GridSearchCV or RandomizedSearchCV.
* Testing additional machine learning algorithms.
* Developing a real-time fraud detection application.
* Deploying the model using Flask or Streamlit.
* Implementing continuous model monitoring.

## Conclusion

This project successfully developed a supervised learning fraud detection pipeline using machine learning techniques. The workflow included data preprocessing, imbalance handling, model training, evaluation, model comparison, and final model selection.

The Random Forest model was selected as the final model because it provided a better balance between Precision and F1-score, making it suitable for fraud detection tasks.
