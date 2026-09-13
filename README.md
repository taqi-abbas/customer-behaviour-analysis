# Customer Shopping Behavior Analysis

## Overview

This project analyzes customer shopping data to understand purchasing patterns, product performance, customer engagement, and revenue distribution. It demonstrates a complete data analytics workflow using Python, MySQL, Power BI, project documentation, and a presentation created with Gamma.

The project converts raw customer data into clear business insights that can support marketing, product, subscription, and customer-retention decisions.

## Dataset

The dataset contains **3,900 customer shopping records** and includes information such as:

- Customer ID, age, gender, and location
- Item purchased and product category
- Purchase amount
- Review rating
- Subscription status
- Shipping type
- Discount and promotional-code usage
- Previous purchases
- Payment method
- Purchase frequency

## Tools Used

| Tool | Purpose |
| --- | --- |
| Python | Data exploration, cleaning, and feature engineering |
| Pandas | Data manipulation and analysis |
| Jupyter Notebook | Documenting the Python workflow |
| MySQL | Running business-focused SQL queries |
| Power BI | Creating measures, visualizations, and an interactive dashboard |
| Microsoft Word | Preparing the final project report |
| Gamma | Creating the project presentation |

## Project Steps

### 1. Data Import

- Imported the dataset into a Jupyter Notebook.
- Reviewed the first rows, column names, data types, and dataset dimensions.

### 2. Exploratory Data Analysis

- Examined summary statistics.
- Checked unique values and category distributions.
- Reviewed customer, product, purchase, and engagement variables.
- Identified missing values and potential data-quality issues.

### 3. Data Cleaning

- Found 37 missing values in the review-rating column.
- Filled missing ratings using the median rating of the relevant product category.
- Standardized column names using lowercase snake_case formatting.
- Renamed the purchase-amount field for easier SQL analysis.
- Verified that no missing values remained after cleaning.

### 4. Feature Engineering

- Created customer age groups.
- Converted purchase-frequency labels into approximate numbers of days.
- Segmented customers as New, Returning, or Loyal based on previous purchases.

### 5. SQL Analysis

Loaded the cleaned data into MySQL and answered business questions related to:

- Revenue by gender
- Customers using discounts who spent above average
- Products with the highest average ratings
- Shipping-method performance
- Subscriber and non-subscriber spending
- Products with the highest discount usage
- Customer loyalty segments
- Top products within each category
- Repeat buyers by subscription status
- Revenue contribution by age group

The SQL analysis uses aggregation, filtering, subqueries, `CASE` expressions, common table expressions, and window functions.

### 6. Power BI Dashboard

Built an interactive Power BI dashboard containing:

- Number of customers
- Average purchase amount
- Average review rating
- Subscription-status distribution
- Revenue and sales by category
- Revenue and sales by age group
- Filters for subscription status, gender, category, and shipping type

### 7. Project Report

Created a professional report explaining the project objective, dataset, cleaning process, SQL analysis, dashboard, findings, and business recommendations.

### 8. Gamma Presentation

Created a presentation in Gamma to communicate the project workflow, dashboard, key findings, and recommendations in a concise visual format.

## Dashboard

![Customer Shopping Behavior Dashboard](images/customer_behavior_dashboard.png)

> Add your Power BI dashboard screenshot to the `images` folder using the filename `customer_behavior_dashboard.png`.

## Key Results

- **Total customers:** 3,900
- **Total revenue:** $233,081
- **Average purchase amount:** $59.76
- **Average review rating:** 3.75 out of 5
- **Subscribed customers:** 27%
- **Non-subscribed customers:** 73%
- Clothing was the highest-performing category by revenue and sales.
- Young adults generated the highest revenue among the age groups.
- The large non-subscriber segment represents a strong conversion opportunity.

## Business Recommendations

- Create targeted campaigns to convert non-subscribers.
- Maintain strong inventory availability for Clothing products.
- Cross-sell Accessories to Clothing customers.
- Develop age-specific campaigns for young adults.
- Investigate low-rated products and customer-service issues.
- Use separate communication strategies for New, Returning, and Loyal customers.

## Project Structure

```text
customer-shopping-behavior-analysis/
├── data/
│   └── customer_shopping_behavior.csv
├── notebooks/
│   └── customer_shopping_behavior_analysis.ipynb
├── sql/
│   └── customer_analysis_queries.sql
├── dashboard/
│   └── customer_behavior_dashboard.pbix
├── report/
│   └── customer_shopping_behavior_report.docx
├── presentation/
│   └── customer_shopping_behavior_presentation.pdf
├── images/
│   └── customer_behavior_dashboard.png
└── README.md
```

## How to Run the Project

### Python Analysis

1. Clone the repository:

```bash
git clone https://github.com/your-username/customer-shopping-behavior-analysis.git
```

2. Open the project folder:

```bash
cd customer-shopping-behavior-analysis
```

3. Install the required Python libraries:

```bash
pip install pandas numpy matplotlib seaborn jupyter
```

4. Start Jupyter Notebook:

```bash
jupyter notebook
```

5. Open the notebook from the `notebooks` folder and run the cells in order.

### MySQL Analysis

1. Create a MySQL database.
2. Import the cleaned customer dataset into a table named `customer`.
3. Open `sql/customer_analysis_queries.sql` in MySQL Workbench.
4. Select the correct database and execute the queries.

### Power BI Dashboard

1. Install Power BI Desktop.
2. Open `dashboard/customer_behavior_dashboard.pbix`.
3. Update the data-source path if Power BI requests it.
4. Refresh the data and use the slicers to explore the dashboard.

## Files Included

- Original or cleaned dataset
- Python EDA and cleaning notebook
- MySQL query file
- Power BI dashboard
- Detailed project report
- Gamma presentation
- Dashboard screenshot

## Author

**Taki Abbas**

Data Analytics Portfolio Project
