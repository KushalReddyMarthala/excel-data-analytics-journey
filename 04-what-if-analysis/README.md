## Problem
A SaaS business wants to understand how sensitive its unit economics are to changes in 
churn, customer acquisition cost, and growth — before those changes actually happen.

## Understanding the data
Built a SaaS unit economics model with 7 inputs (new customers/month, price, churn rate, 
CAC, gross margin, existing customers, marketing spend) and 8 calculated outputs (MRR, 
customer lifetime, LTV, LTV:CAC ratio, net new customers, and more).

## Approach
- **Goal Seek** — worked backward from a target LTV:CAC ratio (3.0, the standard risk 
  threshold) to find the churn rate that would trigger it
- **Scenario Manager** — built 3 named scenarios (Expected, Best, Worst Case) across all 
  7 inputs and generated a side-by-side comparison report
- **Data Table** — tested LTV:CAC across 6 different churn rates (2%–12%) in a single 
  table, instead of running Goal Seek repeatedly

## Solution
- Churn could roughly double (5% → 10%) before LTV:CAC hit the risky 3.0 threshold — 
  but at that same churn rate, the business was already losing more customers than it 
  was gaining. The "safe" ratio and the "safe" growth rate are not the same number.
- In the Worst Case scenario, MRR barely dropped compared to Expected Case, but Net New 
  Customers turned negative (-80/month) — revenue can look healthy right up until it isn't.
- LTV:CAC drops steeply with churn: from 18.7 at 2% churn down to 3.1 at 12% churn.

## Tools used
Goal Seek, Scenario Manager, Data Tables

## Files
- `saas_unit_economics.xlsx` — full model, all 3 What-If tools, and the polished 
  Scenario Summary report
