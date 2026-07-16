REPOSITORY STRUCTURE
=====================

```
Projects_Tableau/
├── Tableau_Project_1.zip
└── Tableau_Project_2.zip
└── PowerBI_Project_1: PowerBI_Project_Hospital_Readmissions_Operations_Dashboard.pbix, PowerBI_Project_Hospital_Readmission_Operations_Dashboard.pdf
└── PowerBI_Project_2: PowerBI_Project_Data_Professional_Survey.pbix, PowerBI_Project_Data_Professional_Survey.pdf
└── README.md
```

# 1. TABLEAU_PROJECT_1: Video Game Global Sales Analysis 🎮

An interactive Tableau project exploring global video game sales data — analyzing trends across genres, platforms, regions, and time to uncover which factors drove commercial success in the gaming industry from the 1980s through the mid-2010s.

## 📊 Project Overview

This project dives into a global video game sales dataset to answer questions like:
- Which genres generated the most revenue globally and in North America?
- How did the industry's sales volume evolve year over year?
- Which genres peaked in which eras, and how did platform-specific performance compare?
- How does regional (NA/EU) performance break down by genre and time period?

The analysis is presented through a series of standalone visualizations and two consolidated interactive dashboards.

## 🔍 Key Insights

- **Action, Sports, and Shooter** are the top three genres by global sales, together accounting for the majority of total revenue.
- Global and NA sales tracked closely together, both **peaking around 2008–2009** before a steady decline through 2016 — reflecting the industry's console-cycle boom and the shift toward digital/mobile gaming.
- **Racing games spiked sharply around 2001–2004**, while **Shooter titles saw a resurgence around 2011**, showing how genre popularity shifted across console generations.
- Genre performance is heavily right-skewed — a handful of genres (Action, Sports) dominate, while niche genres like Strategy and Adventure make up a small share of total sales, as seen in the box-and-whisker distribution.

## 📈 Visualizations

| Visualization | Type | Description |
|---|---|---|

| `GlobalSales_PS_Year_Line` | Line chart | Genre sales trends over time |
| `GlobalSales_Genre_Bar` | Bar chart | Total global sales ranked by genre |
| `Global_NA_Sales_Bar-Line` | Combo chart | Global sales (bars) vs. NA sales (line) by year |
| `GlobalSales_Genre_Pie` | Pie chart | Genre share of total global sales |
| `Global_Sales_Genre_Treemap` | Treemap | Proportional genre sales at a glance |
| `GlobalSales_Genre_Box_Whisker` | Box & whisker | Distribution and spread of sales across genres |
| `GlobalSales_NASales_Genre_PackedBubble` | Packed bubble | Global sales sized, NA sales color-coded, by genre |
| `Global_Sales_EU_Sales_Year_Bin_CF` | Stacked bar | Global vs. EU sales by genre, binned by year, with custom filter |
| `NASales_Genre_Area` | Stacked area | NA sales composition by genre over time |
| `US_States_TimeZone_Map` | Filled map | US states colored by time zone (regional context) |

## 🖥️ Dashboards

- **Global Sales Dashboard** — Genre bar/pie/treemap/bubble/box-whisker views combined for genre-level exploration
- **US Timezone + Global Sales Dashboard** — Combines the timezone map with genre and yearly sales trends
- **US Timezone + NA Sales Dashboard** — Regional context paired with NA sales-by-genre trends

## 🛠️ Tools Used

- **Tableau** — data visualization and dashboard design

## 📁 Folder Structure

```
Tableau_Project_1/
├── README.md
├── dashboards/
│   ├── Global_Sales_Dashboard.png
│   ├── US_Timezone_GlobalSales_Dashboard.png
│   └── US_Timezone_NASales_Dashboard.png
└── visualizations/
    ├── GlobalSales_PS_Year_Line.png
    ├── GlobalSales_Genre_Bar.png
    ├── Global_NA_Sales_Bar-Line.png
    ├── GlobalSales_Genre_Pie.png
    ├── Global_Sales_Genre_Treemap.png
    ├── GlobalSales_Genre_Box_Whisker.png
    ├── GlobalSales_NASales_Genre_PackedBubble.png
    ├── Global_Sales_EU_Sales_Year_Bin_CF.png
    ├── NASales_Genre_Area.png
    └── US_States_TimeZone_Map.png
```


