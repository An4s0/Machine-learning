# ARTI308 - Machine Learning Lab 3

## Overview
This lab focuses on the exploratory data analysis (EDA) of sales data from a coffee vending machine. The goal is to perform data cleaning, statistical summarization, and univariate visualization to understand purchasing patterns and customer preferences.

## Dataset Description
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

## Lab Assessment Tasks (`lab3.ipynb`)
1. Setup: import libraries, load CSV.
2. Data Inspection: first rows, missing values, types.
3. Preprocessing: convert dates, extract hour and day.
4. Statistics: summary of numeric and categorical features.
5. Visualization:
   - **Univariate:** histogram, boxplot, violin, countplot, pie.
   - **Bivariate:** boxplot/violin by cash type, barplot by coffee type, stacked bar & heatmap.
   - **Time-Based:** revenue by hour/day, cumulative sales.
   - **Correlation:** heatmap, pairplot.
6. Each plot includes short explanation below it.