# Inventory & Demand Analysis

End-to-end inventory and demand analysis project with a strong focus on **data cleaning**, exploratory analysis, and visualisation using Python.

**Tools:** Python · Pandas · Matplotlib · Seaborn · PostgreSQL

## Project Overview
This project analyses inventory levels and sales demand across multiple stores and items. The raw dataset was messy and required thorough cleaning before any meaningful analysis could be done.

## Data Cleaning Steps Performed
- Removed duplicate records
- Fixed inconsistent date formats and removed invalid dates
- Handled missing values in `sales_qty` and `stock_on_hand`
- Corrected negative values in sales and stock columns
- Created new features: `stock_status` (Healthy / Low Stock / Stockout) and `high_demand` flag

**Final clean dataset:** 1,497 records

## Key Insights
- 89.2% of records showed Healthy stock levels; only 2.4% were stockouts
- STORE01 and STORE03 had the highest number of stockouts
- STORE03 and STORE01 were the top-performing stores by sales
- ITEM161, ITEM198, and ITEM182 were the highest-demand products
- Several items showed overstock risk (high stock + low sales)
- Some fast-moving items had low stock, increasing stockout risk

## Recommendations
- Reduce stock of overstocked low-sales items to free up capital
- Increase safety stock for high-demand items with low inventory
- Monitor STORE01 and STORE03 more closely
- Set clearer reorder points based on sales velocity
- Review slow-moving high-stock items for promotions or reduced ordering

## Dashboard
<img width="1743" height="1252" alt="image" src="https://github.com/user-attachments/assets/9daa8718-c199-45a9-a07d-96bdc6f972ef" />


## Dataset
[Inventory Data](https://www.kaggle.com/datasets/lindviemasongsong/inventory-dataset)
