# Module 20 (Credit Risk Analysis)

## **Overview**
This project focuses on utilizing a Logisitic Regression model to predict healthy loans(0) versus high-risk loans (1) using both the original dataset and a resampled dataset designed to balance the minority class. This helps financial institutions reduce default rates, make informed lending decisions and ensure financial stability. 

* **The Dataset** - The dataset used for this analysis consists information on 77,536 loans. The data includes columns for loan_size, interest_rate, borrower_income, debt_to_income ratio, number_of_accounts, derogatory_marks, total_debt, and loan_status. The category that we are attempting to predict with our analysis is **loan_status**. The data provided in the remaining columns will be used as features to train the data and inform the predictions. 

* **Stages of the Machine Learning Process** - The stages of the machine learning process are very scripted. If followed in order, they provide you with an accurate assessment of the model's ability to make predictions. The stages of the machine learning process are as follows: 
1. Prepare the data that includes fiancial features related to borrower income, debt, and credit history.  
2. Separate the dataset into features and target labels (loan_status)
3. Split the dataset into training and testing sets. 
4. Train a Logisitic Regression model using the scikit-learn library
5. Evaluate the model's predictions using accuracy, precision, recall, and a confusion matrix.

## **Technologies Used**
- Python 
- Google Colab
- Pandas
- scikit-learn 
    - LogisticRegression
    - train_test_split
    - confusion_matrix
    - classification_report

credit-risk-classification/
│   lending_data.csv        # financial loan data and loan_status market dataset
│   credit_risk_classification.ipynb       # Colab Notebook with code implentation
│   report-template.md     #Project overview
│   README.md           # Project documentation (this file)

## **Setup Instructions**
1. **Clone the Repository:**
Clone the GitHub repository and navigate into the project directory

2. **Install the Dependencies:**
Pandas and scikit-learn are installed 

3. **Load and Explore the Data :**
Load the lending_data.csv into a Pandas DataFrame to display loan statistics and visualize trends.

4. **Prepare the Data:** 
Define the features (X) and target (y). Split the data using train_test_split

5. **Train the Model:**
Import and fit the LogisticRegression model with the training data

6. **Make Predictions:**
Predict loan risk using the test dataset

7. **Evaluate the Model:**
- Calculate the accuracy score and generate the confusion matrix
- Print the classification report

## **Results**
Machine Learning Model - Logistic Regression
* **Accuracy Score:** 99%
	* **Precision Scores:** 
		* Class 0 (Healthy Loans): 100%
		* Class 1 (High-risk Loans): 84%
	* **Recall Scores:** 
		* Class 0 (Healthy Loans): 99%
		* Class 1 (High-risk Loans): 94%
		
    * Description of Model 1 Accuracy, Precision, and Recall scores.

## Summary
The **Logistic Regression model** achieved **99% accuracy**, making it highly reliable for credit risk prediction. It correctly identified most high-risk loans with 94% recall and predicted healthy loans.

Given its performance, this model is recommended for production use in credit risk assessment. Continuous retraining is advised as new loan data becomes available to maintain prediction accuracy.

