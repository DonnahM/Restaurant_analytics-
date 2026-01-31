## Restaurant Performance & Menu Optimization

### Project Overview
This project analyzes a quarter’s worth of transactional order data from a fictitious restaurant serving international cuisine. The objective is to evaluate menu performance, revenue drivers, and operational efficiency, and to translate transaction-level data into clear, business-relevant insights.

The analysis focuses on identifying high- and low-performing menu items, understanding revenue concentration, examining customer purchasing behavior, and uncovering temporal demand patterns that can inform menu optimization and staffing decisions.

---

### Business Problem
Restaurants often face margin pressure caused by menu bloat, inefficient staffing, and a misalignment between customer demand and operational resources. Without data-driven insights, menu and staffing decisions are frequently guided by intuition rather than evidence.

This analysis seeks to answer:
- Which menu items and categories truly drive revenue?
- Where is revenue overly concentrated or underutilized?
- How does customer demand fluctuate throughout the day?
- How can menu and staffing decisions be optimized to improve profitability?

---

### Data Overview
The dataset used in this project is sourced from the [Maven Analytics Restaurant Orders Dataset](https://mavenanalytics.io/data-playground/restaurant-orders), representing a fictitious restaurant and designed for analytical practice.

It consists of three tables:
- **order_details**: Transaction-level order records including order ID, date, time, and item ID  
- **menu_items**: Menu metadata including item name, category, and price  
- **order_analysis (view)**: A derived analytical view joining orders and menu data with calculated revenue and standardized time fields  

Records with missing `item_id` values were excluded from analytical views to ensure accurate item-level revenue analysis, while remaining available in the raw tables for auditability.

---
## 📊 Executive Dashboard Preview
*Quickly visualize the restaurant's performance at a glance.*

![Dashboard Screenshot](./Power%20BI/Power%20Bi_dashboard.png) 

> **Full Analysis:** For a deep dive into the KPIs and visual breakdowns, check out the [Power BI Dashboard Documentation](./Power%20BI/)

---

### Methodology
SQLite was used as the primary analytical engine, with SQL views created to centralize transformations and calculations. Python (pandas) was used to execute SQL queries and present results in tabular form within a Jupyter Notebook.

The analysis emphasizes business interpretation over descriptive statistics, focusing on menu performance, category contribution, revenue concentration, order-level behavior, and temporal demand trends.

---

### Key Insights
- Revenue is highly concentrated among a small subset of menu items, with the Korean Beef Bowl emerging as the single highest revenue contributor.

- Italian cuisine dominates total revenue (31.07%), driven by higher average item prices rather than volume alone.

- Asian cuisine generates comparable revenue (29.34%), supported by higher order frequency but lower average prices.

- Several items show high order frequency but low revenue contribution, indicating potential pricing or portioning inefficiencies.

- A small number of high-value orders contribute a disproportionate share of total revenue.

- Demand peaks occur during midday and early evening hours, aligning with lunch and dinner service windows.

---

### Conclusion
This analysis demonstrates that restaurant revenue is driven primarily by a focused set of high-performing menu items and predictable time-based demand patterns. Italian and Asian cuisines emerge as the strongest contributors to overall performance, supported by customer preference for variety within individual orders. By optimizing the menu around top performers, refining underperforming offerings, and aligning operations with peak demand periods, the restaurant can improve both revenue efficiency and customer satisfaction.

---

### Recommendations

**Protect the Stars:** Prioritize marketing and inventory for top-tier Italian and Asian dishes.

**Implement Bundling:** Create curated lunch/dinner meal bundles to increase the Average Order Value (AOV) during peak hours.

**Menu Pruning:** Review items with low sales and low revenue for removal to reduce operational complexity.

**Shift-Based Staffing:** Align labor hours strictly with the identified lunch and dinner peaks to maximize margin.

---


