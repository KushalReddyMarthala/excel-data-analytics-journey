# Subscription Churn Analysis 

Customer Retention | Segmentation | Excel Analytics

## Project Summary

This project investigates customer churn within a subscription business using a dataset of 100 customers.

The analysis evaluates churn across geography, subscription plan, customer tenure, and rule-based risk categories to identify patterns that could support customer retention strategies.

## Business Question

### Which customer characteristics are most strongly associated with churn?

To answer this, the analysis examines:

Geographic variation in churn
Plan-level retention performance
Tenure-based churn patterns
Customer risk segmentation
Risk model effectiveness

## Dataset

100 customers | 4 countries | 3 plans | 8 fields

### Countries:

India | USA | UK | Australia

### Subscription Plans:

Basic | Standard | Premium

### Fields:

Customer ID | Signup Date | Plan | Monthly Fee | Country | Region | Tenure | Status

## Analytical Process

Raw Customer Data
       ↓
Data Organization
       ↓
Customer Segmentation
       ↓
Churn Rate Analysis
       ↓
Risk Classification
       ↓
Model Validation
       ↓
Insights & Visualization
## Key Metrics
Country
UK — 45.8% churn
Highest churn rate among the four countries analyzed.
Australia — 16.7% churn
Lowest churn rate in the dataset.

## Subscription Plan

Basic — 60.0% churn

Standard — 27.5% churn

Premium — 13.3% churn

The difference between Basic and Premium customers represents the strongest plan-level churn gap observed.

## Tenure
Tenure	          Churn
0–6 months	   25.0%
7–12 months	   30.0%
13–18 months	   31.0%
19–24 months	   47.6%

Longer tenure did not correspond to lower churn in this dataset.

## Risk Model

A rule-based customer risk model was developed using customer characteristics.

Risk levels:

High Risk | Medium Risk | Low Risk

The model was evaluated by comparing risk classifications against actual customer churn.

The results indicate that the initial model provides useful segmentation but requires additional variables to become a stronger predictive model.

## Key Business Insights

01 — Plan matters

Basic customers show substantially higher churn than Premium customers.

02 — Geography matters

The difference between the highest- and lowest-churn countries suggests potential market-specific retention factors.

03 — Long tenure is not necessarily safe

The 19–24 month segment recorded the highest churn rate, indicating that retention efforts should continue throughout the customer lifecycle.

## Excel Functions Used
COUNTIFS
SUMIFS
AVERAGEIFS
IF
IFS
AND
OR
RANK.EQ
TEXTJOIN
SUMPRODUCT

## Deliverables
File	Purpose
subscription_data_100.xlsx	Raw customer dataset
03_subscription_churn_project.xlsx	Completed analysis
screenshot-churn-insights-1.png	Analysis/dashboard screenshot
screenshot-churn-insights-2.png	Analysis/dashboard screenshot

## Tools & Skills

Tool: Microsoft Excel

Skills: Data Analysis · Segmentation · KPI Development · Conditional Logic · Risk Classification · Data Visualization · Business Insights

## Conclusion

The analysis identified subscription plan as the strongest visible churn differentiator, while geography and tenure revealed additional retention patterns.

The next analytical step would be to incorporate variables such as customer usage, engagement, support interactions, pricing changes, and payment behavior to develop a more robust churn prediction model.
