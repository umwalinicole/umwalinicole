# Coffee Orders Analysis (Excel)

## Overview
This project analyzes ~1,000 coffee orders across customers, products, and countries to surface sales trends, top customers, and product performance. The workbook links three related tables (orders, customers, products)  similar to a small relational database and summarizes them into an interactive dashboard.

## File
`coffeeOrdersData_Project.xlsx`

## Dataset
The workbook is organized into a mini data model with three core tables:

| Table | Contents |
|---|---|
| `orders` | ~1,000 individual order line items — order date, customer, product, quantity, coffee type, roast type, size, unit price, and total sales |
| `customers` | Customer master data — name, email, phone, address, city, country, loyalty card status |
| `products` | Product catalog — coffee type, roast type, size, unit price, price per 100g, and profit per unit |

## What's Inside the Workbook

| Sheet | Purpose |
|---|---|
| `orders` | Raw transaction-level data |
| `customers` | Customer reference table |
| `products` | Product reference table with pricing and profit calculations |
| `sales_overtime` | Pivot table/chart of sales trends over time, broken out by coffee type |
| `Country` | Pivot table/chart of total sales by country |
| `Top_Buyer` | Pivot table/chart ranking top customers by total sales |
| `Dashboard` | Combined interactive dashboard (3 charts, slicer) pulling all the above together |

## Process
1. **Data modeling** — structured the data across three linked tables (orders, customers, products) rather than one flat sheet, mirroring how real sales data is stored.
2. **Calculated fields** — computed price-per-100g and profit margin at the product level.
3. **Pivot analysis** — summarized sales over time, by country, and by top customer.
4. **Dashboard** — brought the key visuals together into one filterable view using a slicer.

## Key Questions Explored
- How do sales trend over time, and does it vary by coffee type?
- Which countries generate the most revenue?
- Who are the top customers by total spend?
- Which products are most profitable?

## Skills Demonstrated
`Relational Data Modeling` `Pivot Tables` `Pivot Charts` `Slicers` `Profit/Margin Calculations` `Dashboard Design`

## How to View
Download `coffeeOrdersData_Project.xlsx` and open in Excel.
