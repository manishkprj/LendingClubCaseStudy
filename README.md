# Lending Club Case Study

## Table of Contents

- [General Information](#general-information)
- [Technologies Used](#technologies-used)
- [Conclusions](#conclusions)
- [Acknowledgements](#acknowledgements)
- [Contact](#contact)
- [License](#license)

## General Information

### Project Information

This data science project uses the Lending Club dataset to predict whether a loan will be defaulted or not.

### Project Background

Lending Club is the largest online loan marketplace, facilitating personal loans, business loans, and financing for medical procedures. Borrowers can access lower interest rate loans through a fast online interface. However, lending to risky applicants poses a significant financial loss (credit loss) to the company. Credit loss occurs when a borrower defaults on their loan. This project aims to identify the factors that lead to loan defaults.

### Project Statement

The goal is to find the driving factors that lead to loan defaults, which are a major source of financial loss for the company.

### Data Set

The dataset is a CSV file containing loan data from Lending Club.

## Conclusions

### Univariate Analysis

 -  Loan Status : Defaulted loan are low in numbers compared to Fully Paid.
 -	Loan Amount: Most of the loan amount applied was in the range of 5k-14k
 -	Term: More than half of the loan taken has term of 36 months compared to 60 months.
 -	Interest Rate: The interest rate is more crowded around 5-10 and 10-15 with a drop near 8-10
 -	Grade: A large amount of loans are with grade 'A' and 'B' compared to other grade (C, D, E, F, G)
 -	Employment Duration: Majority of borrowers have working experience greater than 10 years
 -	Home Ownership: Majority of borrowers don't possess property and are on mortgage or rent.
 -	Verification Status: About 50% of the borrowers are verified by the company or have source verified.
 -	Annual Income: Majority of burrowers have very low annual income compared to rest.
 -	Purpose: A large percentage of loans are taken for debt consolidation followed by credit card.
 -	Address: Majority of the borrowers are from the large urban cities like California, new York, Texas, Florida
 -	DTI: Majority of the borrowers have very large debt compared to the income registered, concentrated in the 10-15 DTI ratio.
 -	Public Record Bankruptcies: Majority of the borrowers have no record of Public Recorded Bankruptcy.
 -	Month: Majority of the loans are given in last quarter of the year
 -	Year: The number of loans approved increases with the time at exponential rate, thus we can say that the loan approval rate is increasing with the time

### Segmented Univariate Analysis

  - Charged off loans have a larger IQR and a higher median, suggesting that defaults are more common among larger loans.
  - Debt Consolidation is the most common loan purpose and also defaulter larger in this area.
  - The 60 month term has higher chance of defaulting than 36 month term whereas the 36 month term has higher chance of fully paid loan.
  - A higher DTI ratio indicates a higher chance of defaulting.
  - Defaulters are most likely from RENT or Mortgage categories
  - Analysis shows that defaulter most likely have low income.
  - The default loan amount increases with interest rate and shows are decline after 17.5 % interest rate.
  - The Employees with 10+ years of experience are likely to more defaulter and  also have higher chance of fully paying the loan.

### Bivariate Analysis

- Higher interest rates might correlate with higher default rates
- Loans with grade A have the lowest median interest rate, around 7%. This indicates that A grade is a lower interest rate category.
- Loans with grade G have the highest median interest rate, around 20%. This indicates that G grade is a higher interest rate category.
- The median interest rate increases steadily from grade A to grade G, reflecting the increasing risk associated with the Grade.

- With grade C, D, E, F, G higher chance of defaulter
- Charged Off loans have consistently higher interest rates across all grades. This suggests that higher interest rates are a strong indicator of default risk
- Grades with (E, F, G) show higher median interest rates and more variability, indicating a higher risk of default. Defaulters are more likely found in these grades with high-interest rates

- Borrowers with higher annual incomes are more likely to fully repay their loans, particularly those with no public record bankruptcies.
- Borrowers with one or more public record bankruptcies are more likely to default on their loans, especially if they have lower annual incomes

### Multi Variate Analysis

- A lower annual income combined with a higher interest rate is a strong indicator of a potential defaulter.
- DTI combined with a higher interest rate is a strong indicator of a potential defaulter than someone has no DTI.
- A higher loan amount combined with a higher interest rate is a strong indicator of a potential defaulter.

- Defaulter is most likely, If they have high DTI and Large amount and they have taken the loan for 60 months term.
- Defaulter is most likely, If they have some DTI and low annual income and they have taken the loan for 60 months term.
- Defaulter is most likely  from the Grade F and Garde G with higher Interest rate.
- Defaulter is gradually increasing with the grade.
- Defaulter is most likely, if they have taken a large amount loan for small business and they have low annual income.

### Recommendations

#### Major combined driving factors that can be used to predict the probability of default and avoid credit loss

-  DTI with Large amount and term
-  DTI with low Annual Income and term
-  Grade with higher Interest rate
-  Purpose of loan is small/business
-  Lower annual Income with higher interest
-  Public record bankruptcies with lower annual income

#### More Major driving factors that can be used to predict the probability of default and avoid credit loss

- DTI
- Grade
- Higher interest rates
- Lown annual Income
- Public record bankruptcies

## Technologies Used

- Python - v3.11.5
- Pandas - v2.2.1
- NumPy - v1.26.4
- Seaborn - v0.12.2
- MatplotLib - v3.7.2
- Plotly - v5.22.0

## Acknowledgements

This project was inspired by the UpGrad IITB Programme as a case study for the Machine Learning and Artificial Intelligence course.

## Contact

Created by [@manishkprj](https://github.com/manishkprj) - feel free to contact me!

## License

This project is open source and available without restrictions.


<!-- Optional -->
<!-- ## License -->
<!-- This project is open source and available under the [... License](). -->

<!-- You don't have to include all sections - just the one's relevant to your project -->