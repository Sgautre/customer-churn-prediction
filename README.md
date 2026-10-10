# Telecom Customer Churn Prediction

## Project Overview
This machine learning project predicts whether telecom customers
are likely to leave a service using customer account, service,
contract, tenure, and billing information.

## Objectives
- Analyze customer churn patterns using exploratory data analysis.
- Train classification models to predict customer churn.
- Compare models using accuracy, precision, recall, F1-score,
  and ROC-AUC.
- Identify important features related to model predictions.

## Dataset
The project uses the IBM Telco Customer Churn dataset.
It contains 7043 customer records and 21 columns.

The observed churn rate is 26.54%.

## Methodology
1. Load and inspect the dataset.
2. Clean the TotalCharges column.
3. Explore churn distribution, contract type, tenure, and charges.
4. Split the data into training and testing sets.
5. Preprocess numerical and categorical features using a pipeline.
6. Train Logistic Regression, Random Forest, and XGBoost models.
7. Evaluate and compare the models.
8. Examine Random Forest feature importance.

## Model Evaluation
The models were evaluated on the same test set.

                     Accuracy  Precision  Recall  F1-Score  ROC-AUC
Model                                                              
Logistic Regression    0.7381     0.5043  0.7834    0.6136   0.8416
Random Forest          0.7828     0.6189  0.4733    0.5364   0.8232
XGBoost                0.7601     0.5330  0.7781    0.6326   0.8404

Best model by recall: Logistic Regression

Best model by ROC-AUC: Logistic Regression

Best model by accuracy: Random Forest

## Key Findings
The comparison highlights the trade-offs between identifying
customers who churn and making accurate predictions overall.
Feature importance can help identify characteristics useful
for further customer retention analysis.

Refer to the notebook and exported results for detailed findings
and visualizations.

## Technologies Used
- Python
- Pandas and NumPy
- Matplotlib and Seaborn
- Scikit-learn
- XGBoost
- Google Colab

## Limitations
Predictions are not guaranteed to be correct.
Feature importance indicates predictive usefulness, not causation.
The model should be validated on suitable data before deployment.

## Internship Project
Prepared as part of the Customer Churn Prediction project
for the CodeTech internship.
