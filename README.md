# Credit Card Customer & Transaction Analytics

## Overview

This project is a Power BI analytics report built to analyze credit card transaction activity and customer characteristics.

The report combines transaction-level and customer-level data to provide insights into revenue, transaction activity, interest earned, card categories, expenditure types, customer demographics, and customer satisfaction.

The Power BI report contains two main sections:

* **Credit Card Transaction Report**
* **Credit Card Customer Report**

Both datasets are connected using the `Client_Num` field.

## Objective

The objective of this project is to analyze credit card transaction patterns and customer demographics to understand:

* Revenue and transaction performance
* Interest earned from credit card activity
* Performance across different card categories
* Spending and expenditure patterns
* Customer segments based on demographic characteristics
* Revenue trends over time
* Customer satisfaction
* Relationships between customer characteristics and credit card performance

## Dataset

The project uses the **Credit Card Customers Dataset**, consisting of two CSV files.

### 1. `credit_card_db.csv`

Contains credit card transaction and account-level information, including:

* Card category
* Credit limit
* Transaction amount
* Transaction count
* Revenue
* Interest earned
* Revolving balance
* Expenditure type
* Transaction method

**Approximate records:** 10,108
**Columns:** 18

### 2. `customer_db.csv`

Contains customer demographic and profile information, including:

* Age
* Gender
* Income
* Education
* Customer job
* Marital status
* State
* Dependent count
* Customer satisfaction score

**Approximate records:** 10,108
**Columns:** 15

The two datasets are related using the `Client_Num` field.

The raw dataset was obtained from a public online/Kaggle source, while the Power BI report and analysis were created as part of this project.

## Dashboard Preview

### Credit Card Transaction Report

![Credit Card Transaction Report](images/transaction-report.jpeg)

### Credit Card Customer Report

![Credit Card Customer Report](images/customer-report.jpeg)

## Power BI Report

### Credit Card Transaction Report

The transaction report focuses on credit card performance and transaction behavior.

### Key KPIs

* Total Revenue
* Total Transaction Amount
* Total Interest Earned
* Total Transaction Count

### Visualizations

* Revenue by Quarter with transaction count trend
* Revenue by Expenditure Type
* Revenue by Education Level
* Revenue by Customer Job
* Revenue by Card Category
* Revenue by Transaction Method
* Card Category performance table
* Client count by Quarter
* Client count by Gender
* Client count by Card Category
* Client count by Income Group

### Filter

* Week Start Date

---

### Credit Card Customer Report

The customer report focuses on customer demographics and their relationship with credit card performance.

### Key KPIs

* Average Customer Satisfaction Score
* Total Interest Earned
* Total Income
* Total Revenue

### Visualizations

* Client count by Quarter
* Client count by Card Category
* Revenue by Gender
* Customer revenue and income table
* Revenue by Income Group
* Revenue by Age Group
* Revenue by Education Level
* Revenue by State
* Revenue by Dependent Count
* Revenue by Marital Status
* Revenue trend over time by Gender

### Filter

* Week Start Date

## Data Model

The Power BI report uses two main tables:

```text
credit_card_db
       |
       | Client_Num
       |
customer_db
```

The `Client_Num` field is used to connect transaction/account information with customer demographic information.

This relationship allows transaction performance to be analyzed together with customer characteristics.

## Analysis Areas

The report provides analysis across several dimensions:

* Card Category
* Gender
* Age Group
* Income Group
* Education Level
* Customer Job
* Marital Status
* State
* Expenditure Type
* Transaction Method
* Quarter
* Week Start Date

## Tools & Technologies

* **Microsoft Power BI**
* **Power BI Data Model**
* **CSV**
* **Data Visualization**
* **Data Analysis**

## Project Structure

```text
Credit-Card-Analytics-PowerBI/
│
├── Credit Card Customer & Transaction Analytics.pbix
├── images/
│   ├── transaction-report.jpeg
│   └── customer-report.jpeg
└── README.md
```

## How to Use

1. Download the `.pbix` Power BI report from this repository.
2. Open the file using Microsoft Power BI Desktop.
3. Navigate between the Transaction and Customer report sections.
4. Use the available date filter to explore the report.
5. Interact with the visualizations to analyze different customer and transaction segments.

## Key Takeaways

This project demonstrates the use of Power BI to combine customer and transaction data into an interactive analytical report.

It covers:

* Customer and transaction data analysis
* Data modeling using a common customer identifier
* KPI analysis using Power BI aggregations
* Interactive data visualization
* Customer segmentation
* Revenue and transaction analysis
* Time-based analysis
* Business-oriented dashboard design

## Author

**Gopal Yadav**

GitHub: [gopalyadav-ai](https://github.com/gopalyadav-ai)
