# ARTI308 - Machine Learning Lab 9

## Overview

This lab focuses on implementing Decision Trees and Random Forests for binary classification using a lending dataset. The objective is to build models to predict loan default risk and compare the performance of single decision trees versus ensemble methods.

## Dataset

**Loan Data Dataset**

**Features:**

- **Credit/Financial**: `credit.policy`, `fico`, `int.rate`, `installment`, `log.annual.inc`, `dti`, `revol.bal`, `revol.util`, `days.with.cr.line`
- **Credit History**: `inq.last.6mths`, `delinq.2yrs`, `pub.rec`
- **Categorical**: `purpose` (loan purpose)
- **Target**: `not.fully.paid` (0 = Fully Paid, 1 = Not Fully Paid)

## Lab Tasks

1. **Data Inspection**: Loaded and explored the dataset using `info()`, `describe()`, and `head()` methods.
2. **Exploratory Data Analysis (EDA)**: Created histograms of FICO scores by `credit.policy` and `not.fully.paid`, countplot of loan purposes, jointplot of FICO vs interest rate, and lmplots for trend analysis.
3. **Feature Engineering**: Converted `purpose` categorical feature into dummy variables using `pd.get_dummies()`.
4. **Train-Test Split**: Split data into 70% training and 30% testing sets.
5. **Decision Tree Model**: Trained Decision Tree classifier and evaluated using confusion matrix and classification report, achieving ~72% accuracy.
6. **Random Forest Model**: Trained Random Forest with 600 estimators, achieving ~85% accuracy.
7. **Model Comparison**: Random Forest outperformed Decision Tree in overall accuracy, though both struggled with predicting the minority class (loan defaults).
