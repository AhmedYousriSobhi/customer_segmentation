# Customer Segmentation and Marketing Strategy Optimization: A Data-Driven Approach

| Info | Description |
|:-----:|:----------:|
| Project Objective |Customer Segmentation|
| Assignee | Ahmed Yousri Sobhi |
| Assignee's email | [ahmedyousrisobhi@gmail.com](ahmedyousrisobhi@gmail.com) |
| Department | Data Science |

## Table of Content
- [Customer Segmentation and Marketing Strategy Optimization: A Data-Driven Approach](#customer-segmentation-and-marketing-strategy-optimization-a-data-driven-approach)
  - [Table of Content](#table-of-content)
  - [Objective](#objective)
  - [Project Structure](#project-structure)
  - [Setup Environment](#setup-environment)
  - [Dataset Schema](#dataset-schema)
  - [Analysis Report](#analysis-report)

## Objective
Our goal is to use data insights to better understand our customers. By analyzing their demographics, behavior, and how they respond to our marketing efforts, we aim to create personalized strategies that resonate with different customer groups. Ultimately, we want to boost engagement, loyalty, and revenue by tailoring our approach to what our customers truly want.

## Project Structure
```bash
.
├── data                   # Dataset files
|   ├── raw
|   ├── intermid
|   ├── output
├── nb_workspace           # Jupiter notebooks
├── docs                   # Documentation files which includes analysis report
├── report                 # Reports files
|   ├── plots              # Figures files
|   ├── reports            # Reports HTML files
├── src                    # Source scripts files
|   ├── env                # Script file to create project directory environment
|   ├── model              # Exported trained models
└── README.md
```

## Setup Environment
Go inside the project directory

```bash
cd project_directory
```

Install Required Libararies and packages.

```bash
pip install -r requirements.txt
```

In case of initial setup, create required folders directory using environment script

```bash
python ./src/env/setup_env.py
```

## Dataset Schema
This dataset are divided into 4 categories:
- Customer's Information: [ID, Year_Birth, Education, Marital_status, Income, Kidhome, Teenhome, DT_Customer, Recency, Complain]
- Products: [MntWines, MntFruits, MntMeatProducts, MntFishProducts, mnSweetProducts, MntGoldProds]
- Promotion: [NumDealsPurchases, AcceptedCmp1, AcceptedCmp2, AcceptedCmp3, AcceptedCmp4, AcceptedCmp5, Response]
- Place: [NumWebPurchases, NumCatalogPurchases, NumStorePurchases, NumWebVisitsMonth]

|Feature|Description|Type|
|--|--|--|
|'ID'| Customer’s unique identifier | int64|
|'Year_Birth'| Customer's birth year| int64|
|'Education'| Education Qualification of customer| object|
|'Marital_Status'| Marital Status of customer| object|
|'Income'| Customer's yearly household income| int64|
|'Kidhome'| Number of children in customer's household | int64|
|'Teenhome'|Number of teenagers in customer's household | int64|
|'Dt_Customer'| Date of customer's enrollment with the company| timestamp|
|'Recency'| Number of days since customer's last purchase| int64|
|'MntWines'| Amount spent on wine| int64|
|'MntFruits'| Amount spent on fruits| int64 |
|'MntMeatProducts'| Amount spent on meat products | int64|
|'MntFishProducts'| Amount spent on fish products| int64|
|'MntSweetProducts'| Amount spend on sweets products| int64 |
|'MntGoldProds'| Amount spend on gold products| int64 |
|'NumDealsPurchases'| number of purchase deals| int64|
|'NumWebPurchases'| Number of purchases made through the web| int64|
|'NumCatalogPurchases'|Number of purchases made through catalogs | int64|
|'NumStorePurchases'| Number of purchases made in physical stores| int64|
|'NumWebVisitsMonth'|Number of web visits in a month | int64|
|'AcceptedCmp1'| Whether the customer accepted Marketing Campaign 1| int64|
|'AcceptedCmp2'| Whether the customer accepted Marketing Campaign 2| int64|
|'AcceptedCmp3'| Whether the customer accepted Marketing Campaign 3| int64|
|'AcceptedCmp4'| Whether the customer accepted Marketing Campaign 4| int64|
|'AcceptedCmp5'|Whether the customer accepted Marketing Campaign 5 | int64|
|'Complain'| Whether the customer has made a complaint | int64|
|'Z_CostContact'| Cost associated with contacting the customer | int64|
|'Z_Revenue'| Revenue associated with contacting the customer| int64|
|'Response|  Customer's response to the company's offer| int64|

## Analysis Report
Included inside directory -> docs/analysis_report.pdf

