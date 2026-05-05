# E-commerce-Sales-Analysis-Project

## Project Overview

This project analyzes real-world e-commerce transaction data from a UK-based online retailer.  
The goal is to understand sales performance, customer behavior, product demand, geographic concentration, returns, and customer segmentation.

The analysis was performed using Python, Pandas, Matplotlib, Seaborn, and Scikit-learn.

---

## Dataset

The dataset contains **541,909 records** and **8 columns** representing online retail transactions.

### Key Columns

| Column | Description |
|---|---|
| InvoiceNo | Unique invoice identifier |
| StockCode | Product code |
| Description | Product name |
| Quantity | Number of items purchased |
| InvoiceDate | Transaction date and time |
| UnitPrice | Price per item |
| CustomerID | Unique customer identifier |
| Country | Customer country |

---

## Project Objectives

- Analyze overall sales performance
- Identify top-selling and high-revenue products
- Understand customer spending behavior
- Analyze revenue by country
- Detect and interpret outliers
- Segment customers using RFM analysis
- Apply K-Means clustering for customer grouping
- Analyze product returns
- Generate business insights and recommendations

---

## Tools & Libraries

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- Google Colab

---

## Project Workflow

### 1. Data Cleaning

The dataset was cleaned by:

- Standardizing column names
- Handling missing values
- Removing duplicate records
- Separating sales transactions from returns
- Removing invalid transactions with zero or negative unit prices
- Converting date columns to datetime format

### 2. Feature Engineering

New features were created to support analysis:

- `total_price`
- `year`
- `month`
- `hour`
- `month_year`

### 3. Exploratory Data Analysis

The EDA focused on:

- Monthly revenue trends
- Top products by revenue
- Top products by quantity sold
- Revenue by country
- Customer spending distribution
- Outlier analysis

### 4. Customer Segmentation

RFM analysis was used to segment customers based on:

- Recency
- Frequency
- Monetary value

Customers were grouped into segments such as:

- Champions
- Loyal Customers
- At Risk
- Hibernating
- Needs Attention

### 5. K-Means Clustering

K-Means clustering was applied on RFM values to identify hidden customer groups and support data-driven segmentation.

### 6. Return Analysis

Returned transactions were analyzed to calculate return rate and identify the most returned products.

---

## Key Insights

- The United Kingdom contributes the majority of total revenue, showing a strong geographic concentration.
- A limited number of products generate a significant share of revenue.
- Customer spending is highly skewed, meaning a small group of customers contributes heavily to total revenue.
- Outliers likely represent bulk purchases or high-value customers and were retained in the analysis.
- RFM segmentation helped identify valuable customer groups such as Champions and Loyal Customers.
- Return analysis can help identify potential product quality issues or customer expectation gaps.

---

## Business Recommendations

- Focus on retaining high-value customers through loyalty programs.
- Promote top-performing products to maximize revenue.
- Expand into additional markets to reduce dependency on the UK.
- Investigate highly returned products to improve customer satisfaction.
- Use RFM segments for targeted marketing campaigns.
- Re-engage At Risk and Hibernating customers with personalized offers.

---