# 2. TABLEAU_PROJECT_2: Airbnb Pricing & Revenue Analysis (Seattle) 🏠

A Tableau project analyzing Seattle Airbnb listing data to understand how pricing varies by property size and location, and how host revenue has trended over time.

## 📊 Project Overview

This project explores an Airbnb listings dataset (Seattle, WA — zip codes in the 981xx range) to answer:
- How does average nightly price scale with the number of bedrooms?
- Which zip codes command the highest and lowest average prices?
- How has overall host revenue trended week over week?
- What's the distribution of listings by bedroom count?

## 🔍 Key Insights

- **Price scales steadily with bedroom count** — from ~$96/night for a 1-bedroom up to ~$585/night for a 6-bedroom listing, roughly a 6x increase.
- **Most listings are small**: 1-bedroom units make up the vast majority of inventory (1,811 listings), while 5–6 bedroom listings are rare (20 and 5, respectively) — meaning premium listings are scarce but command a big price premium.
- **Location drives significant price variation**: top zip codes (e.g., 98119, 98109, 98199) average $160–$205/night, while lower-priced zip codes (e.g., 98125, 98133) average under $70/night — nearly a 3x spread across the city.
- **Revenue grew sharply through early 2016** (from ~$1,000K to ~$1,900K by spring), then plateaued and held steady in the $1,900K–$2,000K range for the rest of the year, with a late-year uptick.

## 📈 Visualizations

| Visualization | Type | Description |
|---|---|---|
| `Airbnb_AvgPrice_Bedroom_Bar` | Bar chart | Average price by number of bedrooms |
| `Distinct-Count_Bedroom-Listings_Table` | Table | Listing count by bedroom count |
| `Airbnb_AvgPrice_zipcode_Map` | Filled map | Average price by zip code, geographically |
| `Airbnb_AvgPrice_zipcode_Bar` | Bar chart | Zip codes ranked by average price |
| `Airbnb_Revenue_year_line` | Line chart | Weekly host revenue trend across 2016 |

## 🖥️ Dashboard

**Airbnb Project Dashboard** — a combined view bringing together bedroom pricing, listing distribution, zip-code-level pricing (map + bar), and the revenue trend line for at-a-glance market analysis.

## 🛠️ Tools Used

- **Tableau** — data visualization and dashboard design

## 📁 Folder Structure

```
Tableau_Project_2/
├── README.md
├── dashboard/
│   └── Airbnb_Project.png
└── visualizations/
    ├── Airbnb_AvgPrice_Bedroom_Bar.png
    ├── Distinct-Count_Bedroom-Listings_Table.png
    ├── Airbnb_AvgPrice_zipcode_Map.png
    ├── Airbnb_AvgPrice_zipcode_Bar.png
    └── Airbnb_Revenue_year_line.png
```

# 3. POWERBI_PROJECT 1: Hospital Readmission & Operation Dashboard 🏥

An end-to-end Power BI project analyzing readmission performance and emergency department 
timeliness across 3,000+ Medicare-registered hospitals, built entirely from real, public 
CMS government data (not a pre-cleaned Kaggle dataset).

## 📊 Project Overview

This project explores CMS Hospital Compare data to answer:

- Which hospitals show higher-than-expected 30-day readmission rates?
- How much does readmission performance vary hospital-by-hospital vs. state-by-state?
- Is there a relationship between how fast a hospital's ED moves and its readmission outcomes?
- Where should hospital operations leadership prioritize improvement efforts?

## 🔍 Key Insights

- **Readmission risk is a hospital-level problem, not a regional one.** State-level averages 
  cluster tightly between 1.01–1.03, while individual hospitals range as high as 1.31 and 
  as low as 0.85 — a much wider spread than geography alone would suggest.
- **ED wait times don't predict readmission rates.** A benchmark comparison across hospitals 
  found no consistent relationship between emergency department speed and readmission 
  performance, suggesting these are two independent operational challenges requiring 
  separate improvement strategies.

## 📈 Visualizations

