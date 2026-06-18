# Online Retail Sales Analysis

## Project Overview

This project analyzes the UCI Online Retail dataset to understand sales trends, customer behavior, product performance, country-level performance, and product associations.

The goal of this project is to turn raw transactional retail data into business insights that can support decision-making in areas such as customer retention, product bundling, market strategy, and sales performance tracking.

## Dataset

The dataset used in this project is the Online Retail dataset from the UCI Machine Learning Repository.

Dataset source: UCI Machine Learning Repository
Dataset name: Online Retail
Dataset period: December 2010 to December 2011

## Business Questions

This project answers the following questions:

* What are the overall sales trends?
* Which countries generate the most revenue?
* Which products perform best by revenue, quantity, and invoice count?
* How do customers differ in spending and purchase frequency?
* Which customer segments are most valuable?
* Which products are commonly purchased together?

## Tools Used

* Python
* Pandas
* NumPy
* Matplotlib
* Jupyter Notebook
* Power BI, planned for dashboarding
* GitHub

## Project Structure

```text
online-retail-sales-analysis/
├── data/
│   ├── raw/
│   └── cleaned/
├── notebooks/
│   ├── 01_data_understanding.ipynb
│   ├── 02_data_cleaning.ipynb
│   ├── 03_exploratory_data_analysis.ipynb
│   ├── 04_customer_analysis.ipynb
│   ├── 05_market_basket_analysis.ipynb
│   └── 06_final_insights.ipynb
├── reports/
├── visuals/
│   └── charts/
├── README.md
├── requirements.txt
└── .gitignore
```

## Notebook Summary

### 01 Data Understanding

Explored the raw dataset, checked column types, missing values, duplicates, cancellations, negative quantities, invalid prices, date range, and country distribution.

### 02 Data Cleaning

Cleaned the dataset by removing duplicates, removing cancelled invoices, removing negative quantities, removing invalid prices, standardizing product descriptions, creating revenue fields, and flagging non-product rows.

### 03 Exploratory Data Analysis

Analyzed overall sales performance, monthly revenue trends, country-level revenue, product performance, sales by day and hour, invoice activity, and average order value.

### 04 Customer Analysis

Analyzed customer-level behavior, including top customers by revenue, order frequency, customer lifetime, one-time versus repeat customers, country-level customer patterns, and RFM customer segmentation.

### 05 Market Basket Analysis

Analyzed product pairs that are commonly purchased together in the same invoice. The analysis focused on product co-purchases, support, confidence, and lift.

### 06 Final Insights

Summarized the main findings, business recommendations, project limitations, and suggested next steps.

## Key Findings

* The cleaned dataset generated total revenue of 10,642,110.80.
* The dataset includes 19,960 unique invoices, 3,922 unique products, 4,338 identified customers, and 38 countries.
* The United Kingdom is the dominant market by customer count and total revenue.
* Non-UK customers had higher average revenue per customer than UK customers.
* Customer revenue is highly concentrated.
* Best Customers represent about 21.42% of identified customers but generate about 70.09% of customer revenue.
* Repeat customers generate most of the identified customer revenue.
* Some products have high revenue because of large bulk orders, so product performance should be evaluated using multiple metrics.
* Market basket analysis showed that products from the same product family are often purchased together, such as jumbo bags, lunch bags, teacups, alarm clocks, and Christmas products.

## Business Recommendations

* Focus on retaining high-value customers through loyalty programs and personalized offers.
* Re-engage at-risk and past high-value customers with win-back campaigns.
* Promote product bundles based on strong product pair associations.
* Investigate high-value international markets.
* Evaluate products using revenue, quantity, invoice count, and consistency rather than revenue alone.

## Limitations

* The dataset covers only one year of transactions.
* December 2011 is incomplete because the dataset ends on December 9.
* CustomerID is missing for many rows, so customer analysis only includes identified customers.
* Cancelled invoices and negative quantities were removed to focus on completed positive sales.
* Market basket analysis focused on the top 100 most frequent products.
* The project uses a simple product-pair approach instead of full Apriori or FP-Growth association rule mining.

## Next Steps

Future improvements could include:

* Building a Power BI dashboard.
* Adding dashboard screenshots to the visuals folder.
* Applying Apriori or FP-Growth for deeper market basket analysis.
* Investigating high-value outlier transactions in more detail.
* Comparing UK and non-UK customers more deeply.
* Creating a more detailed customer retention strategy.

## Conclusion

This project demonstrates a complete data analysis workflow, from data understanding and cleaning to exploratory analysis, customer segmentation, market basket analysis, and final business recommendations.

The analysis shows that revenue is highly concentrated among a small group of valuable customers, that the UK is the main market, and that many products are purchased together in clear product families. These findings can support customer retention, product bundling, and market strategy decisions.
