# ARTI308 - Machine Learning Lab 5

## Overview
This lab focuses on the practical application of feature engineering for classification tasks using a "Talabat-style" order dataset. The objective is to build a baseline Random Forest model to predict `Order_Status` and analyze how engineering decisions—such as creating time-based features, handling category cardinality, and feature selection—impact the model's predictive performance and feature importance.

## Dataset
**Talabat-style Orders Dataset**

**Features:**
* **IDs**: `Order_ID`, `User_ID`, `Restaurant_ID`, `Driver_ID`
* **Temporal**: `Order_Time`, `Delivery_Time`, `Delivery_Duration_Minutes`
* **Spatial**: `City`, `Delivery_Distance_km`, `Restaurant_Lat/Lon`, `Customer_Lat/Lon`
* **Categorical**: `Item_Name`, `Payment_Method`, `Order_Status` (Target), `Driver_Vehicle`, `Traffic_Level`, `Driver_Availability`
* **Numerical**: `Quantity`, `Total_Price`

## Lab Tasks
1. **Data Inspection**: Loaded and inspected the dataset to understand data types and potential leakage features.
2. **Feature Engineering**:
    * Created new features (e.g., `Is_Weekend`, `is_peak_hour`).
    * Applied category reduction to `Item_Name` (grouping low-frequency items into 'Other').
3. **Encoding**: Encoded categorical features to numeric format for model compatibility.
4. **Baseline Modeling**: Trained a Random Forest classifier to establish a performance baseline.
5. **Feature Selection & Optimization**: Analyzed feature importances and evaluated the model after selecting top-performing features to optimize accuracy and reduce complexity.

