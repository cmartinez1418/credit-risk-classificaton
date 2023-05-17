# credit-risk-classificaton

The purpose of this analysis was determine loan riskiness. The CSV contained information on the loan amount, interest rate, borrower's income, debt to income ration, number of accounts, derogatory marks, total debt, and loan status. The loan status had values of "0" or "1", with "0" meaning the loan was healthy and "1" meaning the loan had a high risk of defaulting. The loan status was used to train the model. After loading in the CSV with the data, the model was trained by separating the loan status column from the rest of the data frame. The data was then split into training and testing sets and LogisticRegression was used to fit the model. The RandomOverSampler module was also used to resample the data in a second run.

Machine Learning Model 1: LogisticRegression
•	Accuracy: 94.42%
•	Precision: 1.00 for “0”, 0.87 for “1”
•	Recall: 1.00 for “0”, 0.89 for “1”

Machine Learning Model 2: RandomOverSampler and LogisticRegression
•	Accuracy: 99.60%
•	Precision: 1.00 for “0”, 0.87 for “1”
•	Recall: 1.00 for “0”, 1.00 for “1” 

While both models worked very well, Machine Learning Model 2 seemed to work better than Machine Learning Model 1. It had equal or higher accuracy, recall, and F-1 scores for both healthy and high risk loans. In this situation, it is more important to predict the number of high risk loans, as they are more rare than healthy loans. 
