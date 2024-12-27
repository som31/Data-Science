# Lending Club Case Study
Lending Club, a consumer finance marketplace specializing in offering a variety of loans to urban customers, faces a critical challenge in managing its loan approval process. When evaluating loan applications, the company must make sound decisions to minimize financial losses, primarily stemming from loans extended to applicants who are considered "risky."

These financial losses, referred to as credit losses, occur when borrowers fail to repay their loans or default. In simpler terms, borrowers labeled as "charged-off" are the ones responsible for the most significant losses to the company.

The primary objective of this exercise is to assist Lending Club in mitigating credit losses. This challenge arises from two potential scenarios:

Identifying applicants likely to repay their loans is crucial, as they can generate profits for the company through interest payments. Rejecting such applicants would result in a loss of potential business.
On the other hand, approving loans for applicants not likely to repay and at risk of default can lead to substantial financial losses for the company.


## Table of Contents
* [General Info](#Business Understanding)
* [Conclusions](#conclusions)
* [Acknowledgements](#acknowledgements)

<!-- You can include any other section that is pertinent to your problem -->

## Business Understanding
The objective is to pinpoint applicants at risk of defaulting on loans, enabling a reduction in credit losses. This case study aims to achieve this goal through exploratory data analysis (EDA) using the provided dataset.

The company wants to understand the driving factors (or driver variables) behind loan default, i.e. the variables which are strong indicators of default. The company can utilise this knowledge for its portfolio and risk assessment.

The primary objective of this exercise is to assist Lending Club in mitigating credit losses. This challenge arises from two potential scenarios:

Identifying applicants likely to repay their loans is crucial, as they can generate profits for the company through interest payments. 
Rejecting such applicants would result in a loss of potential business.
On the other hand, approving loans for applicants not likely to repay and at risk of default can lead to substantial financial losses for the company.

## Types of Decisions by the Company 
When a person applies for a loan, there are two types of decisions that could be taken by the company:

**Loan accepted** If the company approves the loan, there are 3 possible scenarios described below:

1.**Fully paid**: Applicant has fully paid the loan (the principal and the interest rate)

2.**Current**: Applicant is in the process of paying the instalments, i.e. the tenure of the loan is not yet completed. These candidates are not labelled as 'defaulted'.

3.**Charged-off** : Applicant has not paid the instalments in due time for a long period of time, i.e. he/she has defaulted on the loan

**Loan rejected** : The company had rejected the loan (because the candidate does not meet their requirements etc.). Since the loan was rejected, there is no transactional history of those applicants with the company and so this data is not available with the company (and thus in this dataset)

<!-- You don't have to answer all the questions - just the ones relevant to your project. -->

## Some Conclusions
1) **Low Annual Income** : Applicants with annual incomes less than $40,000 have a higher likelihood of defaulting. The company should consider setting an Amount lending range depending on the income levels.

2) **DTI and Interest Rates** : High Debt-to-Income (DTI) ratios in the 12%-18% are associated with maximum defaults.

3) **Risk Assessment for Grades B, C, and D**: The loan applicants from Grades B, C, and D contribute to maximum of the "Charged Off" loans hence the company should consider implementing a stricter risk assessment and underwriting criteria for applicants falling into these grades.

4) **Verification Status** : The Maximum defaults were committed by Non Verified loan applicants. 


## Contact
Created by [@githubusername] - feel free to contact me!


<!-- Optional -->
<!-- ## License -->
<!-- This project is open source and available under the [... License](). -->

<!-- You don't have to include all sections - just the one's relevant to your project -->
