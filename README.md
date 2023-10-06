# credit-risk-classification
Data Science Bootcamp - Module 20 Challenge

The machine learning models found in "credit_risk_classification.ipynb" aims to predict if a loan is High-Risk or not based on the following:
* loan_size
* interest_rate
* borrower_income
* debt_to_income
* num_of_accounts
* derogatory_marks
* total_debt
* loan_status

In total the data has 75036 Healthy Loans, and 2500 High-Risk Loans.
 This data was split into training and testing sets.
 One model was trained with the orignal split training data, and another was trained with resampled data with the RandomOverSampler function.
 Both models were LogisticRegression models from sklearn

## Results
* Logistic Regression Model 1:
  * Accuracy: .99
  * Precision: 1.00 for Healthy Loans, .85 for High-Risk Loans
  * Recall score: .99 for Healthy Loans, .91 for High-Risk Loans



* Logistic Regression Model 2 (resampled data):
  * Accuracy: .99
  * Precision: 1.00 for Healthy Loans, .84 for High-Risk Loans
  * Recall score: .99 for Healthy Loans, .99 for High-Risk Loans

## Summary
Both Models have a balanced accuracy of 99%. But I would recommend Model 2. The Higher Recall score for the High-Risk Loans means that 99% of the Loans that were High-Risk, were correctly predicted. From a
banks perspectave the Recall Score would be more important than the Percision for the High-Risk Loans. In this case a higher percision would be the number of Loans Predicted to be
High Risk that were. The bank is more concerned with minimizing risk, so a higher Recall Score is very important.