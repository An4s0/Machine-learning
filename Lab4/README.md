# ARTI308 - Machine Learning Lab 3

## Overview

This lab analyzes 50,000 user records related to smartphone usage, productivity, sleep patterns, and stress levels. The main objective is to assess data quality, handle missing values and outliers, normalize features, and apply PCA to prepare the dataset for machine learning tasks.

## Dataset

**Smartphone Usage, Productivity & Lifestyle Analytics (50K Records)**

**Features:**

* Age, Gender, Occupation, Device_Type
* Daily_Phone_Hours, Social_Media_Hours
* Work_Productivity_Score, Sleep_Hours, Stress_Level
* App_Usage_Count, Caffeine_Intake_Cups, Weekend_Screen_Time_Hours

**Dataset Stats:** 50,000 records, no missing values, balanced categorical features, numerical features ready for scaling and ML analysis.

## Lab Tasks

1. Load dataset and inspect first rows, data types, and missing values.
2. Fill missing values (if any) and remove outliers using IQR.
3. Normalize numerical features using Min-Max scaling and Z-score standardization.
4. Apply PCA, analyze explained variance, and reduce dimensionality.
5. Visualize data: boxplots for features after outlier removal, scatter plot of first two principal components.

## Use Cases

* Predicting productivity levels (regression)
* Stress level classification
* Behavioral clustering and sleep impact analysis
* Device-based productivity comparison
* Feature engineering and correlation analysis

**Target Audience:** Data scientists, ML practitioners, behavioral researchers, and productivity analysts.
