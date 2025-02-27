# Default of Credit clients
## Introduction
In this project, we predict customer defaults for a credit card payment using a dataset having customers’ financial and demographical details. The objective is to find out the patterns and trends that have an impact on default behavior, engineer meaningful features so as to build machine learning models based on them to make accurate predictions. A structured process was followed—data preprocessing, exploratory data analysis (EDA), feature engineering, model building and evaluation. Key insights from the analysis include the impact of credit utilization and payment history on defaults, and how Random Forest, Gradient Boosting, and Logistic regression models performed compared to each other to recommend which model would be best to deploy.

## Problem Statement
The problem we are addressing here is the prediction of customer defaults on credit card payments for the following month. The goal here is to identify customers as high likelihood or low likelihood to default, given their financial behavior and demographic information. This prediction is essential to minimise the credit risk for financial institutions, optimise their allocations for collecting customers, and provide targeted interventions to the at-risk customers. Utilizing the record of historical data for such indicators as payment history, billing amount and demographic parameters, the objective is to develop an accurate predictive model that can prevent the losses; simultaneously enhancing the decision making process of customers in this domain.
## EDA
### Univariate Analysis
![image](https://github.com/user-attachments/assets/02726291-6bf1-41b4-9ffd-3adb86119ab8)
![image](https://github.com/user-attachments/assets/2e9917eb-054a-4e78-a989-9daa4557a6c2)
![image](https://github.com/user-attachments/assets/79561d8e-c1e2-4381-8184-cd0beee67cec)

###  Bivariate Analysis
![image](https://github.com/user-attachments/assets/4bfd6e85-ee50-4f76-89d3-93dd4bd93e8a)
![image](https://github.com/user-attachments/assets/51577daa-3da7-4135-9704-b17e5c327485)

## Key Insights from the Data
### Customer Demographics and Default Patterns:

 * Younger customers (e.g., those in their 20s and 30s) tend to have higher default rates, possibly due to limited financial experience or stability.

 * Marital status shows a significant relationship with default rates, with married individuals appearing to manage credit better compared to single or divorced clients.

### Behavioral and Financial Indicators:

* High Payment_Ratio (ratio of payments to credit limit) and consistent on-time payments are strong indicators of lower default risk.
Customers with higher Credit_Utilization ratios (closer to their credit limit) are more likely to default, highlighting the importance of credit management.


## Model Insights
* Logistic Regression provides baseline performance but struggles with complex relationships due to its linear nature.
* Random Forest captures non-linear patterns effectively, improving recall but sometimes overfitting on training data.
* Gradient Boosting achieves the best balance between precision and recall, with a consistently high AUC-ROC score, making it the most reliable model for predicting defaults.

## Recommendations
* Risk Segmentation: Use the model to segment customers into risk tiers based on critical features like payment history, Credit_Utilization, and Payment_Ratio, enabling targeted interventions for high-risk groups.
* Enhance Predictive Modeling: Deploy Gradient Boosting for real-time default predictions while regularly retraining the model with updated data to maintain accuracy and adapt to changing customer behavior.
* Integrate Insights into Business Strategy: Utilize predictions to guide credit approvals, adjust credit limits, and prioritize collections strategies for customers predicted to default.
