# A/B Testing Analysis of Digital Marketing Campaign


## Overview

This A/B Testing Project captures the outcomes of an A/B test run by marketing companies to evaluate whether advertising exposure influences purchasing behavior, and how exposure patterns vary among users. The analysis explores conversion rates, optimal timing for ad delivery, and various factors affecting user engagement using statistical methods and data visualization in R. 

## Report

The complete analysis is available in the [HTML Report](./report.html) or [PDF Report](./A_B%20Testing%20Analysis%20of%20Digital%20Marketing%20Campaign.pdf), which provides detailed explanations, statistical results, and visualizations of the A/B testing campaign.

## Dataset Information

The analysis uses the `marketing_AB.csv` dataset which contains the following variables:
- `user.id`: Unique identifier for each user
- `test.group`: Group assignment (either "ad" or "psa")
- `converted`: Conversion status (TRUE/FALSE)
- `total.ads`: Total number of advertisements shown to the user
- `most.ads.day`: Day of the week with highest ad impressions
- `most.ads.hour`: Hour of the day with highest ad impressions
- `most.ads.time`: Time of day category (Morning, Afternoon, Evening, Night)

## Analysis Highlights

1. **Exploratory Data Analysis**
   - Distribution of test groups, conversion status, and ad impressions
   - Time-based patterns in ad delivery and user engagement

2. **Statistical Testing**
   - Pearson’s Chi-square test for independence to determine association of temporal patterns and conversion rates
   - Z-test for equality of proportions to compare conversion rates between ad (treatment) and PSA (control) groups
   - Welch’s Two-Sample t-test for difference in means of ads seen between converted and non-converted users 
   - Power analysis to validate sample size adequacy

3. **Key Findings**
   - Significant difference in conversion rates between traditional ads and PSAs
   - Identified optimal days and times for ad delivery to maximize conversions
   - Correlation between ad frequency and conversion likelihood

## Visualizations

The report includes several visualizations:
- Conversion rate comparisons between test groups
- Distribution of ad impressions by time of day and day of week
- Heatmap showing conversion rates by day and hour
- Bar charts displaying conversion patterns

## Technical Implementation

This analysis was conducted using R with the following key packages:
- ggplot2 for data visualization
- scales for formatting chart values
- stats for statistical testing

## Getting Started

To reproduce this analysis:

1. Clone this repository
2. Ensure R is installed on your machine
3. Install required R packages
4. Open the `script.Rmd` file in RStudio
5. Execute the code to generate the report


## Author

[Dang Le](https://www.linkedin.com/in/hdang-le3107/)
