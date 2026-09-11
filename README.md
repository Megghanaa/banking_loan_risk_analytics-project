````markdown
# Banking & Loan Risk Analytics Dashboard

## 📊 Power BI Data Analytics Project

An interactive Power BI dashboard developed to analyze loan applications, approval patterns, customer financial profiles, and lending risk.

## 🎯 Project Objective

The objective of this project is to analyze loan application data and identify patterns related to:

- Loan portfolio exposure
- Loan approval rates
- Customer creditworthiness
- Debt-to-income ratio
- Previous loan defaults
- Risk scores
- High-risk loan segments

## 🛠️ Tools & Technologies

- Power BI
- Power Query
- DAX
- Data Cleaning
- Data Visualization
- Exploratory Data Analysis
- Business Intelligence

## 📁 Dataset

The dataset contains loan application and customer financial information.

### Key Attributes

- Loan Amount
- Loan Purpose
- Credit Score
- Employment Status
- Debt-to-Income Ratio
- Previous Loan Defaults
- Risk Score
- Loan Approval Status
- Income
- Interest Rate
- Loan Duration

## 📌 Dashboard Overview

### Executive Overview

The Executive Overview provides a high-level view of the loan portfolio and approval performance.

### Key Performance Indicators

- Total Loans: **20,000**
- Total Loan Amount: **498M**
- Approved Loans: **5,000**
- Approval Rate: **23.9%**

### Key Visualizations

- Total Loan Amount by Loan Purpose
- Approval Rate by Employment Status
- Approval Rate by Credit Score
- Average Risk Score by Loan Purpose
- Approval Rate by Debt-to-Income Ratio
- Approval Rate by Previous Loan Defaults
- Risk Score Distribution
- High-Risk Loans by Loan Purpose

## 🔍 Risk Analysis

The Risk Analysis page focuses on understanding factors associated with lending risk.

The analysis examines:

- Credit score and loan approval
- Debt-to-income ratio and loan approval
- Previous loan defaults and approval
- Risk score distribution
- Average risk score across loan purposes
- High-risk loans across different loan segments

Interactive slicers allow users to filter the dashboard by:

- Loan Purpose
- Employment Status
- Loan Approval Status

## 🧹 Data Preparation

Power Query was used to prepare the dataset before visualization.

### Data Cleaning Steps

1. Imported the loan dataset into Power BI.
2. Verified column names and data types.
3. Checked data quality and validity.
4. Checked for duplicate records.
5. Removed duplicate records where applicable.
6. Converted numerical fields to appropriate data types.
7. Created the cleaned `LoanData` dataset for analysis.

## 📐 DAX Measures

### Total Loans

```DAX
Total Loans =
COUNTROWS(LoanData)
````

### Total Loan Amount

```DAX
Total Loan Amount =
SUM(LoanData[LoanAmount])
```

### Approved Loans

```DAX
Approved Loans =
CALCULATE(
    [Total Loans],
    LoanData[LoanApproved] = 1
)
```

### Approval Rate

```DAX
Approval Rate =
DIVIDE(
    [Approved Loans],
    [Total Loans],
    0
)
```

### High Risk Loans

```DAX
High Risk Loans =
CALCULATE(
    [Total Loans],
    LoanData[RiskScore] >= 70
)
```

### High Risk Rate

```DAX
High Risk Rate =
DIVIDE(
    [High Risk Loans],
    [Total Loans],
    0
)
```

## 💡 Business Value

This dashboard helps analyze:

* Loan portfolio performance
* Approval patterns
* Customer risk indicators
* High-risk loan segments
* Creditworthiness trends
* Factors associated with loan approval

## 📈 Skills Demonstrated

* Power BI
* Power Query
* DAX
* Data Cleaning
* Data Visualization
* KPI Development
* Risk Analytics
* Exploratory Data Analysis
* Business Intelligence

## 🚀 Future Improvements

* Add time-based loan analysis
* Create advanced customer risk segmentation
* Add drill-through functionality
* Connect Power BI to SQL
* Implement automated data refresh
* Explore predictive analytics

## 👩‍💻 Author

**Meghana Mudundi**

B.Tech – Computer Science Engineering

**Interests:** Data Analytics | Business Analytics | Product Management

```
```
