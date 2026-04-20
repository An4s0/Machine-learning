# ARTI308 - Machine Learning Lab 7

## Overview

This lab focuses on the practical application of Logistic Regression for binary classification tasks using an Advertising dataset. The objective is to build a Logistic Regression model to predict whether a user will click on an advertisement (`Clicked on Ad`) and analyze how exploratory analysis, feature selection, and model evaluation reflect the model's classification performance.

## Dataset

**Advertising Dataset**

**Features:**

- **Behavioral**: `Daily Time Spent on Site`, `Daily Internet Usage`
- **Demographic**: `Age`, `Area Income`, `Male`
- **Categorical**: `Ad Topic Line`, `City`, `Country`
- **Temporal**: `Timestamp`
- **Target**: `Clicked on Ad` (0 = Not Clicked, 1 = Clicked)

## Lab Tasks

1. **Data Inspection**: Loaded and inspected the dataset to understand data types, distributions, and confirm there are no missing values.
2. **Exploratory Data Analysis (EDA)**:
   - Plotted the distribution of the `Age` feature using a histogram.
   - Created jointplots to examine relationships between `Age` vs `Area Income`, `Age` vs `Daily Time Spent on Site`, and `Daily Time Spent on Site` vs `Daily Internet Usage`.
   - Generated a pairplot with hue set to `Clicked on Ad` to visualize class separability across all features.
3. **Feature Preparation**: Selected relevant numeric features and defined the target variable, then split the data into training and test sets.
4. **Baseline Modeling**: Trained a Logistic Regression model on the training set to classify whether a user clicked on the ad.
5. **Model Evaluation**: Assessed model performance using a classification report (precision, recall, F1-score) and a confusion matrix to measure prediction accuracy across both classes.
