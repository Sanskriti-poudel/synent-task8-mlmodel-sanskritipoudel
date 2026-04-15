Loan Prediction Dataset – Machine Learning Model
Problem Statement:

The objective of this task is to build a machine learning model to predict loan amount based on applicant details. The goal is to analyze customer data and develop models that can accurately estimate loan values using different regression algorithms.

Dataset Details:

The dataset contains information about loan applicants and their financial background.They are:

Loan_ID ,
Gender ,
Married ,
Dependents ,
Education ,
Self_Employed ,
ApplicantIncome ,
CoapplicantIncome ,
LoanAmount ,
Loan_Amount_Term ,
Credit_History ,
Property_Area 

Approach:

1. Data Loading & Exploration:
Imported required libraries: pandas, numpy, matplotlib, sklearn
Loaded dataset using read_csv()
Performed:
Shape analysis
Data type inspection (info())
Summary statistics
Missing value detection

2. Data Preprocessing:
Handling Missing Values
Filled categorical missing values using mode ,
Filled numerical missing values using mean
Encoding
Used LabelEncoder to convert categorical variables into numeric form

3. Feature Selection:
Selected input features (X) by dropping target variable
Target variable (y) = LoanAmount

4. Train-Test Split
Split dataset into:
80% training data ,
20% testing data ,
Used random_state=42 for reproducibility

5. Model Training:

Three regression models were applied:

a.Linear Regression
b.Decision Tree Regressor
c.Random Forest Regressor

6. Model Evaluation
Used RMSE (Root Mean Squared Error) to evaluate performance. Lower RMSE indicates better model performance

Results:

Linear Regression provides a baseline performance

Decision Tree captures patterns but may overfit

Random Forest generally gives better accuracy due to ensemble learning

RMSE comparison helps select the best model
