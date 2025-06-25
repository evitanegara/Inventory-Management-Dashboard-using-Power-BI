# Inventory Management Dashboard using Power BI

## Project Overview
This project analyzes product-level inventory data to help inventory and procurement teams maintain stock availability, minimize stockouts, and improve restocking efficiency. Built in Power BI, the dashboard transforms raw inventory data into clear, actionable insights using visual KPIs and trend-based reporting. The goal of the dashboard is to support smarter inventory decisions by highlighting where stock levels fall below thresholds, identifying which suppliers perform best on lead times, and revealing how inventory is distributed across regions. This enables businesses to reduce fulfillment delays, better allocate warehouse resources, and ensure that high-demand products remain available when needed.

## Dataset Overview
The dataset includes the following fields:

| Column               | Description                                         |
|----------------------|-----------------------------------------------------|
| Product_ID           | Unique identifier for the product                   |
| Product_Name         | Name of the product                                 |
| Category             | Product category (Books, Electronics, etc.)         |
| Unit_Price           | Price per unit                                      |
| Stock_Quantity       | Number of units currently in stock                  |
| Stock_Level          | Categorical stock level (Low, Medium, High)         |
| Reorder_Point        | Threshold to trigger restocking                     |
| Lead_Time_Days       | Supplier delivery time in days                      |
| Last_Restock_Date    | Last restocking date                                |
| Supplier_ID          | Unique ID for each supplier                         |
| Warehouse_Location   | City of warehouse                                   |
| Min_Order_Quantity   | Minimum quantity for reordering                     |
| Status               | Product status (Active or Discontinued)             |
| Entry_Date           | When product was added to the system                |
| Country              | Warehouse country                                   |
| Latitude / Longitude | Geo-coordinates of the warehouse                    |

## Executive Summary
# This inventory analysis reveals key patterns across product categories, suppliers, and warehouse locations. Books, Home & Garden, and Office Supplies have the highest stock quantities, but Home & Garden also records the most stockouts, suggesting gaps in replenishment. Most categories maintain healthy reorder compliance, though Books and Office Supplies frequently fall below threshold levels, indicating the need for closer monitoring. Inventory is concentrated in Germany, Belgium, and Spain, while France holds fewer units and SKUs, which may limit local fulfillment capabilities. Supplier performance is mostly consistent, with SUP018, SUP016, and SUP030 delivering the fastest lead times. SUP041, on the other hand, shows recurring delays, especially in Books and Toys. Restocking trends are volatile throughout the year, peaking in January and May, and dropping sharply in February and August. These insights support targeted improvements in restocking, supplier selection, and warehouse distribution to maintain inventory balance and service levels.
---

## Insights Deep-Dive
### Inventory Stock Distribution by Category
- Inventory is well-distributed across all categories, with strong stock levels maintained in most segments.
- Books, Office Supplies, and Home & Garden lead in available quantity, holding 318K, 300K, and 313K units respectively.
- The highest stockout volumes are seen in Home & Garden (68K), Office Supplies (67K), and Clothing (58K), pointing to possible supply chain gaps or demand surges.
- Sports and Toys have the lowest out-of-stock counts, with 46K and 50K units respectively.

### Reorder Point Compliance
- Most SKUs are above reorder levels, ensuring availability.
- Books (47 SKUs) and Office Supplies (44 SKUs) are most often below reorder thresholds.
- Electronics and Clothing are compliant but should still be monitored.

### Restocking Volume by Category
- Books require the highest restocking volume at 2,038 units, indicating frequent turnover or strong demand.
- Office Supplies follow closely with 1,717 units, and Clothing ranks third with 1,514 units.
- Toys have the lowest restock requirement at 1,126 units. 

### Country-Wise Inventory Distribution
- Germany holds the most stock (276K units, 533 SKUs), positioning it as the most heavily stocked location.
- elgium and Spain each manage over 260,000 units, placing them among the top three locations by inventory volume.
- France holds the fewest SKUs (470) and lowest stock volume (223K units).

### Inventory Turnover & Lead Time Efficiency
- Home & Garden (25.26K), Books (25.03K), and Sports (24.57K) show the highest turnover, reflecting strong product movement.
- Office Supplies and Clothing maintain steady turnover levels around 24K, indicating consistent sales flow.
- Electronics has the lowest turnover at 21.63K.
- Overall turnover is relatively balanced across all categories.

### Supplier Lead Time Analysis
- Supplier lead times range from 15.7 to 17.3 days, showing overall consistent performance.
- SUP018, SUP016, and SUP030 are the fastest suppliers, each averaging 15.7 days—suitable for time-sensitive or fast-moving products.
- SUP041 is the slowest, with an average lead time of 17.3 days and delays up to 20 days in Books and Toys, which may impact stock availability.
- SUP023 and SUP040 show the most consistent performance across all categories, maintaining lead times between 13 and 18 days.

### Monthly Restocking Trends

- Restocking activity fluctuates throughout the year, with clear peaks and dips.
- High-volume months include January, May, June, September, and November, each exceeding 863 units.
- February (590 units) and August (689 units) mark the lowest restocking periods, suggesting seasonal slowdowns or planning gaps.
- The January spike was led by Office Supplies (284), Clothing (197), and Sports (146)—likely due to post-holiday demand and new-year planning.
- February dropped sharply, especially in Clothing (13 units) and Office Supplies (77 units), while Home & Garden unexpectedly rose to 174 units.
- December closed the year slightly above average, supported by strong restocking in Sports (244) and Books (139), possibly in preparation for year-end demand or Q1 sales.
---

## Recommendations

### Procurement & Replenishment
- Prioritize Books, Office Supplies, and Clothing for restocking.
- Monitor SKUs that regularly fall below reorder point.
- Assign fast-moving SKUs to fast suppliers (SUP018, SUP016, SUP030).

### Warehouse Optimization
- Stock high-demand products in top hubs: Germany, Belgium, and Spain.
- Rebalance stock levels in France to improve product availability.

### Supplier Management
- Reduce reliance on SUP041 due to delays.
- Increase orders with SUP023 and SUP040 for consistent performance.

### Seasonal Planning
- Prepare for restocking spikes in January and Q2.
- Improve forecasting in February and August to avoid stock shortages.

---

## Contact

For questions or collaboration, contact **evitanegara@gmail.com**
