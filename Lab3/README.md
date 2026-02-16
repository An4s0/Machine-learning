# ARTI308 - Machine Learning Lab 3

## 1. Overview
This lab focuses on the exploratory data analysis (EDA) of sales data from a coffee vending machine. The goal is to perform data cleaning, statistical summarization, and univariate visualization to understand purchasing patterns and customer preferences.

## 2. Dataset Description
The dataset, `coffee_sales.csv`, contains detailed transaction records from a vending machine.

**File Structure:**
The dataset consists of 262 rows and 5 columns.

**Feature Definitions:**
- **date:** The calendar date of the transaction.
- **datetime:** The precise timestamp (date and time) of the sale.
- **cash_type:** The payment method used, either "card" or "cash".
- **money:** The amount paid for the beverage (numeric).
- **coffee_name:** The specific name of the beverage purchased.

**Summary Statistics:**
- **Total Transactions:** 262.
- **Payment Preference:** Transactions are primarily made by card (182 instances) compared to cash.
- **Most Popular Item:** "Americano with milk" is the most frequently purchased beverage (44 times).
- **Average Price:** The mean transaction value is approximately 26.30.
- **Price Range:** Sales range from a minimum of 15.0 to a maximum of 33.0.

## 3. Lab Assessment Tasks (`lab3.ipynb`)
The assessment notebook follows a simplified data science workflow:

1. **Environment Setup:** Importing pandas, numpy, matplotlib, and seaborn, and loading the source CSV. 
2. **Data Inspection:** Displaying the first 5 rows to understand the structure. 
3. **Quality Check:** Verifying there are no missing values across the dataset features. 
4. **Preprocessing:** Converting the date and datetime columns into datetime64 format. 
5. **Descriptive Statistics:** Generating a summary of all categorical and numerical features. 
6. **Univariate Visualization**: 
    * **Histogram**: Visualizing the distribution of sales amounts (`money`).
    * **Count Plot**: Comparing the frequency of different coffee types sold.