# Module 12 Report Template

## Overview of the Analysis

* **Purpose of the analysis** - The goal of this analysis is to determine if the Logistic Regression machine learning model can more accurately predict healthy loans versus high-risk loans using the original dataset or a dataset that is resampled to increase the size of the minority class.
	- **The Datastet**  - The dataset used to perform the analysis consists of 77,536 loans. The data includes columns for loan_size, interest_rate, borrower_income, debt_to_income ratio, number_of_accounts, derogatory_marks, total_debt, and loan_status. The category that we are attempting to predict with our analysis is **Loan_status**. The data provided in the remaining columns will be used as features to train the data and inform the predictions.

	- **Stages of the Machine Learning Process**  - The stages of the machine learning process are very scripted. If followed in order, they provide you with an accurate assessment of the model's ability to make predictions. The stages of the machine learning process are as follows: 
		- Prepare the data – import the file, establish the DataFrame, evaluate the columns and features.

		- Separate the data into features and labels – The labels are what you are attempting to predict, is the status of the loan, healthy (0) or high–risk (1). The features are all of the remaining data you will use to train and test the model.

		- Use the train_test_split function to separate the features and labels data into training and testing data sets. Import the machine learning model from the library – in this instance, we will be importing LogisticRegression from SKLearn.
		- Instantiate the model.
		- Fit the model using the training data.
		- Use the model to make predictions using the features test data.
		- Evaluate the predictions - Evaluations are done by calculating and comparing metrics like accuracy score, a confusion matrix, and a classification report.
* **Machine Learning Methods Utilized**  - 
The primary model used in this analysis is:
	- LogisticRegression model from SKLearn
	
	Supporting functions used in this analysis are:
	- train_test_split from SKLearn
	
	Models are evaluated using the following functions:
	- confusion_matrix fromSKLearn
	- classification_report from SKLearn
## Results

Using bulleted lists, describe the accuracy scores and the precision and recall scores of all machine learning models.

* Machine Learning Model - Logistic Regression:
    * **Accuracy Score:** 99%
    * **Precision Scores:**
	    * Class 0 (Healthy Loans): 100%
	    * Class 1 (High-risk Loans): 85%
    * **Recall Scores:**
	    * Class 0 (Healthy Loans): 99%
	    * Class 1 (High-risk Loans): 91%

## Summary
The model does a great job at using the original data to predict the values of the healthy loans. Precision was 100% and recall was 99%.

The model is pretty good at predicting the values of high risk loans, but not as good as predicting the healthy loans. Precision was 85% and recall was 91%.
