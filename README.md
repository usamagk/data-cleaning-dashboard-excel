# Bike Sales Dashboard (Excel)

## What this is

An interactive dashboard built in Excel to explore who actually buys bikes and why, using a customer dataset with details like income, occupation, commute distance, education, and demographics. The goal wasn't just to make some charts, it was to figure out which customer traits actually relate to a purchase decision, and present that in a way someone could explore themselves.

## The dataset

Customer-level data including:
- Demographics: Gender, Marital Status, Age, Children, Education, Occupation
- Financials: Income, Home Owner status, Cars owned
- Behavior/location: Commute Distance, Region
- Target: Purchased Bike (Yes/No)

## Process

1. **Cleaned the raw data:** fixed data types, handled inconsistent category labels, and checked for missing/blank values before moving on to create pivot tables
2. **Created grouped/binned fields** to make the raw numbers analysis-friendly, Age was grouped into life-stage categories (Early Career, Established Adults, Mature Riders, Midlife) and Income was grouped into brackets (Low, Average, High), since raw numbers are hard to compare visually but grouped categories tell a clearer story
3. **Built pivot tables** as the backbone for each chart, summarizing purchase counts and rates across the different customer attributes
4. **Designed the dashboard layout** with charts, KPI-style visuals, and slicers, so the whole thing updates live as filters are applied instead of static, one-off charts

## Dashboard features

- **Slicers for every major dimension:** Marital Status, Gender, Occupation, Age Group, Region, Income Bracket, Commute, Education, and Home Owner, letting anyone explore the data by any combination of these filters
- **Commute Based Purchase (line chart):** compares bike purchases (Yes vs No) across commute distance categories, from Walkable to Long
- **Career Based Purchase (bar chart):** compares purchase outcomes across age/career groups
- **Average Purchase by Education & Occupation (bar chart):** breaks down average purchase rate by occupation, viewable across education levels

All three charts respond to the slicers simultaneously, so filtering by, say, "Female + High Income + Europe" updates every chart on the dashboard at once.

## Key findings & patterns

- **Commute distance clearly affects purchase behavior.** Customers with a "Moderate" commute showed the highest overall purchase activity of any commute category, both for buyers and non-buyers, while "Long" commutes had the lowest activity overall, suggesting commute length plays a real role in whether a bike fits someone's lifestyle.
- **Life stage matters.** "Early Career" and "Midlife" customers stood out with the most purchase activity overall compared to "Established Adults" and "Mature Riders," hinting that bike purchases lean toward customers at the beginning or later-middle stages of their careers rather than the years in between.
- **Occupation and education together shift purchase averages.** Average purchase rate wasn't flat across occupations, some occupation groups consistently showed a higher average likelihood to purchase than others, even within the same education level, which suggests occupation may be a stronger signal than education alone.
- **No single factor tells the full story on its own**, purchase behavior shifts depending on the combination of commute, career stage, and occupation together, which is exactly why the slicers matter: a static chart would hide these combined effects.

## Tools used
- Microsoft Excel
- data cleaning & transformation
- Pivot Tables & PivotCharts
- Slicers (interactive filtering)

## Files
- `bike_sales_dashboard.xlsx` the full workbook, including raw dataset, Cleaned Dataset, pivot tables, and the Interactive dashboard

## What's next

I'm planning to rebuild this same dashboard in Power BI as a follow-up project, to compare how the same dataset and findings translate into a different BI tool.

---
*Part of my data analytics portfolio, feedback welcome.*
