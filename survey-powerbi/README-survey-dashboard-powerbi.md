# Data Professionals Career Insights Dashboard (Power BI)

## Overview
A single-page Power BI report analyzing a 630-person survey of data professionals covering salary by country and role, career satisfaction, and preferred tools to understand how pay, happiness, and tech preferences vary across the field.

## File
`Survey_Dashboard.pbix`

## Data Source
A "Data Professional Survey" table with one response per participant, including fields such as:

- `Unique ID` — respondent identifier
- `Average Salary` — reported salary
- `Q1 — Which Title Best Fits your Current Role?` — job title
- `Q5 — Favorite Programming Language`
- `Q6 — How Happy are you in your Current Position with the following?` — split into sub-measures for Salary and Work/Life Balance (rated 0–10)
- `Q9 — Male/Female?` — gender
- `Q10 — Current Age`
- `Q11 — Which Country do you live in?`

## Report Layout
**Page 1 — Data Professionals Career Insights Dashboard**

- **KPI cards**: 630 total participants, average age 29.87
- **Salary Satisfaction gauge**: average rating of 4.27 out of 10
- **Work/Life Balance gauge**: average rating of 5.74 out of 10
- **Average Salary Distribution by Country** (treemap): United States ($77.69K) and Canada ($67.84K) lead, followed by the UK ($46.36K), other countries ($32.05K), and India ($29.91K)
- **Average Salary by Current Role** (bar chart): Data Scientist ($88K) earns the most on average, followed by Data Architect ($64K), Data Engineer ($61K), Data Analyst ($55K), Database Developer ($33K), and Student/Job-seeking ($27K)
- **Participants by Preferred Programming Language** (column chart): Python dominates with 420 respondents, far ahead of R (101) and other languages (95 combined for C/C++, JavaScript, Java)
- **Participants by Gender** (pie chart): 74.29% male, 25.71% female

## Key Insights
- **Salary satisfaction lags behind work/life balance.** Respondents rate their salary satisfaction lower (4.27/10) than their work/life balance (5.74/10) — even though average salaries across roles range from $27K to $88K, suggesting pay satisfaction isn't purely a function of compensation level.
- **Country matters as much as role.** The gap between the highest- and lowest-paying countries in the survey (US at $77.69K vs. India at $29.91K) is roughly as large as the gap between the highest- and lowest-paying roles (Data Scientist at $88K vs. Student/Job-seeking at $27K) — geography is as strong a salary signal as job title.
- **Python is the overwhelming tool of choice.** With 420 of the (visible) respondents naming it their favorite language, Python outpaces every other language combined, reinforcing its position as the default language for data roles.

## Data Modeling & DAX
This report primarily uses Power BI's built-in aggregations (Sum, Average, Count, Distinct Count) directly on survey fields rather than custom DAX measures. *(If you did write any custom measures — e.g. a weighted satisfaction score — add them here the same way as the Sales Dashboard project.)*

## Skills Demonstrated
`Power BI` `Survey Data Analysis` `Treemap & Gauge Visuals` `Cross-Category Comparison` `Dashboard Design`

