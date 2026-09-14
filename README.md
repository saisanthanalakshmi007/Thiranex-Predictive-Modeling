# Employee Attrition Prediction Using Machine Learning

## Thiranex Data Science Internship — Task 2

**Author: Sai Santhana Lakshmi S**

---

## Project Overview

This project focuses on predicting employee attrition using supervised machine learning.

A synthetic employee dataset was created for this project. The Random Forest Classifier was trained to predict whether an employee is likely to stay with the organization or leave.

The project also evaluates the model using accuracy, precision, recall, F1-score, a confusion matrix, ROC curve, and AUC score.

## Dataset

The dataset contains 100 synthetic employee records with the following features:

- Age
- Monthly Income
- Job Satisfaction
- Years at Company
- Overtime
- Work-Life Balance
- Job Level
- Attrition

### Target Variable

- `0` — Employee Stayed
- `1` — Employee Left

## Machine Learning Workflow

1. Created an original synthetic dataset
2. Checked for missing values and duplicate records
3. Converted categorical data into numerical form
4. Separated features and target variable
5. Split the dataset into training and testing sets
6. Trained a Random Forest Classifier
7. Generated predictions and prediction probabilities
8. Evaluated model performance
9. Created a confusion matrix
10. Created a ROC curve and calculated AUC
11. Analyzed feature importance

## Model

### Random Forest Classifier

The Random Forest model was trained using:

- 100 decision trees
- Random state: 42
- Training data: 80%
- Testing data: 20%

## Model Performance

| Metric | Score |
|---|---:|
| Accuracy | 75.00% |
| Precision | 75.00% |
| Recall | 66.67% |
| F1-Score | 70.59% |
| AUC | 0.69 |

## Feature Importance

The three most important features identified by the Random Forest model were:

1. Age — 0.238
2. Monthly Income — 0.216
3. Years at Company — 0.192

## Visualizations

### Confusion Matrix

The confusion matrix shows the number of correct and incorrect predictions for employees who stayed and employees who left.

### ROC Curve

The ROC curve evaluates the model's ability to distinguish between employees who stayed and employees who left.

The model achieved an AUC score of **0.69**.

### Feature Importance

The feature importance chart shows the relative contribution of each input feature to the Random Forest predictions.

## Tools and Technologies

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- Jupyter Notebook

## Project Structure

```text
Thiranex_Task2_Predictive_Modeling/
│
├── Predictive_Modeling.ipynb
├── employee_attrition_data.csv
├── README.md
│
└── visualizations/
    ├── confusion_matrix.png
    ├── roc_curve.png
    └── feature_importance.png