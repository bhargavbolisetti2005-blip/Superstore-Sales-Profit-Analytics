# Superstore Sales & Profit Analytics
### RLS-Enabled Regional Performance Dashboard | Power BI Capstone Project

---

## Project Overview

This is a complete end-to-end Power BI solution built on the **Indian Superstore** retail dataset. The goal was to transform raw transactional data into a secure, interactive analytics platform that enables Regional Managers to monitor sales, profit, customer behaviour, and shipping performance — while ensuring each manager can access **only their own region’s data**.

**What this project delivers:**
- Fully cleaned and modelled dataset (51,284 orders)
- Star-schema data model with 16+ production-grade DAX measures
- Four analytical report pages + Customer Profile + Region Profile + custom tooltips
- Static Row-Level Security (5 regional roles) and Dynamic RLS using `USERPRINCIPALNAME()`
- Client-ready presentation, insight summary, and complete documentation

---

## Business Context

A retail organisation selling Technology and Office Supplies across India required:
- A single decision-ready view of sales, profit, customers, and shipping
- Secure region-wise visibility for Regional Managers
- The ability to move from raw data to actionable insights

This project closes that gap.

---

## Dashboard Pages

| Page | Purpose |
|------|---------|
| **Sales Overview** | KPI cards with YoY indicators, category performance, monthly sales & profit trend, state-level map, top products |
| **Customer Insights** | RFM segmentation, AI Key Influencers, top customers table, Region vs Customer Sales |
| **Product & Discount Impact** | Discount % vs Profit scatter (size = sales, colour = profit/loss), product ranking, delivery-time analysis |
| **Region & Manager View** | Region → State → City hierarchy, regional profit comparison, monthly trend by region |
| **Customer Profile** | Drill-through page with full order history and KPIs for an individual customer |
| **Region Profile** | Drill-through page with regional deep-dive (sales, profit, state contribution) |
| **Product Tooltip** | Hover page showing live Sales, Profit, Rank and Discount % |
| **Customer Tooltip** | Hover page showing customer-level summary metrics |

---

## Key Business Insights

- **Sales** grew **+49.12% YoY** and **Profit +47.89% YoY**, with overall margin at **11.61%**
- **Technology** is the clear category leader (₹0.39 Bn)
- **North** region consistently leads and serves as the internal benchmark
- **Central** region underperforms across the full year — a structural gap, not seasonal
- Discounts above **9%** are heavily concentrated in loss-making products
- **“Tables – India”** is the single largest margin drag (₹6.28 Cr sales → ₹53.2 L loss)
- Delivery time is stable (15–16 days) — logistics is not the primary issue
- A small group of high-value customers drives disproportionate revenue
- **Standard Class** shipping is the strongest driver of higher profit

---

## Strategic Recommendations

1. **Discount Discipline** — Cap discounts at 5–7% **only** on historically loss-making SKUs (e.g. Tables – India)
2. **Central Region Recovery** — Launch a 90-day structured recovery plan using North as the benchmark
3. **Customer Retention** — Deploy a targeted loyalty programme for the Top 20 revenue-contributing customers
4. **Seasonal Planning** — Align inventory and promotions with the proven Q4 (Nov–Dec) demand spike
5. **Shipping Optimisation** — Prefer Standard Class on margin-sensitive orders

---

## Technical Implementation

| Area | Details |
|------|---------|
| **Data Model** | Star schema — Orders (Fact) + Date, Zone, Users (Dimensions) |
| **Measures** | 16+ DAX measures including YoY growth, RFM metrics, RANKX, Profit % |
| **RLS – Static** | 5 roles (North, South, East, West, Central) filtering by Region |
| **RLS – Dynamic** | Single role using `USERPRINCIPALNAME()` mapped via Users table |
| **Interactivity** | Bookmarks, page navigation buttons, drill-through, custom tooltips |
| **Verification** | All RLS roles tested using **View As** in Power BI Desktop |

---

## Data Preparation Highlights

- Corrected data types and removed duplicates / blank critical fields
- Removed Postal Code column (100% null)
- Created calculated **Delivery Days** column
- Identified and removed 6 records with invalid 29-Feb-2012 dates that were corrupting the Year slicer
- Built continuous Date table for accurate time intelligence

---

## Deliverable Items

| File | Description |
|------|-------------|
| `Superstore_RLS_Regional_Analytics.pbix` | Complete Power BI report (model, measures, all pages) |
| `Indian_Superstore_Dataset.xlsx` | Source dataset used for the project |
| `Dashboard_Screenshots.pdf` | High-quality screenshots of all dashboard pages |
| `Final_Insight_Summary.pdf` | Business-facing insights, recommendations and impact |
| `README.md` | Project documentation |

---

## How to Explore the Dashboard

1. Download `Superstore_RLS_Regional_Analytics.pbix` and open it in **Power BI Desktop**
2. Use the on-page navigation buttons or bookmarks to move between pages
3. Right-click any **customer** → Drill through → **Customer Profile**
4. Right-click any **region** → Drill through → **Region Profile**
5. Hover over products to see the custom **Product Tooltip**
6. Test security: **Modeling → View as →** select a regional role or Dynamic Access role

---

## Tools & Techniques

- Power BI Desktop  
- Power Query (M)  
- DAX (Time Intelligence, RFM, RANKX, ALLEXCEPT)  
- Star-schema modelling  
- Row-Level Security (Static + Dynamic)  
- Bookmarks & Navigation  
- Drill-through pages  
- Custom Tooltip pages  

---

## Author

**Bhargav Bolisetti**  
Power BI Capstone Project  
October 2026

---
