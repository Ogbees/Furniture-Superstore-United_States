# United States Furniture Superstore Analysis


##  Overview
This project delivers a deep-dive commercial analysis into the **United States Superstore (Furniture Sub category) Dataset** sourced from Kaggle. The dataset moves past standard high-level sales summaries to tie operational supply logistics (ship mode, delivery fulfillment  Duration) and detailed client traits directly to underlying business profitability. 
Using an end-to-end Microsoft Excel pipeline, this project uncovers why high-revenue product lines suffer from compressed profit margins, evaluates geographic performance disparities, and identifies operational improvements to increase profitability.

---

## Tools & Key Features Used
* **Data Engineering & ETL:** Excel Power Query (used for initial schema triage, row filtering, and record normalization).
* **Analytical Engines:** Dynamic Pivot Tables, Custom Calculated Fields, and multi-variable source filters.
* **Executive Visualization:** An interactive Excel Dashboard built with unified theme palettes, Timeline controls, and conditional trend alerts.


## Data Cleaning & Feature Engineering
To maximize spreadsheet performance and ensure reliable analytics, the raw data underwent structured refinement inside Excel:
* **Schema Triage & Column Auditing:** Audited and isolated operational calculation buffer columns (`BLANK`, `AVERAGE`, `PROFIT`, `QUANTITY`) from the raw data to preserve native transactional integrity.
* **Temporal Grouping Flags:** Constructed distinct calendar hooks using `=MONTH()` and `=YEAR()` formulas to smoothly map multi-year growth loops.
* **Text Normalization:** Extracted data and handled text string variance across `Product Name` and `Sub-Category` records by stripping hidden whitespace strings using the `TRIM` and `CLEAN` functions.


##  Insights
* **Sales by Month & Profit Trend:** Sales show clear seasonal spikes, with a massive surge in November and December driven by holiday buying and corporate year-end office setups. However, the profit trend does not always follow the sales spike; heavy promotional discounting during these peak months narrows profit margins, meaning higher sales volume often results in lower overall profitability.
* **Geographic Breakdown:** California and New York dominate total revenue, with cities like New York City and Los Angeles emerging as top-selling hubs. Conversely, states like Texas and Ohio show high sales volume but consistently negative net profits, identifying them as areas where high shipping overhead and steep local price cuts hurt performance.
* **Product Performance (Sales by Categories):** Within the Furniture category, Chairs and Furnishings maintain steady, healthy margins. Tables and Bookcases, despite generating significant revenue, act as major profit drains due to high return rates and expensive bulk shipping costs.
* **Logistics Performance:** "Standard Class" shipping remains the most utilized mode across all transactions. However, analyzing the engineered `Duration` metric reveals that the transit times for Standard Class often exceed acceptable thresholds, leading to a noticeable drop in repeat orders from corporate accounts.


## Strategic Recommendations

### 1. Protect Margins During Seasonal Surges
* **Strategy:** Shift from flat-rate store-wide discounts to targeted, high-margin bundling to stop seasonal revenue from wiping out profits.
* **Actions:**  Replace store-wide "20% off all furniture" winter campaigns with a dynamic "Buy a Desk, Get 15% Off a Chair" bundle.
 Cap maximum automated discounts during November/December at 15% for lower-performing sub-categories like Tables.

### 2. Restructure Pricing in High-Volume, Loss-Making Regions
* **Strategy:** Offset local freight costs and over-discounting in deficit states (e.g., Texas, Ohio) by localizing the pricing model.
* **Actions:**  Create a localized regional shipping surcharge in the pricing matrix to pass heavy freight costs onto bulky furniture orders in those specific states.
 Restrict local sales reps in underperforming zones from matching the aggressive discount tiers used in highly profitable hubs like New York.

### 3. Optimize Low-Margin Product Portfolios
* **Strategy:** Minimize warehouse and logistical overhead on bulky, low-margin products like Tables and Bookcases while scaling high-margin assets.
* **Actions:**  Re-allocate 15% of the digital marketing layout away from Tables/Bookcases and move it toward highly profitable lines like Chairs and Furnishings.
Establish a stricter inspection rule for returning furniture items to lower the high return costs tied to the Bookcase category.

### 4. Optimize Standard Shipping to Improve Customer Retention
* **Strategy:** Streamline the transit times of the high-volume "Standard Class" shipping mode to save corporate retention numbers without spikes in budget overhead.
* **Actions:**  Use the engineered `Duration` metric to identify slow transit routes and switch regional logistics partners for those lanes.
 Establish a regional stocking system to pre-stage high-demand products closer to major hubs like New York City and Los Angeles, shaving 1–2 days off standard deliveries.
 
# Interractive Dashbord
please click the link titled "US_Furniture_Superstore.png" to view the dashboard
