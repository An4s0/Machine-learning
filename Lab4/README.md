# ARTI308 - Machine Learning Lab 4
## Data Quality Assessment & Preprocessing

### Overview
This project focuses on the systematic cleaning and preprocessing of the "Chocolate Sales" dataset. The primary objective is to transform raw, inconsistent data into a structured format suitable for machine learning algorithms. This involves identifying data quality issues, handling missing values, removing outliers, normalizing features, and applying dimensionality reduction.

### Dataset
**Chocolate Sales Dataset**

**Features:**
* **Sales Person**: The individual responsible for the sale.
* **Country**: The region where the sale occurred.
* **Product**: The type of chocolate product sold.
* **Date**: The date of the transaction.
* **Amount**: The monetary value of the transaction (requires cleaning).
* **Boxes Shipped**: The quantity of boxes shipped.

### Lab Tasks
1. **Data Inspection & Cleaning**: Identified and corrected formatting issues (e.g., currency symbols, commas) and ensured proper data types (datetime, float).
2. **Missing Value Imputation**: Addressed missing data points using the median imputation strategy.
3. **Outlier Detection**: Detected and removed extreme values using the Interquartile Range (IQR) method to prevent bias in the analysis.
4. **Feature Normalization**: Applied Min-Max Scaling and Z-score Standardization to numerical features (`Amount` and `Boxes Shipped`) to bring them to a common scale.
5. **PCA Application**: Performed Principal Component Analysis (PCA) to reduce dimensionality and analyzed the explained variance ratio of the components.
