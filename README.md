# Zomato Restaurants Analysis — Power BI

A Power BI project analyzing restaurant performance across Indian cities using Zomato data. The report surfaces city-wise density and ratings, cuisine trends, pricing vs. ratings patterns, and quality vs. visibility signals for targeted operational and growth decisions.

## Tech Stack
- **Power BI Desktop**
- **Power Query**
- **DAX**
- **Microsoft Excel**

## Repository Contents
- `Zomato_Insights_Dashboard.pbix` — Power BI dashboard file
- `zomato_data.xlsx` — Source dataset
- `snapshot.jpg` — Dashboard preview image
- `overview.pdf` — Supplementary overview
- `insights.ipynb` — Supporting notebook (optional analysis)

## Key Insights

### 1) City-wise Performance
- **New Delhi** leads with **5,473** listings due to population density, tourist footfall, and mature dining infrastructure.
- **Gurgaon (1,118)** and **Noida (1,080)** follow, driven by large IT/corporate hubs and high delivery demand. Noida shows stronger chain ratings (e.g., **Domino’s 3.36** vs. **Gurgaon 3.20**), likely due to newer outlets and tighter quality controls.
- **Ahmedabad (21), Chennai (20), Jaipur (20)** are underserved but sustain ratings comparable to larger metros, suggesting expansion potential with lower competitive pressure.

### 2) Cuisine Trends
- **North Indian (3,960)** and **Chinese (2,735)** dominate by listings due to broad appeal, scalable operations, and robust supply chains.
- **Fast-food chains** (e.g., **Domino’s 3.36**, **Subway 2.81**) outperform localized **Mughlai (~2.90)** driven by standardized recipes, franchise training, and brand consistency.
- **Italian (764)** and **Continental (736)** show mid-density but strong average ratings—high-potential segments as urban incomes and tastes evolve.

### 3) Pricing vs. Ratings
- **Mid-range pricing** delivers the best satisfaction: Domino’s (mid-tier) leads with **3.36** average rating.
- **Budget** operators (e.g., **Café Coffee Day 2.61**) face thin margins that can limit quality; **premium** segments trend below **3.0** at high review volumes due to heightened expectations and outlet variability.
- Recommendation: focus on **mid-market offerings** that balance value, reliability, and affordability.

### 4) Quality and Visibility
- **Hidden gems**: **Green Chick Chop (2.94)** and **Subway (2.81)** maintain near-3.0 ratings with modest review counts (~3 outlets each)—promote to raise awareness.
- **Risk areas**: **Café Coffee Day (2.61, >1M votes)** and **McDonald’s (2.80, high volume)** show sub-3.0 ratings despite large visibility—prioritize quality interventions (menu standards, store refresh, staff training).

## How to Use
1. Open `Zomato_Insights_Dashboard.pbix` in **Power BI Desktop**.
2. If needed, update the data source path to `zomato_data.xlsx`.
3. Refresh data.
4. Explore via slicers and drill-through: city, cuisine, price band, and rating band.

## Reproduce / Data Prep Notes
- Power Query steps: standardize city/cuisine names, handle nulls, normalize price/rating columns, remove duplicates/outliers.
- Data model: star-like structure with dimension tables for city/cuisine; explicit relationships; DAX measures for KPIs (avg rating, cost for two bands, review counts, top cities/cuisines/brands).

## Recommendations Summary
- Expand in **underserved high-potential cities** (Ahmedabad/Chennai/Jaipur) with curated partner onboarding and targeted promotions.
- Double down on **mid-range pricing** and consistency to lift ratings above 3.0.
- Promote **hidden gems** to increase visibility; apply **quality fixes** for high-volume underperformers.

## Dashboard Preview
![Dashboard Snapshot](./snapshot.jpg)
