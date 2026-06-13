# Tobacco Enterprise Analytics Dashboard

### Production & Sales Efficiency — Power BI Analytics

> Sales Performance, Production Efficiency & Target Achievement Analysis using Power BI

---

## Skills & Tools

**Power BI &nbsp;•&nbsp; DAX &nbsp;•&nbsp; Power Query &nbsp;•&nbsp; Data Modeling &nbsp;•&nbsp; Star Schema &nbsp;•&nbsp; KPI Development &nbsp;•&nbsp; Sales Analytics &nbsp;•&nbsp; Manufacturing Analytics &nbsp;•&nbsp; Business Intelligence &nbsp;•&nbsp; Data Visualization**

---

## Project Overview

This project analyzes sales performance, production efficiency, and target achievement for a tobacco manufacturing company using Power BI. The objective was to create a centralized analytics solution that enables management to monitor business performance, identify operational inefficiencies, and support data-driven decision-making.

The dashboard consolidates sales, production, distributor, and target data into a single reporting platform, providing real-time visibility into revenue growth, quality performance, production losses, and business targets.

---

## Business Problem

The organization lacked a centralized reporting solution to monitor sales growth, production quality, waste loss, and distributor performance. Decision-makers had limited visibility into operational inefficiencies and overall business performance, making it difficult to identify growth opportunities and improve manufacturing efficiency.

This project was developed to provide a single source of truth for monitoring both commercial and operational performance.

---

## Executive Summary

| KPI | Value |
|---|---|
| Total Sales | **15M PKR** |
| Sales YTD | **6M PKR** |
| Target Achievement Ratio | **1.39** |
| Production Waste Loss | **20.26K Units** |
| Sales Growth (2024–2026) | **34.1%** |
| Annual Sales Target | **31M PKR** |
| Monthly Target Achievement | **1,671% (Historical Reference)** |

Sales grew from **4.4M PKR in 2024** to **5.5M PKR in 2025** and **5.9M PKR in 2026**, representing 34.1% overall growth. Monthly production rejection rates fluctuated between **3.3% and 5.0%**, and total production waste reached **20.26K units**, highlighting opportunities for operational improvement and cost reduction.

---

## Dashboard Preview

