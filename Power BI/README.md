# Power BI Dashboard — Restaurant Performance Overview

## Overview
This Power BI dashboard synthesizes exploratory SQL and Python analysis into an interactive, executive-level visual summary. It is designed to provide rapid data-driven answers to core operational questions.  
The goal is to quickly answer:

- How busy is the restaurant?
- When are peak demand hours?
- Which menu items and categories drive revenue?
- How concentrated is revenue across the menu?

---

## Key KPIs
The dashboard opens with four headline metrics that define the scale of operations:

- **Total Orders:** 5,343  
- **Total Revenue:** 159.22K  
- **Total Items Ordered:** 12K  
- **Average Items per Order:** 2.26  

These KPIs provide immediate context before deeper exploration.

---
## Dashboard Preview
![Restaurant Performance Dashboard](Power%20Bi_dashboard.png) 

---

## Dashboard Visuals

### 1. Total Orders by Category
A donut chart showing order distribution across cuisines:
- Italian, Asian, Mexican, and American categories are well-balanced.
- Italian slightly leads in revenue contribution, driven by higher average item prices.

---

### 2. Order Volume by Hour of Day
A column chart highlighting demand patterns:
- Clear lunch peak between **12–2 PM**
- Strong dinner rush between **6–8 PM**
- Late-night demand drops significantly after 9 PM

---

### 3. Revenue Spikes by Hour
An area chart visualizing revenue trends:
- Revenue closely mirrors order volume
- Lunch and dinner periods generate the highest revenue concentration
- Confirms staffing and inventory should be optimized around peak hours

---

### 4. Top Revenue-Generating Menu Items
A horizontal bar chart showing revenue concentration:
- A small set of items (e.g. Korean Beef Bowl, Spaghetti & Meatballs) generate a disproportionate share of revenue
- Indicates opportunities for promotion, bundling, and pricing optimization

---

## Interactivity
- **Category slicer** allows users to explore performance by cuisine
- Cross-filtering enables drill-down into how a single category impacts:
  - Revenue
  - Peak hours
  - Top-performing items

---

## Key Takeaways
- Revenue is highly concentrated in a small number of popular menu items
- Lunch and dinner periods dominate demand and revenue generation
- Italian cuisine leads revenue despite Asian having higher item volume, due to higher average prices
- The dashboard provides a fast, intuitive operational overview suitable for decision-makers

---

## Tools Used
- Power BI Desktop
- DAX measures for KPIs and aggregations
- SQLite / CSV data source from prior analysis

---

