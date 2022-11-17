# MiniProject2_BAN5753
Mini Project 2 - BAN 5743 - Go Pokes

## Problem Statement
The problem which we worked upon is a Deposit opening classification problem.The objective of the classification is to identify clients who will 
subscribe (yes/no) for a term deposit. (Variable y: Target function). The Bank wants us to conduct Exploratory Data Analysis (EDA) to 
identify relationships, trends in data. For example: correlations, bivariate analysis of target versus input variables, facts, univariate 
patterns and missing data.

## Dataset information:
1. Data is about an XYZ bank’s direct marketing campaign. Marketing 
campaigns were driven by telephone calls.
2. Data Set In many cases, more than one contact for the same client 
was required., in order to access if the product (deposit) would be 
('yes') or not ('no') subscribed
3. The purpose of the classification is to forecast whether the customer 
will signup (yes/no) a term deposit (variable y).
4. The dataset: XYZ_Bank_Deposit_Data_Classification.csv, 20 
entries/columns, sorted by date between May 2008 and November 
2010.

## Attributes Information 
1. # Attributes information:
- Age (Numeric)
- Job: type of job (categorical)
- Marital: marital status (categorical)
- Education (categorical)
- Default: has credit in default? (categorical)
- Housing: has housing loan? (categorical)
- Loan: has personal loan? (categorical)
2. #regarding the latest contact in the ongoing campaign:#
- Contact: contact communication type (categorical)
- Month: last contact month of year (categorical)
- Day_of_week: last contact day of the week (categorical)
- Duration: last contact duration, in seconds (numeric)
3. #other attributes:#
- Campaign: number of contacts performed during this campaign and for this 
client (numeric, includes last contact)
- Pdays: number of days that passed by after the client was last contacted from a 
previous campaign (numeric; 999 means client was not previously contacted)
- Previous: number of contacts performed before this campaign and for this client 
(numeric)
- Poutcome: outcome of the previous marketing campaign (categorical)
4. #social and economic context attributes:#
- Emp.var.rate: employment variation rate - quarterly indicator (numeric)
- Cons.price.idx: consumer price index - monthly indicator (numeric) 
- Cons.conf.idx: consumer confidence index - monthly indicator (numeric) 
- Euribor3m: euribor 3 month rate - daily indicator (numeric)
- Nr.employed: number of employees - quarterly indicator (numeric)

## Project Summary -
We started with performing an exploratory data analysis and concluded that there are no missing values in the data. This was followed with a Univariate analysis where we wanted to look at the distribution of every single feature. We then followed this with a bivariate analysis to understand hwo every feature is related with the Target variable. This was followed up with a Correlation Analysis and we found out that there was a high correlation between Euribor3m and nr_employed. Also there seems to be high correlation between nr_employed and emp_var_rate. We decided to removed Euribor3m and nr_employed before we move further with the modeling exercise. 
We worked on 4 classification algorithms - Decision Trees, Random Forest, Logistic Regression and Gradient Boost. We used AUC ROC Score to evaluate the models. Of the 4 models, Gradient boost came out as the champion model with an AUC ROC score of 0.944. We further performed a K-Means CLustering, to identify the most optimum number of clusters in the data based on a metric called "Silhouette Score". We found 3 to be the most optimum number of Clusters. 

For a detailed overview of the project and the findings please refer to the following : 
