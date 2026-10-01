# Customer-Churn-Prediction-Project
![language](https://img.shields.io/badge/language-Python-blue)
![domain](https://img.shields.io/badge/domain-Customer%20Analytics-green)
![method](https://img.shields.io/badge/method-Machine%20Learning-orange)
![type](https://img.shields.io/badge/type-Academic%20Project-lightgrey)

Machine learning project for predicting customer churn, identifying high-risk customers, and supporting targeted retention strategies through customer propensity modeling.

## Project Overview

Customer churn prediction is an important task in customer relationship management, as identifying customers at risk of leaving can support more effective retention strategies.

This project develops an end-to-end machine learning pipeline to predict customer churn using demographic, behavioral, transactional, and satisfaction-related features.

The analysis focuses on two main questions:

- **Churn Prediction:** Can customer characteristics and behavioral patterns be used to accurately identify customers at risk of churn?
- **Retention Targeting:** Which customers should be prioritized for targeted retention actions?

## Dataset

The analysis uses a customer churn dataset containing 5,630 observations and 20 variables describing customer demographics, purchasing behavior, app usage, satisfaction, and transactional characteristics.

### Target Variable

`Churn`

Binary variable representing customer churn:

- 1 → Churned customer
- 0 → Retained customer

Approximately 16.8% of customers in the dataset are classified as churners.

## Methods

### Machine Learning Modeling

The prediction task is formulated as a binary classification problem.

The analytical workflow includes:

1. **Data Quality Assessment:** Analysis of missing values, inconsistent categorical values, and potential outliers.
2. **Exploratory Data Analysis:** Examination of customer characteristics and churn-related patterns.
3. **Data Preprocessing:** Handling of missing values, categorical variables, and feature transformations.
4. **Model Training:** Training and comparison of machine learning classification models.
5. **Hyperparameter Tuning:** Optimization of the selected model.
6. **Model Evaluation:** Assessment using recall, F1-score, and ROC-AUC.
7. **Customer Risk Segmentation:** Identification of customers with the highest churn propensity.
8. **Retention Strategy:** Translation of model predictions into targeted customer retention actions.

## Results and Insights

The final model achieved:

- **Recall:** 97.9%
- **F1-score:** 92.5%
- **ROC-AUC:** 99.8%

### Model Performance

![Confusion Matrix](images/confusion_matrix.png)

The model correctly identified **185 out of 189 churners**, showing a very low number of false negatives.

![Cumulative Gains Curve](images/cumulative_gains.png)

By targeting the **top 20% of customers ranked by churn probability**, the model captures approximately **98.9% of churners**.

### Main Churn Drivers

![Feature Importance](images/churn_drivers.png)

Feature importance analysis highlights the main variables associated with customer churn, including customer tenure, cashback behavior, and complaints.

## Tech Stack

Language:

- Python

Libraries:

- pandas
- numpy
- scikit-learn
- matplotlib

Methods:

- supervised machine learning
- binary classification
- feature preprocessing
- hyperparameter tuning
- churn propensity modeling
- customer risk segmentation

## Project Materials

Additional materials for this project are available below.

- **Project Notebook:** Full customer churn analysis and machine learning pipeline.
- **Project Summary:** Presentation of the methodology, results, and retention strategy.

## Author

Irene Marrali

BSc in Artificial Intelligence @ Università degli Studi di Milano, Università degli Studi di Pavia, Università degli Studi di Milano-Bicocca
