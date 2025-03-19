Module 20 Report
Overview of the Analysis
This section outlines the analysis conducted for the machine learning models used in this challenge.

Purpose of the Analysis
The goal of this analysis was to evaluate whether the Logistic Regression machine learning model could effectively predict healthy loans (0) versus high-risk loans (1). To improve performance, the original dataset was resampled to increase the size of the minority class (1).

Financial Information in the Dataset
The dataset used for this analysis included information on 77,536 loans, with columns detailing:

Loan size

Interest rate

Borrower income

Debt-to-income ratio

Number of accounts

Derogatory marks

Total debt

Loan status

The target variable for prediction was loan status, with two classes: 0 (healthy loan) and 1 (high-risk loan).

Stages of the Machine Learning Process
The machine learning process followed a structured approach to ensure accurate model evaluation. The key stages were:

Data Preparation: Import the dataset, establish the DataFrame, and evaluate the columns and features.

Feature and Label Separation:

Labels: The target variable (loan status), indicating whether the loan is healthy (0) or high-risk (1).

Features: All other columns used for training and testing the model.

Train-Test Split: Use the train_test_split function to divide the data into training and testing datasets.

Model Selection: Import the LogisticRegression class from the SKLearn library.

Model Instantiation: Create an instance of the logistic regression model.

Model Training: Fit the model to the training data.

Predictions: Use the trained model to make predictions on the testing dataset.

Evaluation: Assess the model's performance using metrics such as accuracy score, confusion matrix, and classification report.

Machine Learning Methods Utilized
The following methods from SKLearn were employed:

LogisticRegression

train_test_split

confusion_matrix

classification_report

Results
Below are the key performance metrics for the Logistic Regression model:

Accuracy Score: 99%

Precision:

Class 0 (Healthy Loans): 100%

Class 1 (High-Risk Loans): 84%

Recall:

Class 0 (Healthy Loans): 99%

Class 1 (High-Risk Loans): 94%

Summary
The Logistic Regression model excels at predicting healthy loans (0), achieving a precision of 100% and a recall of 99%, indicating nearly perfect performance.

For high-risk loans (1), the model performs reasonably well, with a precision of 84% and a recall of 94%. This suggests that the model identifies most high-risk loans accurately, though there is room for improvement in reducing false positives.

Overall, the Logistic Regression model effectively predicts both healthy and high-risk loans, leveraging the features provided during training.