
# Lending Data Analysis with Logistic Regression

## Overview of the Analysis

The purpose of this analysis was to develop and evaluate a machine learning model to predict the status of loans based on borrower-related financial information. The dataset used for this analysis includes features such as loan size, interest rate, borrower income, debt-to-income ratio, number of accounts, derogatory marks, and total debt. The primary goal was to predict whether a loan would be classified as "healthy" (low-risk) or "high-risk" based on these features.

The variable of interest, `loan_status`, was binary, with values of `0` for healthy loans and `1` for high-risk loans. The machine learning process involved several key stages:

1. **Data Preparation**: The data was split into features (`X`) and labels (`y`), with `loan_status` serving as the target variable.
2. **Data Splitting**: The dataset was divided into training and testing sets using a 75-25 split, ensuring that the class distribution was maintained via stratification.
3. **Model Selection**: A logistic regression model was chosen for its simplicity and effectiveness in binary classification tasks.
4. **Model Training**: The logistic regression model was trained on the training set.
5. **Model Evaluation**: The model’s performance was evaluated using the testing set, with metrics such as accuracy, precision, and recall being calculated.

## Results

* **Logistic Regression Model**:
    * **Accuracy**: 99%
    * **Precision**:
      * Class 0 (Healthy Loan): 1.00
      * Class 1 (High-Risk Loan): 0.87
    * **Recall**:
      * Class 0 (Healthy Loan): 1.00
      * Class 1 (High-Risk Loan): 0.89

## Summary

The logistic regression model demonstrated exceptional performance in predicting loan status, particularly for healthy loans (Class 0), where it achieved perfect precision and recall scores. This indicates that the model is highly reliable in correctly identifying healthy loans without misclassifying them as high-risk. 

For high-risk loans (Class 1), the model’s performance, while not perfect, was still strong, with a precision score of 0.87 and a recall score of 0.89. This means that the model is fairly effective at identifying high-risk loans, although there is a small margin for improvement in reducing false positives.

### Recommendation

Based on the results, I recommend using the logistic regression model for loan status prediction. The model's high accuracy and strong performance, especially in classifying healthy loans, make it a valuable tool for minimizing financial risk. While the model is effective overall, further refinement could enhance its ability to identify high-risk loans more accurately, which is crucial depending on the company's risk management priorities. If the primary goal is to avoid high-risk loans, additional models or techniques may be considered to complement this logistic regression model.

