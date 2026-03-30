# 📊 CRM Sales Performance Dashboard — Excel

> An interactive, slicer-driven Excel dashboard analyzing **8,800+ B2B sales opportunities** to track quarterly pipeline health, team performance, and revenue insights for sales managers.

---


## Project Overview

This project builds a fully interactive **CRM Sales Performance Dashboard** in Microsoft Excel for a fictitious B2B computer hardware company. The goal was to transform fragmented raw sales pipeline data into a clean, decision-ready reporting tool that sales managers can use to monitor quarterly trends, team productivity, and pipeline health — all within a single Excel workbook.

| Attribute       | Details                                      |
|----------------|----------------------------------------------|
| **Domain**      | Sales Analytics / CRM                       |
| **Tool**        | Microsoft Excel                              |
| **Data Size**   | 8,800 records across multiple tables         |
| **Category**    | Business Intelligence / Dashboarding         |
| **Type**        | Time Series + Cross-sectional Analysis       |

---

## Business Problem

The sales team lacked a centralized, visual way to answer critical questions:

- Which quarters and agents are performing best — and why?
- What percentage of deals are being won, lost, or stalled?
- Which sectors and regions drive the most revenue?
- Where are the pipeline bottlenecks and conversion gaps?

Raw data was spread across multiple CSV tables with missing values, duplicates, and no unified view — making it nearly impossible for managers to act quickly on pipeline signals.

---

## Objectives

| # | Objective |
|---|-----------|
| 1 | **Data Preparation** — Explore, clean, and integrate raw sales pipeline and team data |
| 2 | **Exploratory Analysis** — Use Pivot Tables to uncover quarterly, agent, sector, and regional trends |
| 3 | **Dashboard Design** — Build an interactive, slicer-enabled Excel dashboard for stakeholder reporting |

---

## Dataset

**Source: Maven Analytics Website** Fictitious B2B CRM Sales Dataset (CSV format)

### Files

| File | Description |
|------|-------------|
| `sales_pipeline.csv` | Core table — 8,800 opportunities with deal stages, products, accounts, close dates, and values |
| `sales_teams.csv` | Lookup table — maps each sales agent to their manager and regional office |
| `accounts.csv` | Lookup table — information about companies |
| etc



### Fields Overview in main sales_pipeline.csv

| Field | Description |
|-------|-------------|
| `opportunity_id` | Unique deal identifier |
| `sales_agent` | Agent who owns the deal |
| `product` | Product sold (GTX 500, MG Special, etc.) |
| `account` | Client company name |
| `deal_stage` | Won / Lost / Engaging / Prospecting |
| `close_value` | Revenue closed (USD) |
| `close_date` | Date the deal was closed |
| `manager` | *(Joined from sales_teams)* |
| `regional_office` | *(Joined from sales_teams)* — Central, East, West |
and more

---

## 🛠 Tech Stack & Skills Used

```
Microsoft Excel
├── Data Cleaning         → Remove duplicates, fix nulls, standardize formats
├── VLOOKUP / XLOOKUP     → Join sales_pipeline with sales_teams & accounts table
├── Pivot Tables          → Multi-dimensional analysis (by quarter, agent, sector, region etc)
├── Pivot Charts          → Column, bar, and pie chart visualizations
├── Slicers               → Interactive filters (Product, Manager, Regional Office, Quarter)
├── KPI Cards             → Closed Value, Deals Won, Deals Lost, In-Process, Total Opps
└── Dashboard Layout      → Structured, publication-ready reporting view
```

---

## 🔄 Project Workflow

```
Raw CSV Files
     │
     ▼
1. DATA EXPLORATION
   └── Understand schema, record count, date range, deal stages, products etc
     │
     ▼
2. DATA CLEANING
   └── Remove duplicates → handle nulls → fix data types → standardize categories
     │
     ▼
3. DATA INTEGRATION
   └── VLOOKUP / XLOOKUP → bring Manager + Regional Office into pipeline table
     │
     ▼
4. PIVOT TABLE ANALYSIS
   └── Won/Lost by Quarter → Agent performance → Sector revenue → Office location
     │
     ▼
5. DASHBOARD DESIGN
   └── KPI cards → Charts → Slicers → Formatting → Final layout
     │
     ▼
6. INSIGHT EXTRACTION
   └── Win rate → Top sectors → Regional gaps → Stalled deals → Agent rankings etc
```

---


---

## Key Insights & Findings
- Closed Value of around $10M in all quaters of 2017 with success won rate of 48%.

