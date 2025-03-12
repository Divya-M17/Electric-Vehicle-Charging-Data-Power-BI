# EV Charging Data Analyis - Power BI 

# Project Overview
The EV Charging Data Analysis project aims to analyze electric vehicle (EV) charging trends, customer behavior, station performance, and revenue generation using Power BI. The insights derived help optimize charging station operations, improve customer satisfaction, and enhance profitability.

# Technologies Used
1. Power BI – Data visualization & dashboard creation
2. Excel – Data cleaning & preprocessing
3. DAX (Data Analysis Expressions) – Advanced calculations & measures

# Key Objectives
1. Understand charging trends over time
2. Analyze customer behavior based on subscription plans
3. Evaluate charging station performance
4. Assess revenue patterns & profitability
5. Optimize charging station operations using data insights

# Power BI Dashboard Insights
  1. Time-Based Charging Trends:
  - Peak Charging Hours: High demand between 6 PM - 9 PM
  - Weekday vs. Weekend Usage: More sessions recorded on weekends
  - Monthly Trends: Growing EV adoption observed over time

  2. Charging Station Performance
  - Top Stations by Energy Consumption: Station ST0003 had the highest energy usage
  - Station Utilization Heatmap: Identified underperforming stations for optimization
  - Revenue per Station: Helped determine most profitable locations

  3. Customer Behavior Analysis
  - Most Active Customers: Key users contributed significantly to revenue
  - Subscription Type Trends: Annual subscribers had the highest engagement
  - Battery Level Before & After Charging: Provided insights into charging efficiency

  4. Performance by Revenue Analysis
  - Total Revenue Trends: Month-on-month revenue growth observed
  - Energy Consumption vs. Revenue: Correlation between high energy usage and revenue
  - Utilization Rate: Helped allocate resources efficiently

# DAX Queries Used
- Total Charging Sessions
CALCULATE(COUNT(Sessions[Session ID]))

- Revenue Per Station
SUMX(Stations, Stations[Cost Per Session] * Stations[Total Sessions])

- Average Energy Consumption
AVERAGE(Sessions[Energy Consumed (kWh)])

- Peak Hour Usage
MAX(ChargingData[Session Count])

- Utilization Rate Calculation
(Total Sessions / Available Slots) * 100

# Business Impact
1. Optimized charging infrastructure by identifying high-demand areas
2. Improved revenue forecasting through data-driven pricing strategies
3. Enhanced customer engagement by analyzing subscription trends
4. Increased operational efficiency with better station utilization insights


# Conclusion
This project demonstrates data-driven decision-making using Power BI and DAX, helping businesses optimize EV charging operations. The interactive dashboard provides actionable insights to improve station performance, customer experience, and revenue generation.
