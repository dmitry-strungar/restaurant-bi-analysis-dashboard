# Restaurant BI Analysis (Power BI)

Power BI project focused on customer behavior analysis, segmentation, and restaurant performance evaluation for a restaurant chain.

---

## 📌 Project Overview

This project analyzes sales and customer data of a restaurant network to evaluate:

- Customer activity and engagement
- Revenue performance by city and restaurant
- Customer segmentation (Light / Medium / Hard)
- Average check and product pricing (excluding VAT)
- LTV (Lifetime Value)
- Revenue distribution across restaurants

The goal was to build an interactive analytical dashboard for business decision-making.

---

## 🗂 Data Sources

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

## 🧠 Data Modeling

- Star schema model
- Fact table: Sales
- Dimension tables: Customers, Restaurants, Products, Calendar
- Calculated measures built using DAX
- Age calculated at the moment of transaction
- Customer segmentation based on visits per month

---

## 📊 Key Metrics

- Unique customers
- Number of transactions
- Average check (excl. VAT)
- Revenue (excl. VAT)
- Average monthly transactions
- Average product price
- LTV
- Revenue share by restaurant

---

## 👥 Customer Segmentation Logic

Customers are segmented based on average monthly visits:

- **Light**: < 0.5 visits per month  
- **Medium**: 0.5 – 1.5 visits per month  
- **Hard**: > 1.5 visits per month  

---

## 📈 Dashboards Included

1. General Program Overview  
2. Sales Performance by Restaurant  
3. Customer Activity Analysis  
4. Product & Revenue Analysis  

Interactive bookmarks were implemented to switch between:
- Transactions
- Average Check
- Revenue

---

## 🛠 Tools Used

- Power BI
- Power Query
- DAX
- Data modeling (Star Schema)

---

## 📷 Dashboard Preview

(Screenshots are available in the /screenshots folder)

---

## 📁 File

The Power BI file (.pbix) is included in the repository.
