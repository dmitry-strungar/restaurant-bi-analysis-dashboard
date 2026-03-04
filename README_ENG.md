# Restaurant BI Analysis

Power BI project focused on customer behavior analysis, segmentation, and restaurant performance evaluation for a restaurant chain.

---

## Project Overview

This project analyzes sales and customer data of a restaurant network to evaluate:

- Customer activity and engagement
- Revenue performance by city and restaurant
- Customer segmentation (Light / Medium / Hard)
- Average check and product pricing (excluding VAT)
- LTV (Lifetime Value)
- Revenue distribution across restaurants

The goal was to build an interactive analytical dashboard for business decision-making.

---

## Data Sources

The analysis is based on two datasets:

1. **Customers**
   - Registration date
   - Birth date
   - Gender
   - City
   - Loyalty program information

2. **Sales**
   - Transaction ID
   - Restaurant information
   - Product category
   - Product price (incl. VAT)
   - Quantity
   - Transaction date
   - Total check amount

VAT = 18%. All financial metrics were calculated excluding VAT.

---

## Data Modeling

- Star schema model
- Fact table: Sales
- Dimension tables: Customers, Restaurants, Products, Calendar
- Calculated measures built using DAX
- Age calculated at the moment of transaction
- Customer segmentation based on visits per month

---

## Key Metrics

- Unique customers
- Number of transactions
- Average check (excl. VAT)
- Revenue (excl. VAT)
- Average monthly transactions
- Average product price
- LTV
- Revenue share by restaurant

---

## Customer Segmentation Logic

Customers are segmented based on average monthly visits:

- **Light**: < 0.5 visits per month  
- **Medium**: 0.5 – 1.5 visits per month  
- **Hard**: > 1.5 visits per month  

---

## Dashboards Included

1. General Program Overview  
2. Sales Performance by Restaurant  
3. Customer Activity Analysis  
4. Product & Revenue Analysis  

Interactive bookmarks were implemented to switch between:
- Transactions
- Average Check
- Revenue

---


## Key Insights

- **Hard (Heavy) customers are the primary revenue driver.**  
  With an average LTV of ~38,000 ₽ and contributing up to 100% of segment revenue in selected filters, this segment generates a disproportionately large share of total revenue. Retention of this group has a direct impact on profitability stability.

- **Medium customers represent the main scalable growth opportunity.**  
  While their current contribution is lower than Hard customers, transaction dynamics show steady growth, making them the most convertible segment for upsell and loyalty program optimization.

- **Revenue concentration risk is moderate but visible.**  
  Top-10 customers account for **27.3% of total revenue (≈50.9M ₽ out of 186.5M ₽)**, indicating dependency on a relatively small client base.

- **Significant regional performance gap exists.**  
  Revenue varies strongly across cities:
  - Moscow demonstrates the highest average price level (~109.4)
  - Saint Petersburg follows (~93.6)
  - Rostov-on-Don shows the lowest (~54.8)  
  This reflects purchasing power differences and pricing elasticity.

- **Operational imbalance across restaurants.**  
  Some locations show high transaction volumes but below-average check (~1,358 ₽ overall average), suggesting pricing inefficiencies or suboptimal product mix.

- **Sales dynamics indicate accelerating customer acquisition.**  
  New customer growth spikes toward the end of the period, while total revenue reaches **186,534,458 ₽**, confirming positive momentum.

- **Customer behavior is structurally segmented.**  
  LTV and average check vary significantly by engagement level, confirming the necessity of differentiated retention strategies.

### Management Implications

The dashboard enables:

- Early detection of revenue concentration risk  
- Identification of high-LTV customer segments  
- Pricing optimization at city and restaurant level  
- Performance benchmarking across locations  
- Data-driven segmentation and targeted marketing execution 
---


## Tools Used

- Power BI
- Power Query
- DAX
- Data modeling (Star Schema)

---

## Dashboard Preview

(Screenshots are available in the /screenshots folder)

---

## File

The Power BI file (.pbix) is included in the repository.
