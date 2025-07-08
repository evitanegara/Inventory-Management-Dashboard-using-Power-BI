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

This inventory analysis uncovers patterns across products, suppliers, and warehouse locations. While Books, Home & Garden, and Office Supplies have high stock availability, Home & Garden also leads in stockouts, highlighting gaps in replenishment. Books and Office Supplies frequently fall below reorder points, suggesting the need for closer monitoring. Inventory is mostly concentrated in Germany, Belgium, and Spain, while France holds fewer SKUs and units, which may impact local fulfillment. Supplier performance is generally stable, with SUP018, SUP016, and SUP030 offering the fastest lead times. In contrast, SUP041 shows repeated delays, especially in Books and Toys. Restocking activity varies throughout the year, peaking in January and May, but dropping in February and August. These insights support improvements in restocking schedules, supplier selection, and warehouse planning to maintain balanced inventory and service levels.

---

## Visualization
<p align="center">
  <img src="https://github.com/user-attachments/assets/ed57c6a5-71a6-41ce-8141-8b9e7ddb9cf2" alt="Inventory Dashboard Page 1" width="700"/>
</p>
<p align="center">
  <img src="https://github.com/user-attachments/assets/66af4abc-0f9c-4ddf-8269-3b59b7874cc7" alt="Inventory Dashboard Overview" width="700"/>
</p>






## Insights Deep-Dive
### Inventory Stock Distribution by Category
- Inventory is well-distributed across all categories, with strong stock levels maintained in most segments.
- Books, Office Supplies, and Home & Garden lead in available quantity, holding 318K, 300K, and 313K units respectively.
- The highest stockout volumes are seen in Home & Garden (68K), Office Supplies (67K), and Clothing (58K), pointing to possible supply chain gaps or demand surges.
- Sports and Toys have the lowest out-of-stock counts, with 46K and 50K units respectively.
  <p align="center">
  <img src="https://github.com/user-attachments/assets/db53edfd-00f7-47b4-b551-df270b33e8d7" alt="Inventory Dashboard - Supplier Performance Page" width="700"/>
</p>



### Reorder Point Compliance
- Most SKUs are above reorder levels, ensuring availability.
- Books (47 SKUs) and Office Supplies (44 SKUs) are most often below reorder thresholds.
- Electronics and Clothing are compliant but should still be monitored.
<p align="center">
  <img src="https://github.com/user-attachments/assets/cfe7bdd1-94d4-41ab-8726-071266e3990c" alt="Inventory Overview Dashboard" width="700"/>
</p>

### Restocking Volume by Category
- Books require the highest restocking volume at 2,038 units, indicating frequent turnover or strong demand.
- Office Supplies follow closely with 1,717 units, and Clothing ranks third with 1,514 units.
- Toys have the lowest restock requirement at 1,126 units.
<p align="center">
  <img src="https://github.com/user-attachments/assets/61ff1913-3caf-434f-9eb5-ba5265878db9" alt="Reorder Point Compliance Chart" width="700"/>
</p>


### Country-Wise Inventory Distribution
- Germany holds the most stock (276K units, 533 SKUs), positioning it as the most heavily stocked location.
- elgium and Spain each manage over 260,000 units, placing them among the top three locations by inventory volume.
- France holds the fewest SKUs (470) and lowest stock volume (223K units).
<p align="center">
  <img src="https://github.com/user-attachments/assets/c5fdd357-625f-40ec-b251-7ab85d951abd" alt="Restocking Volume by Category" width="700"/>
</p>


### Inventory Turnover & Lead Time Efficiency
- Home & Garden (25.26K), Books (25.03K), and Sports (24.57K) show the highest turnover, reflecting strong product movement.
- Office Supplies and Clothing maintain steady turnover levels around 24K, indicating consistent sales flow.
- Electronics has the lowest turnover at 21.63K.
- Overall turnover is relatively balanced across all categories.
<p align="center">
  <img src="https://github.com/user-attachments/assets/13f14e3c-903a-4a10-b699-f56d8fba1653" alt="Stock by Country" width="700"/>
</p>


### Supplier Lead Time Analysis
- Supplier lead times range from 15.7 to 17.3 days, showing overall consistent performance.
- SUP018, SUP016, and SUP030 are the fastest suppliers, each averaging 15.7 days—suitable for time-sensitive or fast-moving products.
- SUP041 is the slowest, with an average lead time of 17.3 days and delays up to 20 days in Books and Toys, which may impact stock availability.
- SUP023 and SUP040 show the most consistent performance across all categories, maintaining lead times between 13 and 18 days.
<p align="center">
  <img src="https://github.com/user-attachments/assets/d45417c3-d9f0-4e30-ab63-5dc242c3c977" alt="Restock Requirement Summary Table" width="700"/>
</p>

<p align="center">
  <img src="https://github.com/user-attachments/assets/e9c6e4c5-01b0-4d6e-9981-910c09d2227a" alt="Product Above vs Below Reorder Point" width="700"/>
</p>


### Monthly Restocking Trends

- Restocking activity fluctuates throughout the year, with clear peaks and dips.
- High-volume months include January, May, June, September, and November, each exceeding 863 units.
- February (590 units) and August (689 units) mark the lowest restocking periods, suggesting seasonal slowdowns or planning gaps.
- The January spike was led by Office Supplies (284), Clothing (197), and Sports (146)—likely due to post-holiday demand and new-year planning.
- February dropped sharply, especially in Clothing (13 units) and Office Supplies (77 units), while Home & Garden unexpectedly rose to 174 units.
- December closed the year slightly above average, supported by strong restocking in Sports (244) and Books (139), possibly in preparation for year-end demand or Q1 sales.
<p align="center">
  <img src="https://github.com/user-attachments/assets/a8bd5c34-2322-42a4-9a21-abff0080d9b7" alt="Monthly Restock Trend" width="700"/>
</p>

---

## Recommendations

### Procurement & Replenishment
- Prioritize restocking for Books, Office Supplies, and Clothing , these categories consistently show high restock volume needs (2,038; 1,717; and 1,514 units respectively) and the largest number of SKUs falling below reorder thresholds. This signals strong demand and replenishment gaps that risk future stockouts.
- Monitor Books (47 SKUs) and Office Supplies (44 SKUs) more closely to prevent availability issues and missed sales opportunities.
- Assign fast-moving SKUs to reliable suppliers like SUP018, SUP016, and SUP030 to reduce lead time delays and ensure timely restocking.

### Warehouse Optimization
- Stock high-demand products in top-performing hubs like Germany, Belgium, and Spain, which currently hold the highest inventory volumes and product counts. These locations serve as major distribution centers and can handle demand efficiently.
- Reassess and rebalance inventory levels in France, which holds the lowest product variety (470 SKUs) and stock volume. Enhancing its inventory can improve regional fulfillment and reduce delivery time for local demand.
  
### Supplier Management
- Reduce dependency on SUP041, which shows the slowest lead times and repeated delays.
- Increase allocation to reliable suppliers such as SUP023 and SUP040, who demonstrate consistent delivery performance across all categories, helping maintain steady inventory flow.

### Seasonal Planning
- Strengthen restocking efforts ahead of January and Q2, when demand and replenishment activity consistently peak—likely driven by post-holiday recovery and seasonal inventory cycles.
- Implement machine learning based forecasting models to better anticipate restocking needs in February and August, which currently show the lowest restock volumes. These models can help identify hidden demand patterns and reduce the risk of understocking during slower or irregular seasons.
---

## Contact

For questions or collaboration, contact **evitanegara@gmail.com**
