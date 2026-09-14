# Bike Buyers Analysis (Excel)

## Overview
This project analyzes a dataset of 1,000+ customer records to understand who buys bikes and why. The workbook takes raw survey-style data, cleans and relabels it, engineers a new feature, and builds an interactive dashboard summarizing purchase behavior across customer segments.

## File
`Bike_Buyers_Project.xlsx`

## Dataset
Each row represents one customer, with the following attributes:

- Demographics: Marital Status, Gender, Age, Income, Children, Education, Occupation
- Household: Home Owner, Number of Cars, Commute Distance, Region
- Target: Purchased Bike (Yes/No)

## What's Inside the Workbook

| Sheet | Purpose |
|---|---|
| `bike_buyers` | Raw source data as originally collected (coded values, e.g. `M`/`F`) |
| `New_worksheet` | Cleaned dataset — coded values relabeled to full text (e.g. `M` → `Married`, `F` → `Female`) and a new **Age Range** column engineered (e.g. "41–55 Middle-Aged") for easier segmentation |
| `Pivot table` | Pivot table summarizing bike purchases (Yes/No) across customer attributes |
| `Dashboard` | Interactive summary dashboard with 4 charts and 3 slicers for filtering by segment |

## Process
1. **Data cleaning** — standardized coded fields into readable labels and checked for inconsistencies.
2. **Feature engineering** — bucketed continuous `Age` into readable age-range groups to make segmentation easier to read and visualize.
3. **Analysis** — built pivot tables to break down bike purchase rates by demographic and lifestyle attributes (income, occupation, marital status, region, commute distance, etc.).
4. **Dashboard** — combined the pivot outputs into a single-page dashboard with charts and slicers so the data can be explored interactively without editing formulas.

## Key Questions Explored
- Which demographic groups are most likely to purchase a bike?
- Does income, commute distance, or number of cars owned relate to bike ownership?
- How does purchase behavior differ by region?

## Skills Demonstrated
`Data Cleaning` `Pivot Tables` `Pivot Charts` `Slicers` `Feature Engineering` `Dashboard Design`

