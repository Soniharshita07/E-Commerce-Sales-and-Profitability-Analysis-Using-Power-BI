# E-Commerce Sales and Profitability Analysis Using Power BI

An interactive Power BI dashboard that analyzes sales, profit, and customer purchasing patterns for an Indian e-commerce retailer. It shows where revenue turns into profit, and in which months, states, and payment modes it does not.


## Business Problem
An online retailer can have healthy sales and still earn very little profit. Managers need to know which months, categories, and regions make money, and how customers pay, so they can decide where to focus inventory, marketing, and operations.

**Key questions**
1. What is the overall profit margin, and how does profit move month to month and quarter to quarter?
2. Which product categories drive the most units sold?
3. Which states contribute the most profit?
4. Who are the most profitable customers?
5. How do customers pay (COD, UPI, EMI, cards), and what might that mean for operations?

**Intended users:** sales managers, category managers, regional leads.

## Tools
Power BI, DAX, Power Query, Excel

## Approach
- **KPIs built with DAX:** Total Amount, Total Profit, Quantity Sold, Average Order Value, ]
- **Interactivity:** quarter buttons (Q1 to Q4) and a dropdown filter, 
- **Visuals:** KPI cards, monthly profit trend, profit by state, quantity share by category, most profitable customers, payment method split, best-selling products


## Key Findings

Figures below are read from the dashboard. Values marked "approx." are estimated from chart bars and should be confirmed in Power BI before publishing.

| # | Finding | Evidence | Business implication |
|---|---------|----------|----------------------|
| 1 | Profit margin is thin | About 37K profit on about 438K sales, roughly 8.4% | Small cost or discount changes could erase profit |
| 2 | Profit is uneven across the year | Strongest in Jan to Apr and Nov (Nov approx. 10K). Negative in May, Jul, Sep, and Dec | Some months sell but lose money. The cause needs investigation (discounts, product mix, costs) |
| 3 | Unit sales are concentrated in Clothing | Clothing 63%, Electronics 21%, Furniture 17% of quantity (rounded, so totals 101%) | Volume is concentrated in one category. Profit by category is needed to see whether volume equals profit |
| 4 | Maharashtra leads profit by state | Ranking: Maharashtra, Madhya Pradesh, Uttar Pradesh, Delhi [add values] | Regional focus and stock planning can start with the top states |
| 5 | Nearly half of orders use COD | COD 44%, UPI 21%, Debit 13%, Credit 12%, EMI 10%  | Cash on delivery may carry higher return and handling risk. This is a hypothesis, not tested here |

## Recommendations (proposed, not implemented)
| Action | Supported by | KPI to monitor | Further analysis |
|--------|--------------|----------------|------------------|
| Review loss-making months for discounting and product mix | Finding 2 | Monthly profit margin % | Profit by month and sub-category, discount data if available |
| Compare margin, not just volume, across categories | Findings 1 and 3 | Profit margin % by category | Add profit by category and sub-category visuals |
| Test incentives to move COD customers to prepaid methods | Finding 5 | COD share of orders | Compare return and cancellation rates by payment mode |
| Prioritize inventory and promotion planning in top profit states | Finding 4 | Profit per state | Profit by city and category within each state |

## Limitations
- [Public Kaggle dataset. Add "synthetic" ]
- [Covers only one period: state it. Seasonality cannot be confirmed from a single year.]
- Profit is used as provided. [Confirm whether cost and discount fields exist.]
- Results show patterns, not causes. No experiment tested any recommendation.
- The dashboard does not yet show profit by category or sub-category.

## How to Open
1. Download `MAHADEV SALES.pbix` from this repository.
2. Open it in Power BI Desktop.
3. [Note the data file location, and whether refresh is needed.]
<img width="1057" height="597" alt="Screenshot 2026-10-24 193626" src="https://github.com/user-attachments/assets/320d7ee7-aa82-4017-bd16-70666b4c0227" />



## Skills Demonstrated
Data cleaning, data modeling, DAX measures, KPI design, dashboard design, translating data into business questions
