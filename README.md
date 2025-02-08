# loan-eligibility - The model ultimately takes 22 input features and 4 engineered features.

## Input Features
1. Age – The applicant’s age in years.  
2. AnnualIncome – The applicant’s yearly earnings.  
3. CreditScore – A measure of creditworthiness (and it’s later doubled to amplify its effect).  
4. EmploymentStatus – A categorical feature (e.g. "employed," "self-employed," "unemployed") converted to numeric.  
5. EducationLevel – A categorical indicator (e.g. "bachelor," "master," etc.) encoded as a number.  
6. Experience – Years of work or professional experience.  
7. LoanAmount – The amount of money the applicant is asking to borrow.  
8. LoanDuration – The term or duration of the loan (typically in months).  
9. MaritalStatus – Another categorical feature (e.g. "married," "single") encoded as a number.  
10. NumberOfDependents – The number of dependents the applicant has.  
11. HomeOwnershipStatus – Categorical status of home ownership (e.g. "own," "rent") encoded numerically.  
12. MonthlyDebtPayments – Total monthly payments on existing debts.  
13. DebtToIncomeRatio – The ratio of monthly debt obligations to monthly income.  
14. LoanPurpose – Categorical reason for the loan (for instance, "auto" or "education") encoded numerically.  
15. SavingsAccountBalance – Current balance in savings accounts.  
16. CheckingAccountBalance – Current balance in checking accounts.  
17. MonthlyIncome – The income the applicant earns each month.  
18. JobTenure – How long the applicant has been at their current job.  
19. NetWorth – The overall net worth of the applicant (assets minus liabilities).  
20. BaseInterestRate – A benchmark or base interest rate used in the loan calculations.  
21. InterestRate – The specific interest rate applied to the applicant’s loan.  
22. MonthlyLoanPayment – The expected monthly amount to be paid if the loan is approved.  

## Feature Engineered additional features
1. TotalIncome – An engineered feature computed as AnnualIncome plus SavingsAccountBalance and CheckingAccountBalance.  
2. CreditScore_Income – Another engineered feature calculated as CreditScore multiplied by AnnualIncome (capturing the combined effect of credit history and earnings).  
3. DebtToIncome_CreditScore – The product of DebtToIncomeRatio and CreditScore, which helps adjust debt load relative to creditworthiness.  
4. InterestRate_LoanDuration – The product of InterestRate and LoanDuration, giving a sense of the overall cost of borrowing over time.
