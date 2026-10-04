# Superstore Sales & Profit Analytics
### RLS-Enabled Regional Performance Dashboard | Power BI Capstone Project

A full end-to-end Power BI project built on the Indian Superstore retail dataset — from raw data cleaning through a secured, interactive dashboard, Row-Level Security (static + dynamic), drill-through, custom tooltips, and a client-ready presentation.

---

## Project Overview

A retail organization selling technology and office supplies across India needed a secure, self-service way for Regional Managers to monitor sales, profit, customer behavior, and shipping performance — with each manager seeing only their own region’s data.

**This project delivers:**
- Cleaned & modeled dataset (51,284 orders) with star schema
- 16+ DAX measures (YoY, RFM, Ranking)
- 4 interactive report pages + Customer Profile + Region Profile + Tooltips
- Static RLS (5 regional roles) + Dynamic RLS (USERPRINCIPALNAME)
- Full documentation and client-style presentation

---

## Dashboard Pages

| Page | What it shows |
|------|---------------|
| Sales Overview | KPIs with YoY, category breakdown, map, monthly trend, top products |
| Customer Insights | RFM scatter, Key Influencers, top customers, drill-through |
| Product & Discount Impact | Discount vs Profit scatter, product ranking, delivery analysis |
| Region & Manager View | Region → State → City drill-down, regional comparison |
| Customer Profile | Drill-through deep dive for individual customers |
| Region Profile | Drill-through deep dive for individual regions |
| Product Tooltip | Hover-level product sales, profit & rank |
| Customer Tooltip | Hover-level customer detail |

---

## Key Insights

- Sales +49.12% YoY | Profit +47.89% YoY | Margin 11.61%
- Technology is the top-performing category
- North region leads; Central underperforms consistently
- Discounts above 9% concentrated in loss-making SKUs
- “Tables – India” is the largest margin drag (₹6.28 Cr sales → ₹53.2 L loss)
- Standard Class shipping is the strongest profit driver
- Top customers contribute disproportionately higher revenue

---

## Recommendations

1. Cap discounts at 5–7% only on historically loss-making SKUs
2. Launch a 90-day Central region recovery plan (benchmark North)
3. Deploy loyalty program for Top 20 high-value customers
4. Align inventory & promotions with Q4 festive demand
5. Prefer Standard Class shipping on margin-sensitive orders

---

## Row-Level Security

| Type | Implementation |
|------|----------------|
| Static RLS | 5 roles (North, South, East, West, Central) |
| Dynamic RLS | Single role using USERPRINCIPALNAME() mapped via Users table |

Both verified using **View As** in Power BI Desktop.

---

## Deliverable Items

| File | Description |
|------|-------------|
| Superstore_RLS_Regional_Analytics.pbix | Full Power BI report |
| Dashboard_Screenshots.pdf | Screenshots of all pages |
| Final_Insight_Summary.pdf | Business insights & recommendations |
| Presentation.pptx | Client-style project presentation |

---

## How to Explore

1. Download the `.pbix` file and open in **Power BI Desktop**
2. Use navigation buttons or bookmarks to move between pages
3. Right-click any customer → Drill through → Customer Profile
4. Right-click any region → Drill through → Region Profile
5. Hover on products for custom tooltips
6. Test RLS: **Modeling → View as → select a regional role**

---

## Tools & Techniques

Power BI Desktop · Power Query · DAX · Star Schema · Row-Level Security (Static + Dynamic) · Bookmarks · Drill-through · Custom Tooltips

---

## Author

**Bhargav Bolisetti**  
Power BI Capstone Project | October 2026
