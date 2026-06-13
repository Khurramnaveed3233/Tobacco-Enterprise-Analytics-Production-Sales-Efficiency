````markdown
# Tobacco Manufacturing Analytics Dashboard

### Sales Performance, Production Efficiency & Target Achievement Analysis using Power BI

---

## Project Overview

This project analyzes sales performance, production efficiency, and target achievement for a tobacco manufacturing company using Power BI. The objective was to create a centralized analytics solution that enables management to monitor business performance, identify operational inefficiencies, and support data-driven decision-making.

The dashboard consolidates sales, production, distributor, and target data into a single reporting platform, providing real-time visibility into revenue growth, quality performance, production losses, and business targets.

---

## Skills & Tools

**Power BI • DAX • Power Query • Data Modeling • Star Schema • KPI Development • Sales Analytics • Manufacturing Analytics • Business Intelligence • Data Visualization**

---

## Business Problem

The organization lacked a centralized reporting solution to monitor sales growth, production quality, waste loss, and distributor performance. Decision-makers had limited visibility into operational inefficiencies and overall business performance, making it difficult to identify growth opportunities and improve manufacturing efficiency.

This project was developed to provide a single source of truth for monitoring both commercial and operational performance.

---

## Executive Summary

The dashboard revealed that the company generated **15M PKR in total sales**, achieved **34.1% sales growth** over three years, and maintained a **Target Achievement Ratio of 1.39**. Analysis also identified **20.26K units of production waste** and monthly rejection rates ranging from **3.3% to 5.0%**, highlighting opportunities for operational improvement and cost reduction.

---

## Dashboard Preview

![Tobacco Enterprise Analytics Dashboard](https://github.com/user-attachments/assets/4b39266b-94ff-42e6-965a-2f4d364a5438)

---

## Key Business Metrics

| KPI | Value |
|------|------|
| Total Sales | 15M PKR |
| Sales YTD | 6M PKR |
| Target Achievement Ratio | 1.39 |
| Production Waste Loss | 20.26K Units |

---

## Data Model

A Star Schema data model was implemented to improve performance, scalability, and reporting accuracy.

### Fact Tables

- Fact_Sales
- Fact_Production
- Fact_Targets

### Dimension Tables

- Dim_Date
- Dim_Brand

The model was designed to resolve granularity differences between monthly targets and daily sales transactions, ensuring accurate KPI calculations and time-based analysis.

---

## Power BI Features Implemented

### DAX Measures

- Total Sales
- Sales YTD
- Target Achievement Ratio
- Production Waste Loss
- Time Intelligence Calculations

### Visualizations

- KPI Cards
- Gauge Charts
- Line Charts
- Area Charts
- Trend Analysis Visuals

### User Experience

- Interactive Slicers
- Cross-Filtering
- Report Page Tooltips
- Drill-Down Navigation

---

## Sample DAX Measures

### Total Sales

```DAX
Total Sales =
SUM(Fact_Sales[SalesAmount])
````

### Sales YTD

```DAX
Sales YTD =
TOTALYTD(
    [Total Sales],
    Dim_Date[Date]
)
```

### Target Achievement Ratio

```DAX
Target Achievement Ratio =
DIVIDE(
    [Total Sales],
    [Target Sales]
)
```

---

## Analytical Insights

### Revenue Growth

Sales increased from **4.4M PKR in 2024** to **5.9M PKR in 2026**, representing an overall growth rate of **34.1%**.

### Distributor Performance

Punjab Corp generated **3.9M PKR**, making it the highest-performing distributor and a key revenue contributor.

### Revenue Concentration

The top two distributors contributed approximately **55% of total distributor revenue**, indicating a potential concentration risk.

### Production Waste

Production waste reached **20.26K units**, highlighting opportunities for cost reduction and process optimization.

### Product Quality

Monthly rejection rates fluctuated between **3.3% and 5.0%**, suggesting variability in manufacturing quality.

### Sales Target Performance

The business achieved a **Target Achievement Ratio of 1.39**, demonstrating strong sales execution.

### Distributor Gap Analysis

A significant performance gap exists between the highest-performing distributor (Punjab Corp) and the lowest-performing distributor (Cherab Dist), indicating opportunities for distributor development.

---

## Business Recommendations

### Quality Improvement

Conduct audits during high-rejection periods and implement machine calibration procedures to improve product quality.

### Distributor Development

Introduce targeted incentive programs and performance reviews for lower-performing distributors.

### Waste Reduction

Establish production waste thresholds and implement continuous monitoring to reduce operational losses.

### Inventory Optimization

Align procurement and inventory planning with sales demand patterns to improve efficiency.

### Predictive Maintenance

Implement preventive maintenance schedules to minimize downtime and production disruptions.

### Brand Growth Strategy

Develop promotional campaigns for lower-performing brands to improve market penetration.

### Workforce Training

Provide targeted training programs focused on reducing rejection rates and improving operational consistency.

### Strategic Planning

Use dashboard insights to establish more realistic sales targets and support long-term business planning.

---

## Business Impact

Implementing the proposed recommendations could potentially:

* Reduce production waste by up to 15%
* Increase distributor revenue by approximately 10%
* Improve manufacturing efficiency
* Strengthen product quality consistency
* Improve sales forecasting accuracy
* Increase overall profitability by an estimated 8%

---

## Project Highlights

* Built an executive Power BI dashboard tracking **15M PKR** in sales performance.
* Analyzed **34.1% revenue growth** across a three-year period.
* Identified **20.26K units** of production waste impacting operational efficiency.
* Evaluated distributor performance and revenue concentration risks.
* Designed a Star Schema data model and developed DAX measures for KPI tracking.
* Delivered actionable recommendations to improve profitability and operational performance.

---

## Technical Skills Demonstrated

* Power BI
* DAX
* Power Query
* Star Schema Modeling
* KPI Development
* Sales Analytics
* Manufacturing Analytics
* Business Intelligence Reporting
* Dashboard Design
* Data Visualization
* Business Process Analysis
* Performance Monitoring

---

## Repository Structure

```text
├── Dashboard.pbix
├── Dataset/
├── Screenshots/
├── Documentation/
└── README.md
```

---

## Conclusion

This project demonstrates how Power BI can transform raw sales and production data into actionable business intelligence. By integrating operational and commercial performance metrics into a unified reporting solution, management gains visibility into revenue growth, production efficiency, quality performance, and strategic opportunities for improvement.

```
```
