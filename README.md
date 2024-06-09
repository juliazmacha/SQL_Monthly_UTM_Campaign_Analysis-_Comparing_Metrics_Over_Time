# Monthly UTM Campaign Analysis: Comparing Metrics Over Time

This project builds on a previous analysis of UTM parameters and ad performance metrics for Google and Facebook ads. The goal is to create a monthly sample and compare key metrics over time. The following steps outline the process.

## Steps Undertaken

### Step 1: Use Previous CTE in a New CTE
The first CTE from the previous task was utilized within a new (second) CTE to create a sample with the following data:
- **ad_month**: The first day of the month derived from `ad_date`.
- **utm_campaign**: The UTM campaign parameter, with the same conditions applied as in the previous task.
- **Aggregated Metrics**: Total cost, number of impressions, number of clicks, conversion value, CTR, CPC, CPM, and ROMI, with the same conditions applied as in the previous task.

### Step 2: Select Resulting Fields
A selection was made from the resulting data to include the following fields:
- **ad_month**: The first day of the month.
- **utm_campaign**: The UTM campaign parameter.
- **Total Cost**
- **Number of Impressions**
- **Number of Clicks**
- **Conversion Value**
- **CTR (Click-Through Rate)**
- **CPC (Cost Per Click)**
- **CPM (Cost Per Thousand Impressions)**
- **ROMI (Return on Marketing Investment)**

### Step 3: Calculate Monthly Metric Differences
For each `utm_campaign` in each month, new fields were added to calculate the percentage difference in CPM, CTR, and ROMI compared to the previous month. This involved:
- Calculating the difference between the current month's and the previous month's values for CPM, CTR, and ROMI.
- Converting these differences to percentages.

## Final Product
The resulting analysis provides a comprehensive view of how key ad performance metrics for UTM campaigns change over time on a monthly basis. By comparing metrics such as CPM, CTR, and ROMI from one month to the next, this project helps to identify trends and changes in campaign effectiveness, enabling more informed decision-making.

