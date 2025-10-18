# Marketing Campaign Analysis Dashboard - Fast-Food Product Launch
---
## Project Overview
- **Project Description:** This project applies A/B testing principles to evaluate the effectiveness of three marketing promotions (Promo 1, Promo 2, and Promo 3) for a fast-food chain launching a new product. Using Looker Studio and Google Sheets, the project evaluates which promotion drives the highest per-location sales and provides actionable business recommendations.
- **Project Goal:** Evaluate promotional campaign performance and identify which promotion should be scaled, redesigned, or discontinued.

## Tools Used
Google Sheets, Excel

## Dataset Summary
|Column	          | Description                                        |
|-----------------|----------------------------------------------------|
|MarketID	        | Unique identifier for each market                  |
|MarketSize	      | size of market area by sales (Small, Medium, Large)|
|LocationID	      | Unique identifier for store location               |
|AgeOfStore	      | Store age in years                                 |
|Promotion	      | One of three promotions that were tested           |
|Week             |	One of four weeks when the promotions were run     |
|SalesInThousands | Sales amount                                       |

- **Dataset Size:** 543 rows * 7 columns
- **Data Source:**  Kaggle - Fast Food Marketing Campaign A/B Test by Anastasia Chebotina

## Data Cleaning and Preparation
- Verified numeric types in SalesInThousands
- **Derived Column:** I added a revenue column, converting the SalesInThousands entires, which were in decimals to thousands.

## Descriptive Analysis
- **Total Revenue:** Calculated the total overall revenue -
- **Total Revenue for each Promotion:** shows total revenue for each promotion, to identify which campaign generated the most total revenue.
- **Mean Weekly Sales per Promotion:** gives the average revenue per week for each promotion, to know which campaign performs best on average.
- **Median Weekly Sales per Promotion:** gives the median revenue per week for each promotion, to control for outliers.
- **% Lift Vs Baseline Promotion:** using Promo 1 as the baseline, to show how much better one promotion performs compared to another.
- **Week-over-Week Change (%):** to track how performance changes over time
- **Promo Win Rate (Weeks Won):** to tell how consistent a promo’s success is.
- **Market Size Performance:** to show which market segment (Large, Medium, Small) is most profitable under each promotion.
- **Locations Above Target:** to measure how many store locations achieved strong sales under each promotion.

## Dashboard Overview

Live Dashboard: [View on Looker Studio](https://lookerstudio.google.com/reporting/1a947eb6-5ad5-410f-b8a4-0849ecc3bd95/page/uT5bF/edit)

## Insights Summary 
- Promo 1 is most efficient per store (best average/median sales, 100+ high-performing stores)
- Promo 3 is strongest in large markets and highest total revenue.
- Promo 2 is weakest; should be paused or redesigned.
- Week-over-week trends stable (small variances <5%)
- Market segmentation shows differing promo effectiveness

## Recommendations
- Scale Promo 1 across all markets for consistent per-store performance.
- Pilot Promo 3 only in large markets for possible scalability.
- Discontinue or redesign Promo 2 to minimize inefficiency.
- Collect promotion cost data to measure Return on Investment (ROI) and Return on Ad Spend (ROAS).
- Extend experiment to 8 weeks for trend confirmation.