- From total of 8800 opportunities/deals, 4238 (48%) deals closed successfully while 2473 (28%) deals were lost leaving rest 2089 deals in-process.
- Q1-2017 is a structural collapse — 531 deals only (because of single "March" month closed deals only) vs 1,200+ deals in every other quarter with latest quater (Q4-2017 showing 60% success won rate)
- Retail, Technology, medical, software & finance are leading sectors generating highest revenue in respective order. Finance and Marketing are mid-tier but structurally similar — good for product upsell. While the services, employment & telecommunication need attention
- US office drives 83% of all global deals — while the rest showing 30 to 70 won deals on an average
- Regions & corresponsing Managers show following Won rate:
  
       Central (Manager: Dustin Brinkmann, Melvin Marxen) = 46% won rate among 3512 total opportunities
       East (Manager: Cara Losch, Rocco Neubert) = 51% won rate among 2291 total opportunities
       West (Manager: Celia Rouche, Summer Sewald) = 27% won rate among 2997 total opportunities

- Top 3 Sales agents who lead maximum won deals (>60): Darcel Schlecht (94 highest), Vicki Laflamme (64), Kary Hendrixson (64)
- Bottom 5 Sales agent with least won deals (<22): Garret Kinder (16 Lowest), Rosalina Dieter (21), Rosie Papadopoulos (21)

---


---

## Key Recommendations
- Build a quarterly “best-practice playbook” from top performers.
 Use Darcel Schlecht (highest performer) and other top sales agent to identify what they do differently in discovery, follow-up, and closing.

- Prioritize high-value sectors and replicate winning deal patterns.
  Put more effort into Retail, Technology, medical, software & finance, because they produce the strongest closed values. While also look around other sectors to do better.


- The current win rate is good, but loss rate & in-process rate is still high enough to matter:
    Create a pipeline rescue process for in-process deals i.e., Track stalled deals, aging by stage (how long in that phase), and next-step ownership (call, meeting, follow-up) so the 2,089 in-process opportunities do not go cold.

- Run a region-by-region recovery plan.
    The US is carrying most of the wins, so international offices need focused support, local coaching, and possibly better territory allocation.

- Shift from volume-only reporting to value-based selling.
   Q3 and Q4 show that high wins do not always mean the highest revenue. Push representatives/sales_agent to improve deal size, not only deal count.
  
---


---
## 📸 Screenshots

> **Dashboard Overview (All slicers active)**

![CRM Sales Performance Dashboard](Dashboard%20Screenshot/CRM%20Sales%20Dashboard%20SS%20Excel.png)

*The dashboard updates dynamically when slicers are applied — filter by product, manager, region, or quarter to drill into specific views.*

---

## 🚀 How to Use

1. **Clone or download** this repository
   ```bash
   https://github.com/MushtaqUmar/Excel-CRM-Sales_Performance_Analytics.git
   ```

2. **Open** `CRM Sales Analytics - Excel.xlsx` in Microsoft Excel (2016 or later recommended)

3. **Enable editing** if prompted — required for slicers and pivot tables to function

4. Navigate to the **`Dashboard`** sheet tab

5. Use the **slicers** (top of dashboard) to filter by:
   - `Regional Office` — Central / East / West
   - `Product` — GTX 500, GTX Plus Basic, GTXPro, MG Special, etc.
   - `Manager` — Cara Losch, Dustin Brinkmann, Melvin Marxen, etc.
   - `Quarter` — Q1-2017 through Q4-2017

6. All **charts, KPI cards, and tables update automatically**

> **Note:** Do not modify the `PivotData` or `CleanedData` sheets — they power all dashboard visuals.

---

## 🗂 Project Structure

```
crm-sales-dashboard-excel/
│
├── 📁 Dataset - CRM+Sales+Opportunities/
│   ├── sales_pipeline.csv          # Raw sales pipeline data (8,800 records)
│   └── sales_teams.csv             # Sales team hierarchy lookup table
│   └── accounts.csv             # client company info
│   └── and more

│
├── 📁 screenshots/
│   └── CRM Sales Dashboard SS Excel.png    # Dashboard preview image
│
├── CRM Sales Analytics - Excel.xlsx        # Main Excel workbook (all sheets included)
│
└── README.md                       # Project documentation (this file)
```

---


---

## 👤 Author / Contact</h2>
  - <p><strong>Author:</strong> Umar — Data Analyst & Aspiring Data Scientist</p>
  - <a href="mailto:umarofficial073@gmail.com">Email</a> <br>
  - <a href="https://www.linkedin.com/in/hereumar/">LinkedIn</a> <br>
  - <a href="https://mushtaqumar.github.io/JS-Personal-Portfolio/">Portfolio</a>


---

> ⭐ *If you found this project helpful or insightful, consider giving it a star — it helps others discover it too!*
