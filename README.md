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
  You can view and download the dataset [here](https://github.com/Winner-Dimiri/Marketing-Campaign-Analysis-Dashboard-A-B-Testing-Looker-Studio-Google-Sheets/blob/main/Marketing%20Campaign%20Data%20-%20Campaign_Data.csv)


## Data Cleaning and Preparation
- Verified numeric types in SalesInThousands
- **Derived Column:** I added a revenue column, converting the SalesInThousands column to thousand.

## Descriptive Analysis
- **Total Revenue:** Calculated the total overall revenue

![](https://github.com/Winner-Dimiri/Marketing-Campaign-Analysis-Dashboard-A-B-Testing-Looker-Studio-Google-Sheets/blob/main/Total%20Total%20Revenue%20Function.png)

![](https://github.com/Winner-Dimiri/Marketing-Campaign-Analysis-Dashboard-A-B-Testing-Looker-Studio-Google-Sheets/blob/main/Total%20Total%20Revenue%20Output.png)

- **Total Revenue for each Promotion:** shows total revenue for each promotion, to identify which campaign generated the most total revenue.

![](https://github.com/Winner-Dimiri/Marketing-Campaign-Analysis-Dashboard-A-B-Testing-Looker-Studio-Google-Sheets/blob/main/Total%20Revenue%20Function.png)

![](https://github.com/Winner-Dimiri/Marketing-Campaign-Analysis-Dashboard-A-B-Testing-Looker-Studio-Google-Sheets/blob/main/Total%20Revenue%20Output.png)


- **Mean Weekly Revenue per Promotion:** gives the average revenue per week for each promotion, to know which campaign performs best on average.

![](https://github.com/Winner-Dimiri/Marketing-Campaign-Analysis-Dashboard-A-B-Testing-Looker-Studio-Google-Sheets/blob/main/Average%20Revenue%20Weekly%20Function.png)

![](https://github.com/Winner-Dimiri/Marketing-Campaign-Analysis-Dashboard-A-B-Testing-Looker-Studio-Google-Sheets/blob/main/Average%20Revenue%20Weekly%20Output.png)

- **Median Revenue and Median Weekly Revenue per Promotion:** gives the median revenue per week for each promotion, to control for outliers.

![](https://github.com/Winner-Dimiri/Marketing-Campaign-Analysis-Dashboard-A-B-Testing-Looker-Studio-Google-Sheets/blob/main/Median%20Revenue%20Function.png)

![](https://github.com/Winner-Dimiri/Marketing-Campaign-Analysis-Dashboard-A-B-Testing-Looker-Studio-Google-Sheets/blob/main/Median%20Revenue%20Output.png)

![](https://github.com/Winner-Dimiri/Marketing-Campaign-Analysis-Dashboard-A-B-Testing-Looker-Studio-Google-Sheets/blob/main/Median%20Weekly%20Revenue%20Function.png)

![](https://github.com/Winner-Dimiri/Marketing-Campaign-Analysis-Dashboard-A-B-Testing-Looker-Studio-Google-Sheets/blob/main/Median%20Revenue%20Weekly%20Output.png)

- **% Lift Vs Baseline Promotion:** using Promo 1 as the baseline, to show how much better one promotion performs compared to another.

![](https://github.com/Winner-Dimiri/Marketing-Campaign-Analysis-Dashboard-A-B-Testing-Looker-Studio-Google-Sheets/blob/main/Lift%20Vs%20Baseline%20Promo%20Function.png)

![](https://github.com/Winner-Dimiri/Marketing-Campaign-Analysis-Dashboard-A-B-Testing-Looker-Studio-Google-Sheets/blob/main/Lift%20Vs%20Baseline%20Promo%20Output.png)

- **Week-over-Week Change (%):** to track how performance changes over time.

![](https://github.com/Winner-Dimiri/Marketing-Campaign-Analysis-Dashboard-A-B-Testing-Looker-Studio-Google-Sheets/blob/main/Week%20Over%20Week%20Function.png)

![](https://github.com/Winner-Dimiri/Marketing-Campaign-Analysis-Dashboard-A-B-Testing-Looker-Studio-Google-Sheets/blob/main/Week%20Over%20Week%20Output.png)

- **Promo Win Rate (Weeks Won):** to tell how consistent a promo’s success is.

![](https://github.com/Winner-Dimiri/Marketing-Campaign-Analysis-Dashboard-A-B-Testing-Looker-Studio-Google-Sheets/blob/main/Promo%20Win%20Rate%20Function%201.png)

![](https://github.com/Winner-Dimiri/Marketing-Campaign-Analysis-Dashboard-A-B-Testing-Looker-Studio-Google-Sheets/blob/main/Promo%20Win%20Output%201.png)

![](https://github.com/Winner-Dimiri/Marketing-Campaign-Analysis-Dashboard-A-B-Testing-Looker-Studio-Google-Sheets/blob/main/Promo%20Win%20Rate%20Function%202.png)

![](https://github.com/Winner-Dimiri/Marketing-Campaign-Analysis-Dashboard-A-B-Testing-Looker-Studio-Google-Sheets/blob/main/Promo%20Win%20Rate%20Output.png)

- **Market Size Performance:** to show which market segment (Large, Medium, Small) is most profitable under each promotion.

![](https://github.com/Winner-Dimiri/Marketing-Campaign-Analysis-Dashboard-A-B-Testing-Looker-Studio-Google-Sheets/blob/main/Market%20Size%20Performance%20Function.png)

![](https://github.com/Winner-Dimiri/Marketing-Campaign-Analysis-Dashboard-A-B-Testing-Looker-Studio-Google-Sheets/blob/main/Market%20Size%20Performance%20Output.png)

- **Locations Above Target:** to measure how many store locations achieved strong sales under each promotion.

![](https://github.com/Winner-Dimiri/Marketing-Campaign-Analysis-Dashboard-A-B-Testing-Looker-Studio-Google-Sheets/blob/main/Locations%20Above%20Target%20Function.png)

![](https://github.com/Winner-Dimiri/Marketing-Campaign-Analysis-Dashboard-A-B-Testing-Looker-Studio-Google-Sheets/blob/main/Locations%20Above%20Target%20Output.png)

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

