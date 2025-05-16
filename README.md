
# Module 12 Report

## Overview of the Analysis

The purpose of this analysis was to build and evaluate machine learning models to predict the credit risk of loans using financial information about the borrowers. The target variable, `loan_status`, indicates whether a loan is considered healthy (0) or high-risk (1). This type of prediction is important for financial institutions to minimize potential losses and make informed lending decisions.

The distribution of values is:
- 0: 75036
- 1: 2500

The dataset included variables such as:
- `loan_size`
- `interest_rate`
- `borrower_income`
- `debt_to_income`
- `num_of_accounts`
- `derogatory_marks`
- `total_debt`

The machine learning process followed these main stages:
1. Data preprocessing and splitting into features (`X`) and target (`y`)
2. Train-test splitting using `train_test_split`
3. Standardizing features using `StandardScaler` 
4. Training models: `LogisticRegression`
5. Evaluating model performance using accuracy, precision, and recall

## Results

- **Machine Learning Model: Logistic Regression**
  - **Accuracy:** 99%
  - **Label 0 (healthy loans):**
    - Precision: 1.00
    - Recall: 0.99
    - F1-score: 1.00
  - **Label 1 (high-risk loans):**
    - Precision: 0.84
    - Recall: 0.98
    - F1-score: 0.91



## Summary

The Logistic Regression model performed very well overall, especially for identifying healthy loans. It also did a strong job identifying high-risk loans, with a high recall of 98%, although precision for label 1 was slightly lower (84%). This means the model is cautious — it prefers to flag a loan as high-risk even if it results in some false positives.

Given the strong performance and simplicity of Logistic Regression — and its high recall on high-risk loans — it is a recommended model for credit risk prediction in this case.
