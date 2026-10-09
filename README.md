# Bank Loan Approval & Credit Risk Analysis using Power BI

## 📊 Project Overview

This project focuses on analyzing bank loan applications and understanding the factors that influence loan approval and credit risk.

The project uses **Power BI** to transform a large bank loan dataset into an interactive dashboard. The dashboard provides insights into loan applications, approval rates, customer income, credit scores, loan amounts, interest rates, education, loan purposes, and previous loan defaults.

The dataset contains **70,000 customer loan application records**.

---

## 🎯 Objectives

The main objectives of this project are:

- Analyze total loan applications.
- Compare approved and rejected loans.
- Calculate the overall loan approval rate.
- Analyze customer credit scores.
- Study the relationship between income and loan amount.
- Analyze loan applications based on education.
- Analyze loan applications based on loan purpose.
- Identify the impact of previous loan defaults.
- Compare average loan amounts and interest rates.
- Understand customer and credit risk patterns.

---

## 🛠️ Tools & Technologies

- **Power BI**
- **Power Query**
- **DAX**
- **Microsoft Excel / CSV Dataset**
- **GitHub**

---

## 📁 Dataset

The dataset contains **70,000 loan application records** with information related to customers and their loan applications.

### Important Dataset Columns

- `person_age` – Customer age
- `person_income` – Customer income
- `person_emp_exp` – Employment experience
- `loan_amnt` – Loan amount
- `loan_int_rate` – Loan interest rate
- `loan_percent_income` – Loan amount as a percentage of income
- `credit_score` – Customer credit score
- `cb_person_cred_hist_length` – Credit history length
- `loan_status` – Original loan approval status
- `person_gender_male` – Gender information
- Education-related columns
- Loan purpose-related columns
- `previous_loan_defaults_on_file_Yes` – Previous loan default information

---

## 🧹 Data Cleaning & Transformation

Data cleaning and transformation were performed using **Power Query**.

The following transformations were performed:

- Corrected data types.
- Converted loan percentage income into percentage format.
- Formatted income and loan amount values.
- Created readable loan approval status.
- Created readable previous loan default status.
- Combined education columns into a single `Education` column.
- Combined loan intent columns into a single `Loan Purpose` column.
- Created a `Gender` column from the original gender indicator.

### Created Columns

**Loan Approval Status**
- Approved
- Rejected

**Previous Loan Defaults**
- Yes
- No

**Education**
- Bachelor
- Master
- Doctorate
- High School

**Loan Purpose**
- Education
- Home Improvement
- Medical
- Personal
- Venture

---

## 📐 DAX Measures

Several DAX measures were created to analyze the dataset.

### Total Applications

```DAX
Total Applications = COUNTROWS('Loan Approval Prediction')
