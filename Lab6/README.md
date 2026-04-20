# ARTI308 - Machine Learning Lab 6

## Overview
This lab focuses on the practical application of Linear Regression for predicting continuous outcomes using an E-commerce Customers dataset. The objective is to build a Linear Regression model to predict `Yearly Amount Spent` and analyze how data exploration, feature preparation, and model evaluation—such as examining coefficients, residuals, and error metrics—reflect the model's predictive performance.

## Dataset
**Ecommerce Customers Dataset**

**Features:**
* **Identifiers**: `Email`, `Address`, `Avatar`
* **Behavioral**: `Avg. Session Length`, `Time on App`, `Time on Website`, `Length of Membership`
* **Numerical**: `Yearly Amount Spent` (Target)

## Lab Tasks
1. **Data Inspection**: Loaded and inspected the dataset to understand data types and identify non-numeric columns to exclude from modeling.
2. **Exploratory Data Analysis (EDA)**:
    * Visualized feature relationships using a pairplot.
    * Plotted the distribution of the target variable `Yearly Amount Spent`.
    * Generated a correlation heatmap to identify the most influential features.
3. **Feature Preparation**: Selected relevant numeric features and defined the target variable, then split the data into training and test sets.
4. **Baseline Modeling**: Trained a Linear Regression model and inspected model coefficients to interpret the effect of each feature on yearly spending.
5. **Model Evaluation**: Assessed model performance using MAE, MSE, RMSE, and R² metrics, and analyzed residuals to validate model assumptions.
