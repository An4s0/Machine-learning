# ARTI308 - Machine Learning Lab 8

## Overview

This lab focuses on implementing K-Nearest Neighbors (KNN) for binary classification using an artificial dataset. The objective is to build a KNN classifier, apply feature scaling, use the elbow method to find the optimal K value, and evaluate model performance.

## Dataset

**KNN Project Dataset**

**Features:**

- **Numerical Features**: `XVPM`, `GWYH`, `TRAT`, `TLLZ`, `IGGA`, `HYKR`, `EDFS`, `GUUB`, `MGJM`, `JHZC` (10 anonymized features)
- **Target**: `TARGET CLASS` (0 or 1 - binary classification)

## Lab Tasks

1. **Data Inspection**: Loaded and explored the dataset structure.
2. **Exploratory Data Analysis (EDA)**: Created a pairplot with hue set to `TARGET CLASS` to visualize class separability.
3. **Feature Standardization**: Applied `StandardScaler` to normalize features (critical for distance-based KNN algorithm).
4. **Train-Test Split**: Split data into 70% training and 30% testing sets.
5. **Baseline Model**: Trained KNN with `n_neighbors=1` and evaluated performance using confusion matrix and classification report.
6. **Optimal K Selection**: Implemented elbow method testing K values 1-39, plotted error rates to identify optimal K.
7. **Model Optimization**: Retrained with K=30, achieving ~84% accuracy with balanced precision and recall.