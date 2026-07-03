REPOSITORY STRUCTURE
=====================

├── Tableau_Project_1/
│   ├── README.md
│   ├── dashboards/
│   │   ├── Global_Sales_Dashboard.png
│   │   ├── US_Timezone_GlobalSales_Dashboard.png
│   │   └── US_Timezone_NASales_Dashboard.png
│   └── visualizations/
│       ├── Global_NA_Sales_Bar-Line.png
│       ├── GlobalSales_Genre_Bar.png
│       ├── GlobalSales_Genre_Pie.png
│       ├── Global_Sales_Genre_Treemap.png
│       ├── GlobalSales_Genre_Box_Whisker.png
│       ├── GlobalSales_NASales_Genre_PackedBubble.png
│       ├── Global_Sales_EU_Sales_Year_Bin_CF.png
│       ├── GlobalSales_PS_Year_Line.png
│       ├── NASales_Genre_Area.png
│       └── US_States_TimeZone_Map.png
│
└── Tableau_Project_2/
    ├── README.md
    ├── dashboard/
    │   └── Airbnb_Project.png
    └── visualizations/
        ├── Airbnb_AvgPrice_Bedroom_Bar.png
        ├── Distinct-Count_Bedroom-Listings_Table.png
        ├── Airbnb_AvgPrice_zipcode_Map.png
        ├── Airbnb_AvgPrice_zipcode_Bar.png
        └── Airbnb_Revenue_year_line.png


=====================================================
TABLEAU_PROJECT_1/README.md
=====================================================

# Video Game Global Sales Analysis 🎮

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
    ├── Global_NA_Sales_Bar-Line.png
    ├── GlobalSales_Genre_Bar.png
    ├── GlobalSales_Genre_Pie.png
    ├── Global_Sales_Genre_Treemap.png
    ├── GlobalSales_Genre_Box_Whisker.png
    ├── GlobalSales_NASales_Genre_PackedBubble.png
    ├── Global_Sales_EU_Sales_Year_Bin_CF.png
    ├── GlobalSales_PS_Year_Line.png
    ├── NASales_Genre_Area.png
    └── US_States_TimeZone_Map.png
```


=====================================================
TABLEAU_PROJECT_2/README.md
=====================================================

# Airbnb Pricing & Revenue Analysis (Seattle) 🏠

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

## 🔗 Connect

Feel free to explore the visuals above or reach out with questions/feedback!
