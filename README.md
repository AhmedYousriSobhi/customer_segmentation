# Customer Segmentation and Marketing Strategy Optimization: A Data-Driven Approach
![image](https://github.com/AhmedYousriSobhi/customer_segmentation/assets/66730765/3cabfabd-51dd-43a7-977f-a5dfb6810989)


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
  - [Dataset Info](#dataset-info)
  - [Project Flow](#project-flow)
  - [Analysis Report](#analysis-report)

## Objective
Our goal is to use data insights to better understand our customers. By analyzing their demographics, behavior, and how they respond to our marketing efforts, we aim to create personalized strategies that resonate with different customer groups. Ultimately, we want to boost engagement, loyalty, and revenue by tailoring our approach to what our customers truly want.

## Project Structure
```bash
.
├── cluster                # Clustering Model Notebook
├── data                   # Dataset files
|   ├── raw
|   ├── intermid
|   ├── output
├── nb_workspace           # Jupiter notebooks
├── docs                   # Documentation files which includes analysis report
|   ├── model              # Exported trained models
├── nb_workspace           # Jupiter notebooks
├── report                 # Reports files
|   ├── analysis_report    # Analysis report
|   ├── plots              # Figures files
|   ├── reports            # Reports HTML files
├── src                    # Source scripts files
|   ├── env                # Script file to create project directory environment
|   ├── tools              # Script files used for model pipeline

└── README.md
```

## Setup Environment
Navigate to the project directory:

```bash
cd project_directory
```

Create a virtual environment (optional but recommended):
```bash
python -m venv venv
```

Install the project dependencies:

```bash
pip install -r requirements.txt
```

In case of initial setup, create required folders directory using environment script:
```bash
python ./src/env/setup_env.py
```

## Dataset Schema
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

## Dataset Info
This dataset are divided into 4 categories:
- Customer's Information: [ID, Year_Birth, Education, Marital_status, Income, Kidhome, Teenhome, DT_Customer, Recency, Complain]
- Products: [MntWines, MntFruits, MntMeatProducts, MntFishProducts, mnSweetProducts, MntGoldProds]
- Promotion: [NumDealsPurchases, AcceptedCmp1, AcceptedCmp2, AcceptedCmp3, AcceptedCmp4, AcceptedCmp5, Response]
- Place: [NumWebPurchases, NumCatalogPurchases, NumStorePurchases, NumWebVisitsMonth]

## Project Flow
The projects is splitted into two parts, where:

__Dataset Exploring__:
- The first part describes all the preprocessing, exploarity data analysis (EDA), and features engineering the dataset has gone through.
- Locatted at: nb_workspace/

__Customers Segmentation__:
- The second part describes the pipeline which the raw dataset is passed through, to the output of customers clusters, passing through all the preprocessing process [Data Cleaning and feature engineering].
- Located at: cluster/customer_segmentation.ipynb

All Steps and Code are documented and commented in the notebooks, so any contributor would simply go through the steps made.

## Analysis Report
Included inside directory -> report/analysis_report/analysis_report.pdf

