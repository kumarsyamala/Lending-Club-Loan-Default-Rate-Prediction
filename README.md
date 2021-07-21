# Lending-Club-Loan-Default-Rate-Prediction

Project Details

OVERVIEW 
Due to the current scenario of Covid-19 lots of people lost their jobs and unemployment rate has increased rapidly. Due to the Banks may face huge from personal and corporate customers (Companies may default 2.54 Lakhs Cr bank loan in next 3 years)
U.S. banks have had to prepare for the likelihood of elevated borrower defaults and have more than doubled their allowances for loan losses. This, on the back of about $115 billion of provisions in the first half of 2020, represented major progress toward absorbing the loan losses likely to result from the economic downturn.
So many Banks are in financial losses. To decreases the losses for bank in the future, Banks has to give money to the customer who are going to pay the amount which they lend. For that the prediction that we are going to do helps Banks to Identify the customers who are not going to pay or not able to pay the loan amount, so that they can avoid those customers for Financial Losses.

The “Lending Club" is a "peer to peer" lending company that provides various loans for individuals looking to finance personal loans, business loans, auto refinancing loans and medical loans. The loan data for this project was obtained through Kaggle and consists of loans issued from 2007 - 2015. Solving this case study will give us an idea about how real business problems are solved using EDA and Machine Learning. In this case study, we will also develop a basic understanding of risk analytics in banking and financial services and understand how data is used to minimise the risk of losing money while lending to customers.
We took a Sample data of 5 Months in 2015 1,51,618 records and 74 columns. Through this Data I am going to use the EDA and Machine Learning techniques to predict the real business problem of Risk Analysis.
 
 ![image](https://user-images.githubusercontent.com/82040540/126468264-54da86d1-ab45-4b90-ad86-05d4a103fb0a.png)

 
Business Problem Statement (GOALS)
1.	Understanding the Business Problem 
Lending Club is an American peer-to-peer lending company, headquartered in San Francisco, California. It is the first peer-to-peer lender to register its offerings as securities with the Securities and Exchange Commission, and to offer loan trading on a secondary market. When the company receives a Loan application, the company has to make a decision on the application profiles. 
Two types of risks are associated with the bank’s decision:
•	If the applicant is likely to repay the loan, then not approving the loan results in a loss of business to the company
•	If the applicant is not likely to repay the loan, i.e., he/she is likely to default, then approving the loan may lead to a financial loss for the company
The data given contains the information about past loan applicants, credit card history and score and their demographics to determine whether they ‘defaulted’ or not. The aim is to identify patterns which indicate if a person is likely to default, which may be used for taking actions such as denying the loan, reducing the amount of loan, lending (to risky applicants) at a higher interest rate, etc.
When a person applies for a loan, there are two types of decisions that could be taken by the company:
1.	Loan accepted
2.	Loan rejected

2.	Business Objective

LC is the Largest Online Loan Marketplace which lends the loans to personal, business and medical loans to customers for lowest interest rates easily. In this process of Lending Loans to applicants is ‘Risky’, because if the customer refuses to pay or run away with money that he/she owed will leads to the Financial Loss to the company. 

So, if the company able to identify Who are the customers are ‘Risky’  applicants to lend the money would be helpful to avoid the Financial Loss.

By this Analysis company will understand What variables that drive the Customers towards ‘Default’ to those customers the company will Reject the loan or wouldn’t accept the application.

3.	Approach

Data Cleaning & Exploratory Data Analysis: -

In this project the Data set that I am using is rich data but I have to deal with some Null values and some unwanted variables.

In EDA we need to see the distribution of variables and correlation with Target variable. To find out these I need to use some visualization tools and to select the Important Variables.
 
Predict the Charged off Rate: - 

With the selection of few Important Variables, I will use those to build the Model. I will use some Classification algorithm in the way to predict the charged off rate.

Model Comparison and Evaluation: -

By Few Classification Algorithm I am expected to obtain the predicted values, by using the Model Evaluation Metrics of Different models in classification and compare the results.

From these will select the Best Model.

4.	Conclusions: -

Based on the Best model Company able to Identify the Which applicant that applied for the Loan could be ‘Charged off’.

TOPIC SURVEY IN BRIEF 

From this dataset we will develop a basic understanding of risk analytics in banking and financial services and understand how data is used to minimise the risk of losing money while lending to customers. As we got the data from Kaggle we analysed the data and we choose some important features to predict which customers are going to be charged off and fully paid. By the inference from the current solution to the problem we can give analysis to the Lending Club that to identify the customers who are not going to pay the lending amount so that they can avoid these kinds of applicants and can avoid the financial loss. 

CRITICAL ASSESSMENT OF TOPIC SURVEY 
Find the key area, gaps identified in the topic survey where the project can add value to the customers and business
1.	Handling the null values and missing values in the dataset
2.	Removing unnecessary columns
3.	Handling the imbalanced dataset

What key gaps are you trying to solve?
       1. 	We will drop the null values and replace the missing values from the dataset 
       2. 	Selecting important features for model building
       3. 	Balancing the dataset


METHODOLOGY TO BE FOLLOWED (Explain each step from 1-5)
I.	UNDERSTANDING THE BUSINESS: 

II.	The customers of the Lending club are unable to repay the loans which they have taken from the company and they would like to know what actions to take and how to avoid this kind of customers.
III.	The goal here is that the Lending club has to know before giving the loan to any customer that whether the customer will be able to repay the loan so that they can avoid loses to the company. 
IV.	Here, we use a dataset which contains more than 151618 observations. We will choose the best classification model based on different metrics. 
V.	In simple words, we aim to build a predictive model using Lending Club dataset to predict if the customers will be able to repay the loan or not.

VI.	UNDERSTANDING THE DATA: 

DATASET SOURCE – The publicly available data set used in this project came from Kaggle’s Lending Club Data. We have one Excel file: Lending Club Data. The dataset consists of 74 features and above 8 lakhs records.
We took a sample data from this we selected data for 5 Months from January to May 2015. 
DATASET NAME - Lending Club Data
DATA DESCRIPTION – Lending Club Data - the overall dataset - contains client information about the loan application details from 2007 to 2015.
Each row in the dataset refers to one client’s information about the loan application details. In the 74 columns of the data, we only choose the important columns for to build a model. The dataset consists of   numerical and categorical attributes. 
Numerical Features in the Dataset:

Variable	Description
loan_amnt --	The listed amount of the loan applied for by the borrower. If at some point in time, the credit department reduces the loan amount, then it will be reflected in this value.
funded_amnt	-- The total amount committed to that loan at that point in time.
funded_amnt_inv --	The total amount committed by investors for that loan at that point in time.
int_rate	 -- Interest Rate on the loan
installment	-- The monthly payment owed by the borrower if the loan originates.
annual_inc --	The self-reported annual income provided by the borrower during registration.
dti	-- A ratio calculated using the borrower’s total monthly debt payments on the total debt obligations, excluding mortgage and the requested LC loan, divided by the borrower’s self-reported monthly income.
delinq_2yrs	-- The number of 30+ days past-due incidences of delinquency in the borrower's credit file for the past 2 years
inq_last_6mths ---	The number of inquiries in past 6 months (excluding auto and mortgage inquiries)
open_acc	-- The number of open credit lines in the borrower's credit file.
pub_rec -- 	Number of derogatory public records
revol_bal	-- Total credit revolving balance
revol_util --	Revolving line utilization rate, or the amount of credit the borrower is using relative to all available revolving credit.
total_acc	-- The total number of credit lines currently in the borrower's credit file
total_rec_int	-- Interest received to date
collections_12_mths_ex_med	-- Number of collections in 12 months excluding medical collections
acc_now_delinq	-- The number of accounts on which the borrower is now delinquent.
tot_coll_amt	-- Total collection amounts ever owed
tot_cur_bal	-- Total current balance of all accounts
total_rev_hi_lim	

Categorical Features in the Dataset:
Variable	Description
term	-- The number of payments on the loan. Values are in months and can be either 36 or 60.
emp_length	-- Employment length in years. Possible values are between 0 and 10 where 0 means less than one year and 10 means ten or more years.
home_ownership	-- The home ownership status provided by the borrower during registration or obtained from the credit report. Our values are: RENT, OWN, MORTGAGE, OTHER
verification_status	-- Indicates if income was verified by LC, not verified, or if the income source was verified
loan_status	-- Current status of the loan
purpose	-- A category provided by the borrower for the loan request.
addr_state	-- The state provided by the borrower in the loan application
initial_list_status -- 	The initial listing status of the loan. Possible values are – W, F
application_type	-- Indicates whether the loan is an individual application or a joint application with two co-borrowers

VII.	DATA PREPARATION: -
We plan to approach the problem using below mentioned steps:
STAGE 1: TO PERFORM EXPLORATORY DATA ANALYSIS
1. Importing necessary libraries and reading the dataset
2. Study the nature of variables at hand - Understand the type of distribution the variable belongs to.
3. Check for Missing values/ NULL Values, Outliers: If Missing/NULL values or Outliers are found, they will be removed or imputed depending after observing the feature data.
4.Separate the independent and dependent variables.
5.Perform Exploratory Data Analysis. Study the relationship between variables. Note down the important patterns found for further analysis. We will use matplotlib, seaborn and Plot for data visualization.
6.Study the correlation between variables. (using Pearson's R/Chi Square Test etc. as applicable).

7.Check for Multicollinearity between independent variables.
STAGE 2: FEATURE ENGINEERING
1.Few variables may not be in the form that we expect. Those variables will be transformed using various techniques.
2.Non-numerical categorical variables will be transformed using One Hot Encoding or Label Encoding as appropriate
3.Split the dataset into two parts: Training dataset and testing dataset
4.Perform Feature Selection:
   A. We will use an ensemble of Feature selection techniques like:

•	Pearson's R

•	Chi Square

•	RFE

•	Decision Trees, Random Forest
5.Perform Feature Scaling and Dimensionality Reduction
a.	Dimensionality Reduction may be applied if strong multicollinearity is observed.
b.	Dimensionality Reduction Techniques (depending on the data) to be used are:
c.	Principal Component Analysis
IV.	MODELING:
1.Feed Training Data into the Model. Below mentioned algorithms will be used as appropriate:
                A. KNN Regressor
                B. Decision Tree- R, Random Forest
2.Ensemble Algorithms below mentioned will be utilized to optimize
                 A. Random Forest
                 B. AdaBoost
                  C. Gradient Boost
                  D. XGBoost
                  E. Voting Classifier
                  F. Stacking Techniques
3.Tuning of hyperparameters and selecting best parameters for the model
V. EVALUATION:
1.Model Validation will be performed using metrics like:
       A. Percision
       B. Recall
       C. AUC ROC
       D. F1 Score
       E. Bias Error
       F. Variance error
2. All Models will be validated using Cross-Validation techniques to identify Underfitting/ Overfitting issues
3. Performance of all models will be compared against testing and validation sets and the best model will be chosen for this dataset for final prediction.
Reference documents of CRISP-DM
http://rstudio-pubs-static.s3.amazonaws.com/290261_676d9bb194ae4c9882f599e7c0a808f2.html
https://www.openintro.org/data/index.php?data=loans_full_schema
https://www.kaggle.com/search?q=lending+club+loan


Original owner of data	                  Alex Husted
Data set information	This data set represents thousands of loans made through the Lending Club platform, which is a platform that allows individuals to lend to other individuals
Link to web page	https://www.kaggle.com/faressayah/lending-club-loan-defaulters-prediction/data?select=loan.csv

	

                                                            ***********************************************************
