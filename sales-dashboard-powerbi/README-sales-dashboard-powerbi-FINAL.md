# Sales Dashboard (Power BI)

## Overview
A single-page Power BI report that summarizes sales performance across product categories and over time — built to answer three questions at a glance: which categories sell the most, which are highest-volume, and how does revenue trend month to month.

## File
`sales_dashboard_powerbi.pbix`

## Data Source
An Excel workbook imported into Power BI (`Get Data → Excel workbook`), containing one table, `sales_data`, with the following fields:

- `category` — product category
- `product` — individual product
- `date` — transaction date
- `price` — unit price
- `quantity` — units sold
- `revenue` — total revenue per transaction

## Report Layout
**Page 1 — Sales Dashboard**

- **KPI cards** across the top: No. of Categories, Total Quantities, Total Revenue
- **Revenue by Category** (bar chart) — Electronics leads by a wide margin, followed by Accessories, Clothing, Shoes, and Bags
- **Quantity by Category** (bar chart) — Clothing sells the highest volume of units, even though it doesn't lead in revenue — a sign of a lower price point per unit
- **Revenue by Date** (line chart) — monthly revenue trend across the year, showing the highs and lows month to month

## Key Insights
- **Revenue and unit volume don't move together.** Electronics generates the most revenue ($516,080 — 69% of total) despite Clothing selling the most units (2,281 vs. 1,439 for Electronics). This points to a large price-per-unit gap: Electronics is a lower-volume, higher-price category, while Clothing is higher-volume but lower-price.
- **Revenue is heavily concentrated in one category.** Electronics alone accounts for more revenue than the other four categories (Accessories, Clothing, Shoes, Bags) combined — a useful flag for how exposed total revenue is to a single category's performance.
- **Monthly revenue is fairly stable with a mid-year peak.** Revenue ranges from a low of $53,740 (February) to a high of $67,260 (July), with no single month dramatically outperforming the rest — suggesting demand is fairly steady year-round rather than driven by a seasonal spike.

## Data Modeling & DAX
Three DAX measures power the KPI cards:

```dax
Total_revenue = SUMX('sales_data (2)', 'sales_data (2)'[price] * 'sales_data (2)'[quantity])
```
Calculates revenue per row (price × quantity) and sums across the table — used instead of a static `revenue` column so it recalculates correctly under any filter/slicer context.

```dax
Total_quantities = SUM('sales_data (2)'[quantity])
```
Sums total units sold across all transactions.

```dax
No_of_categories = DISTINCTCOUNT('sales_data (2)'[category])
```
Counts the number of unique product categories in the filtered data.

## Skills Demonstrated
`Power BI` `Data Import & Modeling` `KPI Cards` `Bar & Line Charts` `Sales Trend Analysis`
