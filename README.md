# credit-risk-classification
Module 20 Challenge

# Overview of the Analysis
In this challenge, I used various techniques to train and evaluate a model based on loan risk using machine learning processes.  More specifically, the model's objective was to predict whether a given loan was healthy, would be paid back in full, or high risk, would not be paid back in full.  The data included information about borrowers as well as loan size, income, interest rate, debt, etc..  The target variable was loan_status, where "0" indicates a healthy loan, and "1" indicates a loan that was high-risk.  

At first, the data was prepared where it was read into a data frame splitting out the features from labels.  Next, the data was split into training and testing sets using "train_test_split".  Next came the creation of a logistic regression model, training that model with the training data and using that to predict the 'value_counts'/loan statuses in the testing set.

# Results
Machine Learning Model 1: Logistic Regression (scale of 0 to 1)
- Accuracy Score: 0.99
- Precision Score:
    - Precision measures how often a model is correct when predicting positives.
    - A high precision score here means that the model is most likely correct at predictions.
    - Class 0 (Healthy): 0.99
    - Class 1 (High-risk): 0.91
- Recall Score:
    - Recall measures the ability of the model to correctly identify all objects of the target class.
    - A high recall score means that the model is good at identifying most of the loans that will not be fully paid. 
    - Class 0 (Healthy): 1.00
    - Class 1 (High-risk): 0.85

# Summary
The logistic regression model created here performed rather well.  This is shown through an overall accuracy score of 99%. The model was very good at predicting healthy loans with precision and recall scores at 0.99 and 1.0, respectively. The model was less effective at predicting high-risk loans, shown through a recall score of 0.85.

The strong perfmorance of this model allows me to be able to recommend the use of it, though it may depend on the end use.  It works great for predicting whether a loan will be paid off but less so on loans that will not.  If the goal of the model is to strictly predict healthy loans, this will be highly recommended.  If the goal is to prioritize only the identification of high-risk loans, more work may need to be done to the model/processes.

