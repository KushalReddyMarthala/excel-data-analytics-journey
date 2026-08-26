## Problem
A retail company wants to understand where its revenue is actually coming from — not just 
which regions and categories are the busiest, but which ones actually drive the most business value. 
This project analyzes 50 sales orders to answer that question using Excel formulas alone, 
without any pivot tables or visualization tools beyond basic charts.

## Understanding the data
The dataset contains 50 sales transactions with the following columns:
- Order ID, Order Date, Customer, Region, Product, Category, Quantity, Sales

Orders are spread across 4 regions (North, South, East, West) and 4 product categories 
(Electronics, Furniture, Stationery, Appliances). Unlike my first project, this dataset 
was already clean — the focus here was entirely on analysis, not cleaning.

Before writing any formulas, I looked at the data manually first to form a hypothesis: 
I assumed the region and category with the most orders would also generate the most revenue. 
That assumption turned out to be wrong for regions, but correct for one category and wrong for another.

## Approach
I used four core formulas to answer different business questions:

- **SUMIF** — calculated total revenue per region and per category, to identify where the money is coming from
- **COUNTIF** — calculated the number of orders per region and per category, to identify where the activity is concentrated
- **AVERAGEIF** — calculated average order value per region, to understand whether high revenue came from many small orders or fewer large ones
- Manual comparison — cross-checked order volume against revenue side by side to see where the two metrics agreed and where they diverged

I organized all formulas in a separate "Calculations" section next to the raw data, so the 
raw dataset stays untouched and every number can be traced back to its formula.

## Solution

**Region-level finding:**
South placed the most orders (16 total) of any region — more than North, East, or West. 
But North generated the highest total revenue (₹14,26,899), despite placing only 12 orders. 
The reason becomes clear when you look at average order value: North's average order is 
worth ₹1,18,908, compared to South's ₹75,808 — a difference of roughly 57%. North isn't 
winning because of more transactions; it's winning because each transaction is worth 
significantly more.

**Category-level finding:**
Electronics led in both order count (19) and revenue (₹33,34,922) — a case where volume 
and value moved together, which makes sense given electronics tend to be higher-priced items.

But Stationery and Furniture told a different story. Both categories had exactly 11 orders — 
identical order counts. Yet Stationery generated ₹4,99,498 in revenue, nearly 84% more than 
Furniture's ₹2,71,935. Same number of transactions, very different business impact.

**Key takeaway:**
Order count measures activity, not value. Two categories with identical order volume can 
have dramatically different revenue outcomes, and a region generating fewer transactions 
can still be the strongest revenue driver. If a business only tracked "which region places 
the most orders" or "which category sells the most units," it would draw the wrong conclusion 
about where to focus resources.

## Files
- `sales_data_50.xlsx` — raw order data with all calculation formulas included in a separate labeled section
- `02_sales_analysis_project.xlsx` — final insights sheet with formatted tables, two focused charts, and written key-insight summaries for each finding
