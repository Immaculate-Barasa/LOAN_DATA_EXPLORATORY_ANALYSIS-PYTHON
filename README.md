# Loan_Data_Exploratory_Analysis-Python
An in-depth analysis of a company's loan applications covering data cleaning, handling missing values, exploratory data analysis and visualisations. The aim was to investigate how an applicant's demographics, financial position and household structure influence loan approval outcomes, and identify areas where the company can optimize its credit risk assessment.

## Business Problem
The business faces operational inefficiencies due to incomplete applicant data and a lack of clear visibility into how demographic factors such as education level and family size, and geographic locations influence loan approvals. Without data-driven credit risk insights, the company risks either rejecting viable borrowers or blindly approving high-risk applicants.

## Data Overview
The dataset set contains 614 rows and 13 columns.
The key information from the columns includes:
- Gender
- Marital status
- Number of dependents
- Education (graduate or non-graduate)
- Self-employment status
- Applicant's income
- Co-applicant's income
- Loan amount
- Repayment term
- Credit history
- Property area
- Loan status.

## Business Questions
To guide the investigation, the analysis focused on answering the following questions:

1. What is the typical loan size requested by the client base, and how is the demand distributed?

2. Does an applicant's formal education level impact their likelihood of loan approval?

3. Does a higher number of dependents increase credit risk and lead to higher loan rejections?

4. Where are the biggest gaps in the current data collection pipeline, and how do they impact the risk assessment?

## Key Insights
1. Most applicants request relatively small-to-moderate loan sizes, with a heavy concentration between KES 100,000 and KES 150,000.
   <p align = "center">
   <img src = "Loan_amount.png" width ="70%" alt = "Loan Amount Distribution Chart">
   </p>

3. Graduates submit the vast majority of applications and secure a much higher volume of approvals than non-graduates.
    <p align = "center">
   <img src = "Education.png" width ="70%" alt = "Education Vs Approval Status Chart">
   </p>
4. The majority of the applicants have zero dependents. However, for those with more dependents the company does not heavily penalize them; their approval rate remains consistently higher than their rejection rate.
 <p align = "center">
   <img src = "Dependents.png" width ="70%" alt = "Dependents Vs Approval Status Chart">
   </p>
5. The Credit_History column contains the highest number of missing values. This creates a blind spot that makes it difficult to assess risk accurately.

## Recommendations
1. Streamline small loan approvals since the highest customer demand is for loans between KES 100,000 and KES 150,000. 

2. Introduce alternative credit scoring such as mobile money transaction histories  to help viable non-graduates.

3. Tighten data collection controls by updating the digital loan application form to make the credit check field mandatory. Liaise with  Credit Reference Bureau (CRB) to pull history instantly.

## Tools
Python,
Pandas,
Numpy,
Seaborn,
Matplotlib,
Jupyter Notebook
