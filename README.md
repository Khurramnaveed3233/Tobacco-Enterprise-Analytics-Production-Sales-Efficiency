# Tobacco Enterprise Analytics: Production & Sales Efficiency

<img width="1649" height="954" alt="Tobacco-Enterprise-Analytics-Production-Sales-Efficiency" src="https://github.com/user-attachments/assets/4b39266b-94ff-42e6-965a-2f4d364a5438" />

## Executive Summary

Developed an interactive Power BI dashboard to analyze sales performance and production efficiency for a tobacco manufacturing company. The solution consolidates sales, distributor, production, and target data into a single reporting platform, enabling stakeholders to monitor key business metrics, identify operational inefficiencies, and make data-driven decisions.

The dashboard provides visibility into revenue growth, target achievement, distributor performance, production waste, and quality trends, helping management improve profitability and operational effectiveness.

---

## Business Problem

The organization lacked a centralized reporting system to monitor sales growth, production quality, waste loss, and distributor performance. As a result, management had limited visibility into operational inefficiencies and overall business performance, making strategic decision-making more difficult.

This project was designed to provide a single source of truth for monitoring sales and production operations through interactive business intelligence reporting.

---

## Key Insights

- Total sales reached **15M PKR**.
- Sales increased from **4.4M PKR in 2024** to **5.9M PKR in 2026**, representing **34.1% overall growth**.
- Punjab Corp generated **3.9M PKR**, making it the highest-performing distributor.
- The top two distributors contributed approximately **55% of total distributor revenue**.
- Production waste reached **20.26K units**, indicating opportunities for cost optimization.
- Monthly rejection rates ranged between **3.3% and 5.0%**, highlighting quality consistency challenges.
- The business achieved a **Target Achievement Ratio of 1.39**, demonstrating strong sales performance.

---

## Business Impact

This dashboard enables management to monitor business performance in real time, identify revenue opportunities, reduce production waste, improve quality control, and optimize distributor performance.

The insights generated support:
- Improved profitability
- Better operational efficiency
- Faster decision-making
- Enhanced production planning
- More effective strategic execution

---

## Data Modeling Approach

A Star Schema data model was implemented, with **Fact_Sales**, **Fact_Production**, and **Fact_Targets** serving as the central fact tables.

These tables are connected to shared dimension tables such as:

- Dim_Date
- Dim_Brand

The model was specifically designed to resolve granularity differences between monthly sales targets and daily sales transactions, ensuring accurate reporting and KPI calculations.

---

## Power BI Features Used

### DAX Measures
- Time Intelligence Calculations (YTD Sales)
- Target Achievement Ratio
- KPI Aggregations
- DIVIDE-based Performance Metrics

### Visualizations
- KPI Cards
- Gauge Charts
- Line Charts
- Area Charts
- Trend Analysis Visuals

### User Experience (UX)
- Interactive Slicers
- Cross-Filtering
- Report Page Tooltips
- Drill-Down Navigation

---

## Key Performance Indicators (KPIs)

| KPI | Value | Business Meaning |
|------|---------|----------------|
| Total Sales | 15M PKR | Total revenue generated |
| Sales YTD | 6M PKR | Current year sales performance |
| Target Achievement Ratio | 1.39 | Sales performance relative to targets |
| Production Waste Loss | 20.26K Units | Total production losses |

---

## Analytical Insights

### 1. Sales Growth Trend
Sales increased from **4.4M PKR (2024)** to **5.9M PKR (2026)**, representing an overall growth rate of **34.1%**.

### 2. Revenue Concentration
Punjab Corp contributed approximately **26% of total revenue**, making it the most important distributor.

### 3. Production Quality Variability
Rejection rates fluctuated between **3.3% and 5.0%**, indicating inconsistencies in production quality.

### 4. Waste Impact on Profitability
Production waste reached **20.26K units**, potentially reducing profit margins by an estimated **5–8%**.

### 5. Sales Target Performance
Actual sales reached **15M PKR** against an annual target of **31M PKR**, achieving approximately **48% of the target**.

### 6. Distributor Performance Gap
A significant revenue gap exists between Punjab Corp (**3.9M PKR**) and Cherab Dist (**1.5M PKR**), representing a difference of approximately **61%**.

### 7. YTD Performance Monitoring
Current Year-to-Date sales stand at **6M PKR**, representing approximately **19% of the annual target**, indicating a need for stronger sales momentum in upcoming periods.

### 8. Rejection Rate Correlation
Higher rejection rates tend to occur during peak production periods, suggesting capacity-related quality challenges.

### 9. Brand Performance
Gold Leaf and Capstan emerged as leading contributors to distributor sales performance.

### 10. Target Efficiency
The **1.39 Target Achievement Ratio** indicates performance above the baseline expectation.

---

## Business Recommendations

### Quality Control Optimization
Conduct audits during high-rejection periods and implement machine calibration procedures.

### Distributor Development
Introduce targeted incentive programs for lower-performing distributors such as Cherab Dist.

### Inventory Planning
Align raw material procurement with peak sales periods to avoid shortages and excess inventory.

### Waste Reduction Strategy
Establish a production waste threshold of **3.5%** and continuously monitor performance.

### Target Planning
Increase future sales targets by approximately **10%** based on current achievement trends.

### Brand Growth Initiatives
Launch promotional campaigns for lower-performing brands to increase market share.

### Predictive Maintenance
Implement preventive maintenance schedules to reduce production disruptions.

### Workforce Training
Provide specialized training programs focused on reducing rejection rates and improving quality consistency.

---

## Business Impact

Implementing these recommendations could potentially:

- Reduce production waste by **15%**
- Increase distributor revenue by **10%**
- Improve production efficiency
- Enhance product quality
- Strengthen sales performance
- Increase profitability by an estimated **8%**

---

## Technical Skills Demonstrated

- Power BI
- DAX
- Power Query
- Star Schema Data Modeling
- Data Visualization
- KPI Development
- Business Process Analysis
- Sales Analytics
- Manufacturing Analytics
- Performance Reporting
- Dashboard Design
- Business Intelligence
