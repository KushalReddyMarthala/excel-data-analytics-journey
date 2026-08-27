# Data Analytics Journey

Real datasets. Real problems. Documented as I work through them — no daily tutorial recaps, just the actual thinking behind each project.

## How Each Project Is Documented

Every folder in this repo follows the same structure:

- **Problem** — what needed to be solved
- **Understanding the data** — what shape the data was in and what needed attention
- **Approach** — the method and tools used to solve it
- **Solution** — the final result and what it means

## Projects

| # | Project | Problem | Result |
|---|---|---|---|
| 01 | [Data Cleaning](./01-data-cleaning) | 105-row employee dataset with inconsistent formatting, mixed date formats, missing values, and duplicates | 105 messy rows → 100 clean, usable records |
| 02 | [Sales Analysis](./02-sales-analysis) | 50 sales orders — which regions and categories actually drive revenue? | Found that order volume and revenue don't always align |
| 03 | [Subscription Churn](./03-subscription-churn) | 100 subscription customers — which countries, plans, and tenure groups have the highest churn? | Found that plan type is the strongest visible churn differentiator, with churn also varying significantly by geography and tenure |

## Project 03 — Subscription Churn

The third project analyzes customer churn across:

- 4 countries
- Multiple geographic regions
- 3 subscription plans
- Customer tenure
- Customer risk categories

### Key Findings

- **UK** has the highest churn rate at **45.8%**
- **Australia** has the lowest churn rate at **16.7%**
- **Basic** customers have the highest churn at **60.0%**
- **Premium** customers have the lowest churn at **13.3%**
- Churn increases from **25.0%** among 0–6 month customers to **47.6%** among 19–24 month customers
- The initial rule-based risk model provides useful segmentation but requires additional variables to become a stronger predictive model

[View the full Subscription Churn Analysis →](./03-subscription-churn)

## Skills & Techniques

### Excel

- Data Cleaning
- Data Validation
- Conditional Formatting
- COUNTIFS
- SUMIFS
- AVERAGEIFS
- IF / Nested IF
- IFS
- AND / OR
- RANK.EQ
- TEXTJOIN
- SUMPRODUCT
- Customer Segmentation
- KPI Analysis
- Data Visualization
- Business Insights

