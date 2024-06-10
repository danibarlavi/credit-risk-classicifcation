# Credit Risk Analysis Report
##Overview of the analysis

The purposes of this machine learning model is to quickly analyze a number of financial factors relating to the credit of loan applicants to classify them as either a 'healthy' or 'high risk' loan applicant. The model trains itself on features of historical data of past loan applicants, including the size of the given loan ('loan_size'), the interest rate ('interest_rate'), the borrower's annual income ('borrower_income'), the borrower's debt ('total_debt'), the borrower's ration of debt to income (debt_to_income), the number of bank accounts the borrower posseses ('num_of_accounts'), and the "derogatory marks" on the borrower's file ('derogatory_marks'). It also trains itself on the 'loan_status' labels, a score given to each historical lone classifying them as 'healthy' ('0') or 'high-risk' ('1'). It was this same variable, 'loan_status', that we're trying to predict for future applicants using this model.

In the machine learning process, I went through the following stages:
-- Data collection (reading the csv into a pandas DataFrame)
-- Data Exploration (Reviewing the data)
-- Data preprocessing (splitting data into labels ['y'] and features ['X'])
-- Data splitting (Using **train_test_split** to seperate the dataset into labels and features)
-- Model selection (Importing and instatiating **LogisticRegression** from SKLearn) and training (fitting LogisticRegression to the training data)
-- Prediction (had my model make a prediction on the test set)
-- Model Evaluation (Used a confusion matrix and classification report to evaluate the model)

##Results
- Machine Learning Model
  -- Accuracy: 0.99
  -- Precision: 1.00 for healthy ('0'), 0.85 for 'high-risk' ('1')
  -- Recall: 0.99 for healthy ('0'), 0.91 for 'high-risk' ('1')

##Summary
I would recommend the model for use by a company given the 0.99 overall accuracy score, with a caution that the model more accurately predicts ('0') or 'healthy' loan applicants than ('1') or 'high-risk' applicants. My recommendation for how to improve the model would be encouraging the company to gather more data on 'high-risk' applicants in order to increase the model's precision around such projections. 
