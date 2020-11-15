# Loan Features Effect on Loan Status and Borrower's APR
## by Alya Fattah

## Dataset Overview

This data set contains 113,937 loans with 81 variables on each loan, including loan amount, borrower rate (or interest rate), current loan status, borrower income, and many others.The dataset can be found in [here](https://s3.amazonaws.com/udacity-hosted-downloads/ud651/prosperLoanData.csv),with feature documentation available [here] (https://docs.google.com/spreadsheets/d/1gDyi_L4UvIrLTEC6Wri5nbaMmkGmLQBk-Yx3z0XDEtI/edit) .


## Summary of Findings

In the univariate exploratory analysis, we highlighted that ~50%  of the loans are current (56576 out of 113907) and ~15% of the loans are charged-off or defaulted (17010 out of 113907. We noticed also after zooming in that the debt to income ratio distribution is right skewed and the majority of the borrowers have a ratio between 0-0.4.In addition, We saw that ~93% of the borrowers have income supporting documentation available. These observations indicates although half of the loans are current/active, the company has managed to reduce its risk with low debt to income ratio and high available supporting documentation. We also observed that the distribution of borrower's APR is multimodal. We saw mutiple peaks at 0.1,0.2,0.3 and ~0.35 with very few loans greater than 0.4.

In the bivariate exploration, we focused on the selected 8 features only. We observed high positive correlation between CurrentCreditLines & OpenRevolvingAccounts (~0.85) and negative correlation between BorrowerAPR & ProsperScore (-0.67).Similarly between BorrowerAPR & LoanOriginalAmount(-0.32) - the higher the loan amount the lower APR.The current loans also have a very high income verification which is a good sign as Proper's is ensuring that the borrowers have supporting documentation.There is also a relationship between Prosper's rating and term. We noticed that employed people take the most number of loans which are all mainly 36 months long with ranking A having the highest 36 months number of loans and ranking C highest 60 months number of loans.  However, we dont have enough data for part-time, retired and not employed borrowers to see any relationship between term and Proper rating for these employment statuses.

In this multivariate analysis, we focused on the selected 5 features only. We observed a negative correlation between APR and loan amount regardless of the term. We noticed better Prosper ratings changes the correlation between APR and loan amount from negative to positive. People with higher ratings tend to borrower higher amounts and have lower APR.We also saw that the borrower APR decrease with the increase of borrow term for borrowers with HR-C ratings and the APR increase with the increase of borrow term for borrowers with B-AA ratings.


## Key Insights for Presentation

For the presentation, I just focused on the 5 main features effecting loan status and borrower's APR: employment status, debt to income ratio, loan amount, term and Proper rating.

We first looked at the number of loans for each employment status and the debt to income distribution. We then checked the borrower's APR per loan amount and the number of loans per employement status & term. We finally investigated the term effect on the relationship of Prosper Rating vs APR and Prosper Rating vs Loan Amount.

To conclude, Prosper is reducing its risk by targeting low debt to income ratio, high amount of loans with income verification and mainly employed borrowers. We observed high negative correlation between Borrower 's APR & Loan Original Amount(-0.323) as the higher the Loan Amount the lower APR would be. We saw a relationship between Employment Status and Term where employed people take the most number of loans which are all mainly 36 months long. We also noticed that the borrower APR decrease with the increase of borrowers' term with HR-C ratings and the APR increase with the increase of borrowers' term with B-AA ratings.

