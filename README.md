# Zomato Sales and Restaurant Rating Analytics

[![SQL](https://img.shields.io/badge/SQL-Data_Extraction_%26_Transformations-orange?style=for-the-badge)](#)
[![Tableau](https://img.shields.io/badge/Tableau-Business_Intelligence-blue?style=for-the-badge&logo=tableau&logoColor=white)](#)
[![Power BI](https://img.shields.io/badge/Power_BI-F2C811?style=for-the-badge&logo=powerbi&logoColor=black)](#)
[![Excel](https://img.shields.io/badge/Microsoft_Excel-217346?style=for-the-badge&logo=microsoftexcel&logoColor=white)](#)

**Author:** [Arya Pandey](https://github.com/aryapandeyyy28-sudo)  
**Role:** Data & Business Analyst  
**Contact:** [aryapandeyyy28@gmail.com](mailto:aryapandeyyy28@gmail.com)

---

## Project Overview
This project presents an end-to-end data analytics study of Zomato restaurant operations, customer dining patterns, pricing tiers, and rating distributions. By combining data transformation in SQL and visual storytelling in business intelligence dashboards, the objective is to uncover operational factors that influence customer sentiment, average spend, and table booking retention.

---

## Key Business Questions Analyzed
- What is the relationship between average dining cost for two and net customer ratings?
- Do restaurants offering online order delivery receive higher review counts and better ratings compared to dine-in only establishments?
- Which city localities represent underserved markets with high demand but low restaurant density?
- What are the most popular cuisine categories across budget and premium dining segments?

---

## Dashboard Visuals and Performance Views

### 1. Executive Performance and Rating Overview
> Comprehensive scorecard displaying total restaurants analyzed, average customer rating, average cost for two, and total votes.

![Executive Performance Overview](Screenshots/1.png)

---

### 2. Online Delivery vs. Table Booking Breakdown
> Comparative distribution examining vote concentration and ratings based on operational capabilities (Has Table Booking vs. Has Online Delivery).

![Delivery and Booking Analysis](Screenshots/2.png)

---

### 3. City-Wise Restaurant Density and Spending Distribution
> Geographic breakdown highlighting leading restaurant markets, average dining spend by locality, and rating variations across territories.

![City and Locality Breakdown](Screenshots/3.png)

---

### 4. Cuisine Popularity and Price Tier Segmentation
> Detailed matrix analyzing top-performing cuisines, cost bands (Budget, Moderate, Luxury), and voter distribution.

![Cuisine and Cost Segmentation](Screenshots/4.png)

---

## Data Architecture and Methodology

### 1. Data Cleaning and Preparation (SQL & Excel)
- Removed duplicate restaurant IDs and handled null values in cost and aggregate ratings.
- Normalized multi-value string columns containing multiple cuisines into standardized categories.
- Classified pricing into distinct customer spending tiers using SQL `CASE WHEN` logic.

### 2. Key SQL Queries and Aggregations
- Identified top-rated restaurants by city with a minimum vote threshold to eliminate statistical bias.
- Calculated rating distribution percentiles across delivery vs. non-delivery venues.
- Formulated rolling averages and vote-weighted dining scores.

### 3. Business Intelligence Dashboard Design
- Configured interactive cross-filtering by city, cuisine, price range, and delivery options.
- Designed dynamic KPI cards with automated color formatting for rating bands (Poor, Average, Good, Excellent).

---

## Key Analytical Findings
- **Online Delivery Advantage:** Outlets offering online food ordering recorded 28% higher overall review engagements and consistent rating volumes.
- **Cost vs. Rating Sweet Spot:** Mid-tier dining segments (Cost for Two between 500 and 1,200) exhibited the highest customer satisfaction-to-price ratio.
- **Table Booking Impact:** High-end restaurants featuring table reservation options scored consistently above 4.0 in customer sentiment.

---

## Repository Structure

```text
├── data/               # Raw and cleaned restaurant datasets (CSV / Excel)
├── sql/                # SQL queries, transformations, and view scripts
├── reports/            # BI dashboard source files (.twbx / .pbix)
├── Screenshots/        # Dashboard captures and visual report assets
│   ├── 1.png
│   ├── 2.png
│   ├── 3.png
│   └── 4.png
└── README.md           # Project documentation and executive summary