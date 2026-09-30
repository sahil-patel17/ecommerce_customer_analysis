# E-Commerce Customer Behavior Analysis

## Project Overview

This project analyzes customer shopping behavior using an e-commerce
customer dataset containing 3,900 customer purchase records.

The objective of this project is to understand customer demographics,
purchasing behavior, product preferences, subscription patterns,
payment methods, seasonal trends, and customer satisfaction.

The project follows a complete data analysis workflow including:

- Data understanding
- Data cleaning
- Exploratory Data Analysis (EDA)
- Business insight generation
- Data visualization

---

## Business Objective

The analysis aims to answer questions such as:

- Who are the customers?
- How does purchasing behavior vary across age groups?
- Which product categories and products are most popular?
- Do subscription customers behave differently?
- Which payment methods are commonly used?
- Does purchasing behavior change across seasons?
- What can customer review ratings tell us?
- Are there meaningful relationships between numerical variables?

---

## Dataset

The dataset contains **3,900 customer purchase records** and **18 columns**.

### Main Features

| Feature | Description |
|---|---|
| Customer ID | Unique customer identifier |
| Age | Customer age |
| Gender | Customer gender |
| Item Purchased | Product purchased |
| Category | Product category |
| Purchase Amount (USD) | Amount spent on the purchase |
| Location | Customer location |
| Size | Product size |
| Color | Product color |
| Season | Purchase season |
| Review Rating | Customer review rating |
| Subscription Status | Whether customer has a subscription |
| Shipping Type | Shipping method |
| Discount Applied | Whether discount was applied |
| Promo Code Used | Whether promo code was used |
| Previous Purchases | Number of previous purchases |
| Payment Method | Payment method used |
| Frequency of Purchases | Customer purchase frequency |

---

## Data Cleaning

The following preprocessing steps were performed:

- Checked dataset structure and data types
- Checked missing values
- Checked duplicate records
- Verified numerical ranges
- Examined categorical values for inconsistencies
- Treated `Customer ID` as an identifier rather than a numerical feature
- Handled missing values in `Review Rating`

There were **37 missing values** in `Review Rating`.

These missing values were replaced using the **median rating of 3.8**.

The cleaned dataset was saved separately so that the original raw dataset remained unchanged.

---

## Exploratory Data Analysis

The analysis covers the following areas:

### 1. Customer Demographics

Analyzed:

- Age distribution
- Gender distribution
- Age groups
- Average purchase amount by age group

### 2. Purchase Behavior

Analyzed:

- Total sales
- Average purchase amount
- Median purchase amount
- Purchase amount distribution
- Discount vs non-discount purchases

### 3. Product & Category Analysis

Analyzed:

- Product category distribution
- Most purchased products
- Products generating the highest total sales
- Average purchase amount by category

### 4. Subscription Analysis

Analyzed:

- Subscriber vs non-subscriber distribution
- Average purchase amount
- Total sales
- Purchase frequency patterns

### 5. Payment Method Analysis

Analyzed:

- Payment method usage
- Average purchase amount
- Total sales
- Subscription distribution by payment method

### 6. Season Analysis

Analyzed:

- Customer distribution by season
- Average purchase amount by season
- Total sales by season

### 7. Review Rating Analysis

Analyzed:

- Review rating distribution
- Average purchase amount by rating
- Average rating by product category

### 8. Correlation Analysis

Analyzed relationships between:

- Age
- Purchase Amount
- Review Rating
- Previous Purchases

---

## Key Insights

### Customer Behavior

- The dataset contains **3,900 customers**.
- Customer distribution across seasons is relatively balanced.
- Payment method usage is also relatively balanced.
- Customers are distributed across a wide age range.

### Purchasing Behavior

- Total sales in the dataset are approximately **$233K**.
- Average purchase amount is approximately **$59.76**.
- Purchase amounts remain relatively consistent across different customer segments.

### Product & Category

- **Clothing** has the highest number of purchases and highest total sales.
- Product-level purchase counts are relatively evenly distributed.
- Average purchase values across categories are fairly similar.

### Subscription

- Non-subscribers represent the majority of customers.
- Subscription and non-subscription customers have very similar average purchase values.
- Purchase frequency patterns are relatively similar between the two groups.

### Seasonality

- **Fall** has the highest average purchase amount.
- **Summer** has the lowest average purchase amount.
- However, the difference between seasons is relatively small.

### Customer Satisfaction

- Review ratings range from **2.5 to 5.0**.
- Average ratings across product categories are relatively similar.
- Review rating and purchase amount show a very weak relationship.

### Correlation

The numerical variables show very weak linear relationships.

For example:

- Age ↔ Purchase Amount: approximately **-0.01**
- Purchase Amount ↔ Review Rating: approximately **0.03**
- Purchase Amount ↔ Previous Purchases: approximately **0.01**

This suggests that these numerical variables do not have strong linear relationships in this dataset.

---

## Tools & Technologies

- Python
- Pandas
- NumPy
- Matplotlib
- Jupyter Notebook
- Exploratory Data Analysis
- Data Cleaning
- Data Visualization

---

## Project Structure

```text
Ecommerce_Customer_Analysis/
│
├── data/
│   ├── raw/
│   │   └── customer_shopping_behavior.csv
│   │
│   └── cleaned/
│       └── customer_shopping_behavior_cleaned.csv
│
├── notebook/
│   └── ecommerce_customer_analysis.ipynb
│
├── visualizations/
│
├── report/
│
└── README.md
