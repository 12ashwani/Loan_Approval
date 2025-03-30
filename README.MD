# Problem Statement
Dream Housing Finance Company deals in all kinds of home loans and has a presence across urban, semi-urban, and rural areas. Customers apply for home loans online, and the company validates their eligibility based on various details provided during the application process.

The company aims to automate the loan eligibility process in real time using customer-provided data. To achieve this, a dataset has been provided to identify customer segments eligible for loan approval, allowing the company to specifically target these customers.

---

# Data Dictionary

## **Train File** (CSV containing customer loan eligibility information)

| Variable           | Description                                      |
|--------------------|--------------------------------------------------|
| Loan_ID           | Unique Loan ID                                   |
| Gender            | Male/Female                                      |
| Married           | Applicant married (Y/N)                         |
| Dependents        | Number of dependents                            |
| Education         | Applicant Education (Graduate/Under Graduate)   |
| Self_Employed     | Self-employed (Y/N)                             |
| ApplicantIncome   | Applicant income                                |
| CoapplicantIncome | Co-applicant income                            |
| LoanAmount        | Loan amount in thousands                        |
| Loan_Amount_Term  | Term of loan in months                          |
| Credit_History    | Credit history meets guidelines                 |
| Property_Area     | Urban/Semi Urban/Rural                          |
| Loan_Status       | (Target) Loan approved (Y/N)                    |

## **Test File** (CSV containing customer information for loan eligibility prediction)

| Variable           | Description                                      |
|--------------------|--------------------------------------------------|
| Loan_ID           | Unique Loan ID                                   |
| Gender            | Male/Female                                      |
| Married           | Applicant married (Y/N)                         |
| Dependents        | Number of dependents                            |
| Education         | Applicant Education (Graduate/Under Graduate)   |
| Self_Employed     | Self-employed (Y/N)                             |
| ApplicantIncome   | Applicant income                                |
| CoapplicantIncome | Co-applicant income                            |
| LoanAmount        | Loan amount in thousands                        |
| Loan_Amount_Term  | Term of loan in months                          |
| Credit_History    | Credit history meets guidelines                 |
| Property_Area     | Urban/Semi Urban/Rural                          |

---

# **Submission File Format**

| Variable    | Description                         |
|------------|-------------------------------------|
| Loan_ID    | Unique Loan ID                      |
| Loan_Status | (Target) Loan approved (Y/N)       |

---

# **Evaluation Metric**
The model performance will be evaluated based on the accuracy of predicting the loan status for the test data (`test.csv`). The submission must be formatted as shown in the sample submission file.

At the backend, the actual loan status for the test dataset will be compared against the predicted values to compute accuracy.

---

# **Public and Private Split**
The test dataset is divided into two parts:
- **Public (25%)**: Initial responses will be checked and scored on this subset.
- **Private (75%)**: The final rankings will be based on this score, which will be revealed after the competition ends.

---

# **Guidelines for Final Submission**
Ensure that the final submission includes the following:
1. **Solution File** containing the predicted loan status for the test dataset (following the required format).
2. **Code File** to reproduce the submission (mandatory for valid submission).