# Loan-Prediction
<p align="center">
  <img src="https://github.com/nguneonard/Loan-Prediction/blob/main/loan.png"  title="hover text">
</p>



## Project Objective
Dream Housing Finance company deals in all home loans. They have presence across all urban, semi urban and rural areas. Customer first apply for home loan after that company validates the customer eligibility for loan. Company wants to automate the loan eligibility process (real time) based on customer detail provided while filling online application form. These details are Gender, Marital Status, Education, Number of Dependents, Income, Loan Amount, Credit History and others. To automate this process, they have given a problem to identify the customers segments, those are eligible for loan amount so that they can specifically target these customers.
This is a classification problem where we have to predict whether a loan would be approved or not.

## Project Description
Loan prediction is a very common real-life problem that each retail bank faces atleast once in its lifetime. If done correctly, it can save a lot of man hours at the end of a retail bank.
In the course of this project, we had to start by examing the some of the features on the test and train datasets(number of rows and columns, nature of the features), then walked through exploratory data to look at some hidden patterns and trends of the predictors with respect to the outcome variable. Data cleaning and Engineering were performed, then feeding into the appropriate machine learning algorithms where the best one was logistics regression giving an accuracy of 83%
The data for this project is available at:
- train file: https://datahack.analyticsvidhya.com/contest/wns-analytics-hackathon-2018-1/download/train-file
- test file: https://datahack.analyticsvidhya.com/contest/wns-analytics-hackathon-2018-1/download/test-file
- sample submission file:  https://datahack.analyticsvidhya.com/contest/wns-analytics-hackathon-2018-1/download/sample-submission

## Dataset Description
The train and test dataset  have the same columns except for the target column that is “Loan Status”.

| Variable     | Description |
| -----------  | ---: |
|Loan_ID|	Unique Loan ID|
|Gender|	Male/ Female|
|Married|	Applicant married (Y/N)|
|Dependents|	Number of dependents|
|Education|	Applicant Education (Graduate/Under Graduate)|
|Self_Employed|	Self employed (Y/N)|
|ApplicantIncome|	Applicant income|
|CoapplicantIncome|	Coapplicant income|
|LoanAmount|	Loan amount in thousands|
|Loan_Amount_Term|	Term of loan in months|
|Credit_History|	Credit history meets guidelines|
|Property_Area|	Urban/ Semi Urban/ Rural|
|Loan_Status|	Loan approved (Y/N)|

## What is hypothesis generation?

This is a very importanbt stage in any data science or machine learning pipeline. it involves understanding the problem in detail by brainstorming as many factors as possible which can impact the outcome. it is done by understanding the problem statement thoroughly and before looking at the data.
 
Below are some of the factors which i think can affect Loan approval(dependent variable for this loan prediction problem).
- salary: Apllicants with high income should have more chances of loan approval
- previous history: Applicants who have repayed their previous debt should have high er chances of loan approval
- Loan Amount: Loan approval should also depend on loan amount. if the loan amount is low, the chances of loan approval should be high
- Load terms: loan for less time period and less amount should should have higher chances of approval.
- EMI: lesser the amount to be paid monthly to repay the loan, higher the chances of loan approval

The answers to these questions were verified by performing exploratory data analysis on the dataset notably: univariate and bivariate analysis in order
to view some hidden inside of the data.Then we proceed unto data preprocessing where missing data and outlier analysis was performed. Going through the notebook, we will realise that the train and test dataset were concatenated before performing the appropriate cleaning so as to avoid the redundant work of cleaning train and test dataset separately.Since machine learning algorithms work only with numbers after the cleaning the process, i performed one-hot encoding to convert the rest of the categorical variables to numerical variables and subsequent dropping of irrelevant features. This was followed by applying various regression models using scikit learn andcomparing the accuracy of each. The best model was then tuned using grid_search and finally applied in the test dataset.

## Methods Used
- Machine Learning
- Data Visualization
- Predictive Modeling
- feature engineering
- Inferential Statistics

## Technologies used
- seaborn
- matplotlib
- numpy
- scikit learn
- pandas

## Needs of this project
- financial analysis
- data exploration/descriptive statistics
- data processing/cleaning
- feature engineering
- statistical modeling

## Contributing DSWG Members

**Team Leads (Contacts) : [Kubin Ngu Neonard](https://github.com/nguneonard)**