| Visualization | Type | Description |
| -------------- | ---- | ----------- |
| `KPI_Summary_Cards` | Card | Total hospitals, national avg readmission ratio, avg ED wait time |
| `Readmission_Ratio_by_State` | Filled map | US states shaded by average excess readmission ratio |
| `Top10_States_Readmission_Bar` | Bar chart | Worst-performing states by readmission ratio |
| `Hospital_Drilldown_Table` | Table | Facility-level ratio, variance, and rank, conditionally formatted |
| `Top10_Hospitals_Variance_Bar` | Bar chart | Worst-performing individual hospitals |
| `EDWaitTime_vs_Readmission_Scatter` | Scatter chart | Benchmark comparison across all hospitals |

## 🖥️ Dashboard Pages

- **Executive Overview** — KPI cards, US map, top 10 worst states, and a key-finding callout
- **Hospital Drill-down** — filterable (State, Measure) table ranked and color-coded by 
  readmission variance, paired with a worst-performers bar chart
- **Benchmark Comparison** — scatter plot testing ED wait time against readmission ratio

## 🗂️ Data Sources

All data sourced directly from [data.cms.gov](https://data.cms.gov):
- Hospital General Information
- Hospital Readmissions Reduction Program (HRRP)
- Timely and Effective Care - Hospital

## 🛠️ Tools Used

- **Power BI Desktop** — data modeling, DAX, dashboard design
- **Power Query (M)** — data cleaning and transformation
- **DAX** — RANKX, CALCULATE, ALLEXCEPT for benchmark and ranking measures

## 📁 Folder Structure

```
Project_Tableau_PowerBI/
├── Hospital_Readmissions_Operations_Dashboard.pbix
└── PowerBI_Project_Hospital_Readmission_Operations_Dashboard.pdf
```

# 4. POWERBI_PROJECT 2: Data Professional Survey Analysis 📋

An interactive Power BI dashboard analyzing a real survey of ~630 data professionals, exploring salary, role, tools, and career trends across 
the data industry.

## 📊 Project Overview

This project explores survey responses from working data professionals to answer:

- How does average salary vary by role (Data Analyst, Data Scientist, Data Engineer, etc.)?
- Which countries report the highest and lowest average salaries?
- What programming languages and tools do data professionals prefer?
- What level of education is typical for breaking into the data field?
- How satisfied are respondents with their current roles, and how many have switched 
  careers into data?

## 🔍 Key Insights

- Data Scientists report the highest average salary among data roles, followed by 
  Data Engineers and Data Architects — with Data Analysts earning notably less.
- Salary varies significantly by country, with cost of living playing a clear role — 
  a high number doesn't always mean better relative pay.
- A graduate degree isn't a strict requirement to enter the field — many respondents 
  broke in with a Bachelor's degree.
- A majority of respondents report having switched careers into data from a different field.

## 📈 Visualizations


| Visualization | Type | Description |
| -------------- | ---- | ----------- |
| `Avg_Salary_by_Role_Bar` | Bar chart | Average salary broken down by job title |
| `Avg_Salary_by_Country_Map` | Filled map | Average salary by respondent country |
| `Favorite_Language_Donut` | Donut/Pie chart | Most preferred programming language |
| `Education_Level_Bar` | Bar chart | Highest education level among respondents |
| `Career_Switcher_KPI` | Card | % of respondents who switched careers into data |
| `Job_Satisfaction_Table` | Table/Matrix | Satisfaction levels by role |

## 🖥️ Dashboard

**Data Professional Survey Dashboard** — a single-page interactive view combining salary, 
role, tools, education, and satisfaction insights with slicers for role and country.

## 🛠️ Tools Used

- **Power BI Desktop** — dashboard design and DAX
- **Power Query (M)** — data cleaning (standardizing salary ranges, consolidating 
  low-frequency job titles into "Other," removing empty tracking columns)

## 📁 Folder Structure

```
PowerBI_Project_Data_Professional_Survey/
├── PowerBI_Project_Data_Professional_Survey.pbix
├── PowerBI_Project_Data_Professional_Survey.pdf
└── Power BI - Final Project.xlsx
```
## 🔗 Connect

Feel free to explore the visuals above or reach out with questions/feedback!
