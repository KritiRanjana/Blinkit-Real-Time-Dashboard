# Blinkit Sales Analytics Dashboard

**Tools:** Power BI | DAX | Power Query | Microsoft Excel 
---

## Overview

This project is an interactive sales analytics dashboard built in Power BI for **Blinkit — India's Last Minute Delivery App**. It analyzes grocery retail performance across store formats, city tiers, and product categories using real transactional data spanning 2011 to 2022.

The dashboard helps answer key business questions around revenue distribution, product performance, and outlet efficiency — turning raw data into clear, actionable insights.

**Dataset:** 8,523 records | 12 columns | 2011–2022

---

## Problem Statement

Blinkit operates multiple outlet formats (Grocery Stores, Supermarket Type 1/2/3) across Tier 1, 2, and 3 cities in India. With a wide product range and a growing store network, the business needed a centralized view to answer:

- Which city tiers and store formats generate the most revenue?
- Which product categories are driving or dragging overall sales?
- How has sales performance trended since the first outlet opened?
- Where should resources be focused to improve outlet efficiency?

---

## Key Metrics

| Metric | Value |
|--------|-------|
| Total Sales | **$1.20M** |
| Average Sales per Item | **$141** |
| Total Items Tracked | **8,523** |
| Average Customer Rating | **3.9 / 5** |

---

## Key Findings

**Tier 3 cities outperform larger markets**
Outlets in Tier 3 cities generated $472K in revenue, ahead of Tier 2 ($393K) and Tier 1 ($336K). This points to strong untapped demand in smaller cities and makes a case for prioritizing expansion there.

**A handful of categories drive most sales**
Fruits & Vegetables ($178K), Snack Foods ($175K), and Household items ($136K) together account for nearly 40% of total revenue. At the other end, Seafood ($9K) and Breakfast items ($15K) contribute minimally and may need a stocking strategy review.

**Supermarket Type 1 dominates revenue**
Supermarket Type 1 outlets contribute $787K — 65% of total sales — with the highest item count (5,577). This makes them the most critical store format and a priority for operational investment.

**Sales growth has plateaued post-2018**
Revenue peaked at $205K in 2018 as new outlets were being rapidly established, then declined to $131K by 2022. This suggests that scaling through new store openings alone is not sufficient — optimizing existing outlets is equally important.

**Regular fat products lead by a wide margin**
Regular fat content items ($776K) outsell Low Fat products ($425K) by nearly 2:1, which has direct implications for inventory planning and targeted health-segment promotions.

---

## How It Was Built

**Data Cleaning — Power Query**
- Resolved inconsistent fat content labels (e.g. `LF`, `low fat` → `Low Fat`)
- Handled missing values in `Item Weight` and `Outlet Size` columns
- Created supporting columns for outlet age and sales groupings

**Calculations — DAX**
```dax
Total Sales  = SUM('BlinkIT Data'[Sales])
Avg Sales    = AVERAGE('BlinkIT Data'[Sales])
No. of Items = COUNTROWS('BlinkIT Data')
Avg Rating   = AVERAGE('BlinkIT Data'[Rating])
```

**Dashboard Design — Power BI**
- Filter panel to slice data by outlet location, size, and item type
- Metric toggle tabs to switch all visuals between Total Sales, Avg Sales, Item Count, and Rating
- Custom tooltips on product bar chart showing item-level detail on hover
- Conditional formatting on the outlet comparison table for quick performance scanning
- Area chart tracking outlet establishment and sales trends from 2011 to 2022

---

## About Me

I am a fresher Data Analyst with hands-on experience in Power BI, Excel, and DAX. I enjoy working with real business data to find patterns that drive decisions — not just building visuals, but asking the right questions behind them.

📧 kritiranjana03@gmail.com &nbsp;|&nbsp; 💼 [LinkedIn](www.linkedin.com/in/kritiranjana03-833b15226) 
*Open to Data Analyst and Business Intelligence opportunities — feel free to connect.*
