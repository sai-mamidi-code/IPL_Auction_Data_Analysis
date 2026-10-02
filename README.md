# IPL 2023 Auction Data Analysis & Power BI Dashboard

An end-to-end analysis of the IPL 2023 player auction: cleaning a 568-player dataset, exploring spending patterns, and presenting the results in an interactive Power BI dashboard.

> **Note:** Data cleaning and exploratory analysis were done with **Julius AI**. The Power BI dashboard was built by me.

## Objective

To understand where the money went in the IPL 2023 auction: which teams spent the most, which player types were in demand, who the top buys were, and how many players went unsold.

## Key Findings

- **₹167 Cr** was spent across **80 actual auction purchases**.
- Of the 568 records, **325 players (57%) went unsold** and **163 were retained** by their teams at zero auction cost.
- **Sunrisers Hyderabad** spent the most at the auction (**₹35.7 Cr**), followed by Mumbai Indians (₹20.5 Cr) and Punjab Super Kings (₹20 Cr).
- **Sam Curran** was the most expensive buy at **₹18.5 Cr** (PBKS), followed by Cameron Green (₹17.5 Cr) and Ben Stokes (₹16.25 Cr).
- **All-rounders** drew about **42%** of total spend (₹70.75 Cr), ahead of batsmen (₹36.5 Cr), bowlers (₹32.15 Cr) and wicketkeepers (₹27.6 Cr).
- **All-rounders (126) and bowlers (104)** made up most of the unsold players.

## Data Cleaning

- Standardized column names and data types.
- Split **retained players** (163) from **actual auction purchases** (80) so zero-cost retentions would not distort price analysis.
- Checked missing values and verified recorded totals against the source data.

## Dashboard

The Power BI dashboard includes:

- **KPI cards:** Total Auction Spending, Actual Purchases, Retained Players, Unsold Players
- **Slicers:** filter by Player Type (and a second slicer)
- **Visuals:**
  - Team-wise Auction Spending
  - Top 10 Most Expensive Players
  - Auction Spending by Player Category
  - Players Purchased by Team
  - Unsold Players by Category
  - Share of Total Auction Spending
  - Base Price vs Purchase Price (scatter)

<!-- Add dashboard screenshot here: ![Dashboard](images/dashboard.png) -->

## Repository Structure

```
IPL_Auction_Data_Analysis/
├── Raw_dataset/
│   └── IPL_Squad_2023_Auction_Dataset_Raw.csv
├── Cleaned_dataset/
│   ├── IPL_Auction_Cleaned.csv
│   ├── IPL_Auction_EDA_Tables.xlsx
│   └── IPL_Auction_EDA_Charts.pdf
├── Power BI Dashboard/
│   └── IPL_Auction_Dashboard.pbix
└── README.md
```

## Dataset Columns (cleaned)

| Column | Description |
|---|---|
| Player | Player name |
| Base_Price | Base price (or retained marker) |
| Player_Type | Batsman, Bowler, All-rounder, Wicketkeeper |
| Cost_Cr | Auction price in ₹ crore |
| Cost_USD_000 | Auction price in thousand USD |
| Squad_2022 | Team in the 2022 season |
| Team | Team for 2023 |
| Auction_Status | Sold / Unsold |

## Tools Used

- **Julius AI** for data cleaning and exploratory analysis
- **Excel** for EDA summary tables
- **Power BI** for the interactive dashboard

## How to View

1. Clone or download this repository.
2. Open `Power BI Dashboard/IPL_Auction_Dashboard.pbix` in Power BI Desktop.
3. Browse `Cleaned_dataset/` for the cleaned data and EDA outputs.

## Author

**Sai Kumar Mamidi**
