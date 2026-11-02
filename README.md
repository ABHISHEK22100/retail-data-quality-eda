# Retail Store Sales — Data Quality & Exploratory Data Analysis

## 1. Project Overview

This project focuses on analyzing retail store transaction data to identify sales patterns, evaluate product category performance, understand customer purchasing behaviour, and generate actionable business insights.

The project follows a structured data analysis workflow, starting with data understanding and quality assessment, followed by data cleaning, exploratory data analysis (EDA), and business recommendations.

## 2. Project Objectives

* Understand the structure and quality of retail transaction data.
* Identify and handle missing values.
* Perform exploratory data analysis to discover sales patterns.
* Analyze product categories, payment methods, and sales channels.
* Evaluate monthly and yearly revenue trends.
* Generate meaningful business insights and recommendations.

## 3. Dataset Information

* Dataset: Retail Store Sales
* Original Records: 12,575 transactions
* Features: 11 columns
* Format: CSV

### Key Features

* Transaction ID
* Customer ID
* Category
* Item
* Price Per Unit
* Quantity
* Total Spent
* Payment Method
* Location
* Transaction Date
* Discount Applied

## 4. Project Structure

```text
retail-data-quality-eda/
│
├── notebooks/
│   ├── 01_data_understanding.ipynb
│   ├── 02_data_cleaning.ipynb
│   ├── 03_eda.ipynb
│   └── 04_business_insights.ipynb
│
├── raw_data/
│   └── retail_store_sales.csv
│
├── processed_data/
│   └── retail_store_sales_cleaned.csv
│
├── README.md
├── requirements.txt
└── .gitignore
```

## 5. Project Workflow

### Step 1: Data Understanding

* Dataset structure and dimensions.
* Data types and statistical summaries.
* Missing value analysis.
* Duplicate record checks.
* Data consistency and validation checks.

### Step 2: Data Cleaning

* Missing product names handled using an "Unavailable" category.
* Missing Price Per Unit values recovered using available transaction values.
* Unrecoverable Quantity and Total Spent values retained.
* Missing Discount Applied values retained rather than guessed.
* Datatypes converted where appropriate.
* Cleaned dataset exported to CSV.

### Step 3: Exploratory Data Analysis

* Product category analysis.
* Revenue and average transaction value analysis.
* Payment method analysis.
* Online versus in-store sales comparison.
* Monthly and yearly revenue trends.
* Product demand analysis.
* Customer revenue contribution.
* Correlation analysis.

### Step 4: Business Insights

* Identify high- and low-performing product categories.
* Evaluate payment method performance.
* Compare online and in-store sales.
* Examine yearly revenue patterns.
* Analyze customer revenue contribution.
* Develop data-driven business recommendations.

## 6. Key Business Findings

* Butchers generated the highest category revenue: 208,118.
* Milk Products generated the lowest category revenue: 180,112.
* Furniture recorded the highest quantity sold: 8,462 units.
* Cash was the most frequently used payment method and generated the highest payment-method revenue.
* Online sales generated higher revenue than in-store sales.
* 2024 recorded the highest revenue among complete calendar years.
* The top 10 customers contributed approximately 41.82% of total revenue.

*Note: Revenue calculations use available Total Spent values. Transactions with missing Total Spent values are excluded from these calculations.*

## 7. Data Limitations

* The dataset contains only 25 unique customers.
* Quantity and Total Spent are missing for 604 transactions.
* Discount Applied contains 4,199 missing values.
* Missing product names limit product-level demand analysis.
* January 2025 contains partial-month data.
* The dataset does not provide enough information to establish the causes of revenue changes.

## 8. Technologies Used

* Python
* Pandas
* NumPy
* Matplotlib
* Seaborn
* JupyterLab

## 9. How to Run the Project

### Step 1: Clone the Repository

```bash
git clone https://github.com/ABHISHEK22100/retail-data-quality-eda.git

### Step 2: Navigate to the Project Directory

```bash
cd retail-data-quality-eda
```

### Step 3: Install Dependencies

```bash
pip install -r requirements.txt
```

### Step 4: Launch JupyterLab

```bash
jupyter lab
```

### Step 5: Run the Notebooks

Execute the notebooks in the following order:

1. 01_data_understanding.ipynb
2. 02_data_cleaning.ipynb
3. 03_eda.ipynb
4. 04_business_insights.ipynb

## 10. Project Outcome

This project demonstrates a structured approach to data quality assessment, data cleaning, exploratory analysis, and business insight generation using Python.

It highlights the importance of data validation, transparent handling of missing values, and evidence-based business recommendations.

## 11. Version Control

This project is maintained using Git for version control and GitHub for repository hosting.

The complete source code, Jupyter notebooks, and project documentation are organized for reproducibility.

## 12. Author

**Abhishek Kumar**
B.Tech – Artificial Intelligence
Aspiring Data Science / Machine Learning Engineer
