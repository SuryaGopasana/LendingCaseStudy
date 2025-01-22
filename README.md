# Project Name
> EDA Lending Club Case Study

## Table of Contents
* [Problem Statement](#Problem-Statement)
* [Data Understanding](#data-understandin)
* [Data Cleaning](#data-cleaning)
* [Analysis](#analysis)
* [Conclusions](#conclusions)

<!-- You can include any other section that is pertinent to your problem -->

## Problem Statement
- You work for a consumer finance company which specializes in lending various types of loans to urban customers. When the company
  receives a loan application, the company has to make a decision for loan approval based on the applicant’s profile. Two types of risks are
  associated with the bank’s decision:
  - If the applicant is likely to repay the loan, then not approving the loan results in a loss of business to the company
  - If the applicant is not likely to repay the loan, i.e. he/she is likely to default, then approving the loan may lead to a financial loss for the
  company
- Like most other lending companies, lending loans to ‘risky’ applicants is the largest source of financial loss (called credit loss). Credit loss is
the amount of money lost by the lender when the borrower refuses to pay or runs away with the money owed. In other words, borrowers
who default cause the largest amount of loss to the lenders. In this case, the customers labelled as 'charged-off' are the 'defaulters’.
The core objective of the exercise is to help the company minimize the credit loss

## Data Understanding
- loan.csv contains the complete loan data for all loans issued through the time period 2007 t0 2011
- It contains 39717 rows and 111 columns
- There are 2 types of attributes: Loan Attributes and Customer Attributes
- Leading Attribute
- Loan Status - Key Leading Attribute (loan_status). The column has three distinct values
  - Fully-Paid - The customer has successfully paid the loan
  - Charged-Off - The customer is "Charged-Off" ir has "Defaulted“
  - Current - These customers, the loan is currently in progress and cannot contribute to conclusive evidence if the
  customer will default of pay in future
- For the given case study, "Current" status rows will be ignored

- ## Data Cleaning
- No header, footers, summary or Total rows found.
- There were 1140 rows present of loan_status=‘current’ which has been deleted as loan_status =‘current’ does not
participate in analysis.
- No duplicates rows found.
- There were 55 columns which is having all the rows values as null/blank and doesn’t participate in analyze has
been removed.
- ‘url’ and ‘member_id’ is unique in nature and has been deleted. Have kept ‘id’ for future purpose analyse.
- ‘desc’ and ‘title’ text/description values and doesn’t participate has been dropped from analysis.
- Limiting our analysis till ‘Group’ level only hence sub group has been dropped.
- Using domain knowledge, behavioral data is captured and hence will not available during the loan approval
and doesn’t participate in analysis. 21 behavioral data columns has deleted.
- 8 columns whose values were 1, and is uniqueness in nature has been dropped from analysis.
- There were two columns which is having more that 50% of data as na has been removed. 

## Analysis
- Univariate Analysis
  - Quantitative Variable Analysis
  - Unordered Categorical Variable Analysis
  - Ordered Categorical Variable Analysis
  - Univariate Segmented Analysis
- Bivariate Analysis
- Correlation
  
## Conclusions
- Most of the loan amount applied was in the range of 5k-14k
- Most of the applicant's rate of interest is between in the range of 8%-14%
- CA state has the maximum amount of loan applications
- Income range 0-40000 has high chances of charged off
- interest rate more than 16% or very high has good chances of charged off as compared to other category intrest rates.
- Charged off proportion is increasing with higher intrest rates.
- Those who are not owning the home is having high chances of loan defaults.
- Those applicants who is having home loan or car loan is having low chances of loan defaults. Those applicants having loan
  for small business is having high chances for loan defaults.
- High DTI value is having high risk of defaults
- Higher the Bankruptcies record higher the chance of loan defaults
- TN States is holding highest number of loan defaults
- The Loan applicants with loan Grade G is having highest Loan Defaults. The Loan applicants with loan A is having lowest
  Loan Defaults
- Year 2007 is highest loan defaults. 2009 is having lowest loan defaults
- Purpose : Debt Consolidation has high chances of loan defaults
- Employee experience : 10 years has high chances of loan default
- Annual income range : Medium(40K-80K) segment has high chances of loan default
- Home ownership and Verification status : Rent (Verified and Not Verified) and Mortgage (Verified) has high chances of
loan default


## Technologies Used
- numpy - version 1.19.2
- pandas - version 1.1.3
- matplotlib - version 3.3.2
- seaborn - version 0.11.0


## Contact
Created by [@SuryaGopasana] - feel free to contact me!
