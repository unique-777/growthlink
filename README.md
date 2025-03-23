# Customer Churn Prediction 

## Overview
This project involves performing Exploratory Data Analysis (EDA) on a customer churn dataset to gain insights and prepare the data for machine learning models. The dataset contains information about customers, including demographic details, account balance, tenure, credit score, and whether they have churned (Exited).

## Dataset Information
The dataset consists of the following key columns:
- **RowNumber**: Index of the row
- **CustomerId**: Unique identifier for each customer
- **Surname**: Last name of the customer
- **CreditScore**: Customer's credit score
- **Geography**: Country of the customer
- **Gender**: Male or Female
- **Age**: Age of the customer
- **Tenure**: Number of years with the bank
- **Balance**: Account balance
- **NumOfProducts**: Number of products held
- **HasCrCard**: Whether the customer has a credit card (1 = Yes, 0 = No)
- **IsActiveMember**: Whether the customer is an active member (1 = Yes, 0 = No)
- **EstimatedSalary**: Estimated annual salary
- **Exited**: Target variable (1 = Churned, 0 = Stayed)

## Data Cleaning & Preprocessing
1. **Dropped Unnecessary Columns**:
   - Removed `RowNumber`, `CustomerId`, and `Surname` as they do not contribute to the prediction.

2. **Checked for Missing Values**:
   - Verified that there are no missing values in the dataset.

3. **Data Type Verification**:
   - Ensured all numerical and categorical columns are correctly formatted.

## Exploratory Data Analysis (EDA)
1. **Target Variable Analysis**:
   - Checked the distribution of the `Exited` column (churn rate).
   
2. **Statistical Summary**:
   - Displayed summary statistics for numerical variables.

3. **Visualizations**:
   - **Churn Distribution**: Bar chart to show churn percentage.
   - **Age Distribution**: Histogram or KDE plot.
   - **Correlation Heatmap**: To find relationships between numerical features.
   - **Boxplots**: Identified outliers in numerical columns.
   - **Count Plots**: Checked categorical distributions (e.g., `Geography`, `Gender`).

## Feature Engineering
1. **One-Hot Encoding**:
   - Converted categorical variables (`Geography`, `Gender`) into numerical format.

2. **New Features**:
   - Created `Balance-to-Salary Ratio`,'credit category','longtermcustomer','credit ageratio','productbalanceratio' to assess financial standing.

## Testing and splitting dataset
1.  **Train-Test Split**:
   - here training and testing datsets are evolved using stratified k fold.

2. **Model Selection**:
   - Here we used Random Forest for churn prediction. and used accuracy and other metrics for analysing the performance


3. **VISUALIZATION OF CHURN AND CLUSTERS**:
   - here we used kmeans based on silhoutte score which is ameasure to form clusters for cluster visualization,and heirarchial clustering for reason behind churn...


This README provides a structured approach to analyzing and preparing data for churn prediction. 🚀