![Tobacco Enterprise Analytics Dashboard](https://github.com/user-attachments/assets/4b39266b-94ff-42e6-965a-2f4d364a5438)

---

## Sales Performance by Distributor

| Distributor | Total Sales | Notes |
|---|---|---|
| Punjab Corp | **3.9M PKR** | Highest performer |
| Arifwala Sales | **3.3M PKR** | |
| Sahiwal Traders | **2.3M PKR** | |
| Multan Mart | **2.1M PKR** | |
| Cherab Dist | **1.5M PKR** | Lowest performer |

Punjab Corp and Arifwala Sales together contributed approximately **55% of total distributor revenue**, indicating a revenue concentration risk. A significant performance gap exists between the top distributor (3.9M PKR) and the lowest (1.5M PKR).

---

## Revenue Growth Trend

| Year | Total Sales |
|---|---|
| 2024 | 4.4M PKR |
| 2025 | 5.5M PKR |
| 2026 | 5.9M PKR (YTD: 6M PKR) |

The consistent upward trend reflects **34.1% growth** over three years, with continued acceleration from 2025 to 2026.

---

## Brand Portfolio

The dashboard tracks four brands, each filterable via interactive slicers:

- **Capstan**
- **Diplomat**
- **Gold Leaf**
- **Morven**

---

## Production Quality & Waste Analysis

Monthly production rejection rates fluctuated between **3.3% and 5.0%** across the reporting period, indicating variability in manufacturing quality.

- Rejection rate **peaked at ~5.0%** in months 5 and 12
- Rejection rate **dipped to ~3.3%** in months 3 and 10
- Total production waste: **20.26K units**

---

## Sales vs. Annual Target Achievement

The gauge chart tracks actual sales against the annual target:

| Metric | Value |
|---|---|
| Actual Total Sales | 15M PKR |
| Annual Sales Target | 31M PKR |
| Monthly Reference Floor | 917K PKR |
| Monthly Target Achievement | 1,671% (Historical Reference) |
| Target Achievement Ratio | 1.39 |

---

## Data Model

A Star Schema was implemented to improve performance, scalability, and reporting accuracy. The model resolves granularity differences between monthly targets and daily sales transactions, ensuring accurate KPI calculations and time-based analysis.

<img width="1668" height="943" alt="schema" src="https://github.com/user-attachments/assets/408d3fa2-581e-4a7a-807b-bb6768756888" />

### Fact Tables

- `Fact_Sales`
- `Fact_Production`
- `Fact_Targets`

### Dimension Tables

- `Dim_Date`
- `Dim_Brand`

---

## Power BI Features Implemented

### DAX Measures

- Total Sales
- Sales YTD
- Target Achievement Ratio
- Production Waste Loss
- Time Intelligence Calculations

### Visualizations

- **KPI Cards** — Total Sales, Sales YTD, Target Achievement Ratio, Production Waste Loss
- **Area Chart** — Total Sales Trend by Year (2024–2026)
- **Line Chart** — Monthly Production Rejection Rate Trend
- **Horizontal Bar Chart** — Sales Performance by Distributor
- **Gauge Chart** — Sales vs. Annual Target Achievement

### User Experience

- Interactive Slicers (Year, Brand)
- Cross-Filtering across all visuals
- Report Page Tooltips
- Drill-Down Navigation

---

## Sample DAX Measures

### Total Sales

```dax
Total Sales =
SUM(Fact_Sales[SalesAmount])
```

### Sales YTD

```dax
Sales YTD =
TOTALYTD(
    [Total Sales],
    Dim_Date[Date]
)
```

### Target Achievement Ratio

```dax
Target Achievement Ratio =
DIVIDE(
    [Total Sales],
    [Target Sales]
)
```

---

## Analytical Insights

| Area | Finding |
|---|---|
| Revenue Growth | Sales grew from 4.4M PKR (2024) to 5.9M PKR (2026) — a 34.1% increase |
| Distributor Performance | Punjab Corp led at 3.9M PKR; Cherab Dist lowest at 1.5M PKR |
| Revenue Concentration | Top two distributors contributed ~55% of total revenue — concentration risk |
| Production Waste | 20.26K units of waste identified; significant cost reduction opportunity |
| Product Quality | Monthly rejection rates of 3.3%–5.0% indicate manufacturing variability |
| Target Performance | Target Achievement Ratio of 1.39 demonstrates strong sales execution |
| Distributor Gap | 2.4M PKR gap between highest and lowest distributor performance |

---

## Business Recommendations

### Quality Improvement
Conduct audits during high-rejection months (months 5 and 12) and implement machine calibration procedures to consistently reduce rejection rates below 3.3%.

### Distributor Development
Introduce targeted incentive programs and performance reviews for lower-performing distributors, particularly Cherab Dist and Multan Mart.

### Waste Reduction
Establish production waste thresholds and implement continuous monitoring to reduce the current 20.26K units of operational waste.

### Inventory Optimization
Align procurement and inventory planning with the observed sales growth trajectory (4.4M → 5.9M PKR) to improve supply chain efficiency.

### Predictive Maintenance
Implement preventive maintenance schedules to minimize downtime and production disruptions that contribute to quality variability.

### Brand Growth Strategy
Develop promotional campaigns for lower-performing brands to improve market penetration across all four product lines.

### Workforce Training
Provide targeted training programs focused on reducing rejection rates and improving operational consistency during high-rejection periods.

### Strategic Planning
Use dashboard insights to align the 31M PKR annual target with realistic monthly milestones and support long-term business planning.

---

## Projected Business Impact

Implementing the proposed recommendations could potentially:

- Reduce production waste by up to **15%**
- Increase distributor revenue by approximately **10%**
- Improve manufacturing efficiency and quality consistency
- Strengthen sales forecasting accuracy
- Increase overall profitability by an estimated **8%**

---

## Technical Skills Demonstrated

- Power BI
- DAX
- Power Query
- Star Schema Modeling
- KPI Development
- Sales Analytics
- Manufacturing Analytics
- Business Intelligence Reporting
- Dashboard Design
- Data Visualization
- Business Process Analysis
- Performance Monitoring

---

## Repository Structure

```
├── Dashboard.pbix
├── Dataset/
├── Screenshots/
├── Documentation/
└── README.md
```

---

## Conclusion

This project demonstrates how Power BI can transform raw sales and production data into actionable business intelligence. By consolidating **15M PKR in sales** across five distributors and four brands into a unified reporting platform, the dashboard gives management real-time visibility into revenue growth (34.1% over three years), production quality (3.3%–5.0% monthly rejection rates), waste performance (20.26K units), and target achievement (ratio of 1.39).

The Star Schema data model and DAX measures ensure accurate, scalable KPI tracking, while interactive slicers and cross-filtering empower management to drill into specific periods, brands, or distributors. The insights and recommendations delivered through this dashboard position the organization to reduce waste, develop distributor performance, and improve overall profitability.
