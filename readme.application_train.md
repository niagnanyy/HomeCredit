
# EDA for Application Train Data - Jericho Medion

This project covers the Exploratory Data Analysis (EDA) for the `application_train.csv` dataset. The analysis aims to uncover insights into loan applications and identify potential predictors for the risk of default. Below are the key analyses, insights, and business recommendations derived from the data.

## Table of Contents
1. Data Overview
2. Univariate and Multivariate Analysis
3. Business Insights
4. Recommendations

## 1. Data Overview
The `application_train.csv` dataset includes loan application data with multiple features such as income, credit amount, annuity, employment duration, and more. The target variable represents whether a customer defaulted on their loan (1) or not (0). However, in this analysis, we're using the test dataset (`application_test.csv`) to build a predictive model for default risk, which doesn't include a target.

### Key Features:
- `SK_ID_CURR`: Unique customer ID.
- `AMT_INCOME_TOTAL`: Total income of the applicant.
- `AMT_CREDIT`: Credit amount applied for.
- `DAYS_EMPLOYED`: Days the applicant has been employed.

## 2. Univariate and Multivariate Analysis
### Univariate Analysis
Several features were explored through distribution plots and summary statistics to understand their distribution and presence of any outliers. Notable findings:
- **AMT_INCOME_TOTAL**: Exhibits a right-skewed distribution with some extreme values.
- **DAYS_EMPLOYED**: Has negative values, which indicate the number of days since employment began (before the loan application).
- **AMT_CREDIT**: Shows a distribution with some extreme credit applications.

### Multivariate Analysis
Correlations between key variables such as `AMT_CREDIT`, `AMT_ANNUITY`, and `DAYS_EMPLOYED` were visualized using heatmaps and scatter plots. We found:
- Strong correlation between `AMT_CREDIT` and `AMT_ANNUITY`, which makes sense as larger loans would have higher annuities.
- Weak correlations between other variables, suggesting that further feature engineering may be necessary to uncover meaningful patterns.

## 3. Business Insights
### Insight 1: Microcredit Products for Low-Income Applicants
From the analysis of income distribution, many applicants apply for relatively small loans. Offering microcredit products with low interest rates and flexible terms could be beneficial.

### Insight 2: Employment Stability as a Predictor
Analysis of the `DAYS_EMPLOYED` feature suggests that applicants who have been employed longer may be more stable and thus lower-risk. Offering them better loan terms could increase customer retention and reduce risk.

### Insight 3: Segmenting Loan Products by Age Group
Applicants aged 30-50 represent the largest segment. Targeting this group with products like home or car loans can increase engagement and product uptake.

## 4. Recommendations
1. **Microcredit Products**: Develop microcredit offerings to cater to the large group of low-income applicants.
2. **Employment Verification**: Implement stricter employment verification for applicants with short employment history to reduce default risk.
3. **Target Marketing**: Focus marketing campaigns on applicants aged 30-50 with tailored loan products (e.g., mortgage, car loans).
4. **Loyalty Programs**: Reward customers with long employment history with lower interest rates or better loan terms.
5. **Income-Based Loan Caps**: Cap loan amounts based on applicant income to prevent over-borrowing and defaults.

## Conclusion
By focusing on employment stability, income levels, and loan segmentation by age, the company can optimize its loan offerings to reduce default risk and better serve its customers.

---
**Author**: Jericho Medion Haryono
