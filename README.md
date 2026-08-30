Here's the updated README with What-If Analysis renumbered to 04:

markdown
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
|---|---------|---------|--------|
| 01 | [Data Cleaning](./01-data-cleaning) | 105-row employee dataset with inconsistent formatting, mixed date formats, missing values, and duplicates | 105 messy rows → 100 clean, usable records |
| 02 | [Sales Analysis](./02-sales-analysis) | 50 sales orders — which regions and categories actually drive revenue? | Found that order volume and revenue don't always align |
| 03 | [Subscription Churn](./03-subscription-churn) | 100 subscription customers — which countries, plans, and tenure groups have the highest churn? | Found that plan type is the strongest visible churn differentiator, with churn also varying significantly by geography and tenure |
| 04 | [What-If Analysis](./04-what-if-analysis) | How sensitive is a SaaS business's unit economics to changes in churn, CAC, and growth? | Churn could roughly double before hitting risk thresholds — but customer growth turns negative before that point |

## Project 03 — Subscription Churn

The third project analyzes customer churn across:
- 4 countries
- Multiple geographic regions
- 3 subscription plans
- Customer tenure
- Customer risk categories

**Key Findings**
- UK has the highest churn rate at 45.8%
- Australia has the lowest churn rate at 16.7%
- Basic customers have the highest churn at 60.0%
- Premium customers have the lowest churn at 13.3%
- Churn increases from 25.0% among 0–6 month customers to 47.6% among 19–24 month customers
- The initial rule-based risk model provides useful segmentation but requires additional variables to become a stronger predictive model

[View the full Subscription Churn Analysis →](./03-subscription-churn)

## Project 04 — What-If Analysis

The fourth project builds a SaaS unit economics model and stress-tests it using Goal Seek, Scenario Manager, and Data Tables.

**Key Findings**
- Goal Seek: churn could roughly double (5% → 10%) before the LTV:CAC ratio hit the risky 3.0 threshold — but at that same churn rate, the business was already losing more customers than it gained
- Scenario Manager: in the Worst Case scenario, MRR barely dropped versus Expected Case, but Net New Customers turned negative — revenue can look healthy right up until it isn't
- Data Table: LTV:CAC drops from 18.7 at 2% churn down to 3.1 at 12% churn, mapped across the full range in a single table

[View the full What-If Analysis →](./04-what-if-analysis)

## Skills & Techniques

**Excel**
- Data Cleaning
- Data Validation
- Conditional Formatting
- COUNTIFS, SUMIFS, AVERAGEIFS
- IF / Nested IF, IFS
- AND / OR
- RANK.EQ
- TEXTJOIN
- SUMPRODUCT
- VLOOKUP, INDEX+MATCH
- PivotTables, PivotCharts
- Slicers
- Goal Seek, Scenario Manager, Data Tables

**Analysis**
- Customer Segmentation
- KPI Analysis
- Data Visualization
- Business Insights
- Financial Modeling
- Sensitivity Analysis
