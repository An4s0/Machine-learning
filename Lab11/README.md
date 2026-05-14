# ARTI308 - Machine Learning Lab 11

## Overview

This lab focuses on implementing K-Means clustering for customer segmentation using credit card usage data. The objective is to apply unsupervised learning techniques to discover hidden patterns in customer behavior, segment customers into meaningful groups, and provide actionable insights for marketing strategies.

## Dataset

**Credit Card Customer Dataset (CC_GENERAL.csv)**

**Features:**

- **Balance Information**: `BALANCE`, `BALANCE_FREQUENCY`
- **Purchase Behavior**: `PURCHASES`, `ONEOFF_PURCHASES`, `INSTALLMENTS_PURCHASES`, `PURCHASES_FREQUENCY`, `ONEOFF_PURCHASES_FREQUENCY`, `PURCHASES_INSTALLMENTS_FREQUENCY`, `PURCHASES_TRX`
- **Cash Advance**: `CASH_ADVANCE`, `CASH_ADVANCE_FREQUENCY`, `CASH_ADVANCE_TRX`
- **Payment Information**: `PAYMENTS`, `MINIMUM_PAYMENTS`, `PRC_FULL_PAYMENT`
- **Credit Information**: `CREDIT_LIMIT`, `TENURE`
- **Identifier**: `CUST_ID` (removed before clustering)
- **Target**: None (unsupervised learning - no predefined labels)

## Lab Tasks

1. **Data Loading**: Loaded the credit card dataset and performed initial exploration using `head()`, `shape`, `info()`, and `describe()` methods.
2. **Data Cleaning**: Removed the `CUST_ID` identifier column as it doesn't represent customer behavior, identified missing values in `CREDIT_LIMIT` and `MINIMUM_PAYMENTS`, and applied mean imputation to handle missing data.
3. **Exploratory Data Analysis (EDA)**: Created histograms for all numerical features to understand distributions, generated correlation heatmap to identify feature relationships, and created scatter plots for `BALANCE` vs `PURCHASES` and `BALANCE` vs `CASH_ADVANCE`.
4. **Feature Scaling**: Applied `StandardScaler` to normalize all features (critical for distance-based K-Means algorithm to ensure equal feature contribution).
5. **Elbow Method**: Tested K values from 1 to 10, plotted inertia values to identify the optimal number of clusters where decrease starts to slow down.
6. **Silhouette Score Analysis**: Calculated silhouette scores for K values from 2 to 10, plotted scores and created comparison table to evaluate cluster quality and separation.
7. **Final K-Means Model**: Selected K=4 based on elbow method and silhouette score analysis, trained final model with `random_state=42` and `n_init=10`, and added cluster labels to original dataframe.
8. **Cluster Analysis**: Generated summary statistics for each cluster using `groupby()`, counted customers per cluster, and interpreted cluster characteristics to identify customer segments.
9. **Dimensionality Reduction Visualization**: Applied PCA with 2 components to visualize high-dimensional clusters in 2D space, plotted clusters with color coding to show separation patterns.
10. **Business Insights**: Identified four distinct customer segments (Transactors, High-value customers, Cash advance users, and Low activity customers) and provided marketing strategy recommendations for each segment to maximize customer lifetime value.
