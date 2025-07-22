# Megaline Plan Profitability Analysis: #

## Project Overview: ##
Analyzed customer usage data to determine which prepaid plan—Surf or Ultimate—generates more revenue for Megaline. Using a dataset of 500 clients and their monthly activity (calls, texts, and data usage), we performed a statistical and financial analysis to identify the more profitable plan based on user behavior.
**Goal:** Recommend the most profitable plan based on user activity and revenue, supporting Megaline’s data-driven decision-making.
**Business Context:**
Megaline rounds seconds up to minutes, and megabytes to gigabytes. For calls, each individual call is rounded up: even if the call lasted just one second, it will be counted as one minute. For web traffic, individual web sessions are not rounded up. Instead, the total for the month is rounded up. E.g. if someone uses 1025 megabytes this month, they will be charged for 2 gigabytes.

**Surf:**
1)Monthly charge: $20
2)500 monthly minutes, 50 texts, and 15 GB of data
3)After exceeding the package limits:
  .1 minute: 3 cents
  .1 text message: 3 cents
  .1 GB of data: $10

**Ultimate:**
1)Monthly charge: $70
2)3000 monthly minutes, 1000 text messages, and 30 GB of data
3)After exceeding the package limits:
  .1 minute: 1 cent
  .1 text message: 1 cent
  .1 GB of data: $7

## Methods and Implementation: ## 
- Data Preprocessing & EDA:
  .Loaded multiple datasets; cleaned and corrected data types, formatting errors, and duplicates.
  .Consolidated usage data to calculate monthly usage per user for calls, texts, and internet.
- Feature Engineering:
  .Created custom revenue calculation functions based on Megaline’s pricing rules.
  .Aggregated monthly revenue per user.
- Statistical Analysis:
  .Described user behavior (average usage, distribution by plan and region).
  .Plotted distributions and trends using Matplotlib and Seaborn.
  .Calculated means, variances, standard deviations of monthly revenue.
- Hypothesis Tests:
  .Compared average revenue between Surf and Ultimate users.
  .Compared average revenue between NY/NJ users and users from other regions.
  .Used two-sample t-tests to determine statistical significance.

## Tools Used: ##
- Python: pandas, numpy, scipy, matplotlib, seaborn
- Jupyter Notebook

## Key Results: ##
- Identified which plan is more profitable based on actual user behavior.
- Found statistically significant differences in revenue between plans and across regions.
- Delivered data-driven recommendations to optimize Megaline’s marketing and pricing strategy.

## View Project: ##
Full analysis and conclusions are available in the Jupyter Notebook in this repository. 

  
