# ARTI308 - Machine Learning Lab 10

## Overview

This lab focuses on implementing Support Vector Machines (SVM) for multi-class classification using the Iris dataset. The objective is to build an SVM classifier, visualize feature relationships, optimize hyperparameters using GridSearchCV, and evaluate model performance across three flower species.

## Dataset

**Iris Dataset**

**Features:**

- **Sepal Measurements**: `sepal_length`, `sepal_width`
- **Petal Measurements**: `petal_length`, `petal_width`
- **Target**: `species` (setosa, versicolor, virginica - 3-class classification)

## Lab Tasks

1. **Data Loading**: Loaded the Iris dataset from sklearn and created a pandas DataFrame with properly renamed columns for easier analysis.
2. **Exploratory Data Analysis (EDA)**:
   - Created a pairplot with hue set to `species` to visualize feature relationships and class separability across all four features.
   - Generated a KDE (Kernel Density Estimation) plot for the setosa species, examining the relationship between `sepal_length` and `sepal_width`.
3. **Train-Test Split**: Split data into 70% training and 30% testing sets with random state for reproducibility.
4. **Baseline SVM Model**: Trained a Support Vector Classifier with default parameters and evaluated using confusion matrix and classification report.
5. **Hyperparameter Tuning**: Implemented GridSearchCV to optimize C and gamma parameters, testing multiple combinations to find the best model configuration.
6. **Model Optimization**: Retrained SVM with optimized hyperparameters from grid search and compared performance against baseline model.
7. **Model Evaluation**: Assessed both baseline and optimized models using classification reports and confusion matrices to measure prediction accuracy and determine if hyperparameter tuning improved performance on the highly separable Iris dataset.
