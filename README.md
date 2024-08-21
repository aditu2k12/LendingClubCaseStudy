# Lending Club Case Study
> You work for a consumer finance company which specialises in lending various types of loans to urban customers. When the company receives a loan application, the company has to make a decision for loan approval based on the applicant’s profile. Two types of risks are associated with the bank’s decision:

If the applicant is likely to repay the loan, then not approving the loan results in a loss of business to the company

If the applicant is not likely to repay the loan, i.e. he/she is likely to default, then approving the loan may lead to a financial loss for the company

The data given below contains information about past loan applicants and whether they ‘defaulted’ or not. The aim is to identify patterns which indicate if a person is likely to default, which may be used for taking actions such as denying the loan, reducing the amount of loan, lending (to risky applicants) at a higher interest rate, etc.


## Table of Contents
* [General Info](#general-information)
* [Technologies Used](#technologies-used)
* [Conclusions](#conclusions)
* [Acknowledgements](#acknowledgements)

<!-- You can include any other section that is pertinent to your problem -->

## General Information
This company is the largest online loan marketplace, facilitating personal loans, business loans, and financing of medical procedures. Borrowers can easily access lower interest rate loans through a fast online interface. 

Like most other lending companies, lending loans to ‘risky’ applicants is the largest source of financial loss (called credit loss). Credit loss is the amount of money lost by the lender when the borrower refuses to pay or runs away with the money owed. In other words, borrowers who default cause the largest amount of loss to the lenders. In this case, the customers labelled as 'charged-off' are the 'defaulters'.  

If one is able to identify these risky loan applicants, then such loans can be reduced thereby cutting down the amount of credit loss. Identification of such applicants using EDA is the aim of this case study.

<!-- You don't have to answer all the questions - just the ones relevant to your project. -->

## Conclusions
Based on the EDA, we have identified the following features as most important in detecting default loans

a) loan amount
   1) With increasing loan amount the probability of defaults also increases.
   2) when the loan amount is greater than 13k, the default rate is always greater than the overall
      dataset default rate of 14.5%
	
b) Interest Rate
   1) With increasing interest rate the probability of defaults also increases
   2) when the interest rate is greater than 12.5%, the default rate is always greater than the overall
      dataset default rate of 14.5%
	
c) Annual Income
   1) With increasing annual income the probability of defaults decreases
   2) when the annual income is less than 64k, the default rate is always greater than the overall
      dataset default rate of 14.5%
	

d) Debt to Annual Income Ratio
   1) With increasing debt to annual income ratio the probability of defaults also increases
   2) when this ratio is greater than 10, the default rate is always greater than the overall
      dataset default rate of 14.5%
	
e) Revolving line utilization rate
   1) With increasing revolving line utilization rate the probability of defaults also increases
   2) when this rate is greater than 40, the default rate is always greater than the overall
      dataset default rate of 14.5%
	
f) term
   1) The probability of default is more high for a loan given for 60 months than for 36 months
   2) For 36 months the default rate is 11% and for 60 months its 25%
	
g) grade
   1) The probability of default increases as we move in alphabetical order of grades; i.e the probability of
      default is more in G grade (~34%),less in F(~33%), more less in E(~27%) and same pattern follows till A(~6%).
   2) Their is a order associated with grade
   3) From grade C onward till G, the default rate is always greater than the overall dataset default rate of 14.5%
	
h) sub-grade
   1) Sub Grade column follows the same pattern as that of grade with loan status column leaving a few exceptions;
      i.e the A sub grades default rate is lower than of B, B sub grades have a default rate less than of C
      and same pattern follows till G sub grades
   2) Within each grade the the default rate increases with alphabetical order,eg; within A grade the default rate
      of A1 is less than of A2, A2 is less than of A3, A3 is less than of A4 and A4 is less than of A5.
    3) The default rate of F5 is highest(~48%) and that of A1 is lowest(~2.6%) among all sub-grades
    4) From all sub-grade C onward till all sub-grade of G, the default rate is always greater than the
       overall dataset default rate of 14.5%
	
i) purpose
    1) The probability of default is highest for small_business(~27%),followed by renewable_energy(~18.6%)
    2) When the loan is taken for debt_consolidation, educational, medical, moving, other, renewable_energy, 
       small_business then the default rate is always greater than the overall dataset default rate of 14.5%
	  
j) derogatory public records: Customers with known derogatory public records more prone for default with 
   rate greater than the overall dataset default rate of 14.5% 
	
k) known public bankruptcies: Customers with known public bankruptcies more prone for default with rate
   greater than the overall dataset default rate of 14.5% 
	
l) Customers taking any loan amount but with interest rate greater than 15% are much more prone to 
   default with default rate greater than 14.5% 

m) Customers taking loan amount greater than 10.5K and annual income less than 64k have more prone for 
   default with default rate greater than 14.5%

n) Customers taking loan amount greater than 15.5K and dti greater than 10 have more prone for default
   with default rate greater than 14.5%

o) Customers having loan amount greater than 10.5K and revolving rate greater than 70 have more prone 
   for default with default rate greater than 14.5%

p) Customers having annual income less than 94k and interest rate greater than 15 have more prone for
   default with default rate greater than 14.5%

q) Customers taking any loan amount but for term of 60 months are more prone for default than customers 
   taking the same amount for 30 months with default rate greater than 14.5%

r) Customers taking any loan amount but beloning to grade C, D, E or F are more prone for 
   default with default rate greater than 14.5%

s) Customers taking any loan amount but having a public record of bankruptcy are more prone 
   for default with default rate greater than 14.5%

t) Customers having any annual income but taking loan for a term of 60 months are more prone
   for default with default rate greater than 14.5%

u) Customers having annual income less than 79k and belonging to grade C, D, E or F are more prone
   for default with default rate greater than 14.5%
   
v) Customers having any annual income and taking loan for small business purpose are most prone for 
   default with default rate greater than 14.5%

w) Customers having annual income less than 64k and taking loan for debt consolidation, housing or other purposes
   are most prone for default with default rate greater than 14.5%



## Technologies Used
* Python - version 3.11.4
* Matplotlib - version 3.7.1
* Numpy - version 1.24.3
* Pandas - version 1.5.3
* Seaborn - version 0.12.2

<!-- As the libraries versions keep on changing, it is recommended to mention the version of library used in this project -->

## Acknowledgements
Give credit here.
- This project was inspired by Akashdeep Makkar 
- UpGrad sessions on Exploratory Data Analysis (EDA) on the learning platform.



## Contact
Created by Aditya Singh and Aditya Jain - feel free to contact us!

