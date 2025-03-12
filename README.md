# EV Charging Data Analysis - Power BI 

# Project Overview 
The EV Charging Data Analysis project focuses on analyzing electric vehicle charging patterns, customer behaviors, station performance, and revenue generation. The insights derived from this analysis help optimize charging station operations and improve user experience.

# Tools & Technologies Used
- **Power BI** – Data visualization & dashboard creation
- **SQL** – Data extraction & transformation
- **Excel** – Data cleaning & preprocessing
- **DAX (Data Analysis Expressions)** – Advanced calculations & measures

# Key Objectives:**
1. **Understand charging trends** over time.
2. **Analyze customer behavior** based on subscription plans and usage.
3. **Evaluate station performance** to identify top-performing locations.
4. **Assess revenue patterns** and profitability.
5. **Optimize charging station operations** using data-driven insights.

# Dashboard Insights:**
# Time-Based Charging Trends**
- **Peak Charging Hours:** Identifies high-demand hours to optimize station availability.
- **Weekday vs. Weekend Usage:** Highlights behavioral patterns for strategic planning.
- **Monthly Charging Trends:** Tracks charging growth and seasonal variations.

# 2. Charging Station Performance**
- **Top 10 Stations by Energy Consumption:** Helps identify high-usage locations.
- **Station Utilization Heatmap:** Displays station-wise session distribution.
- **Revenue per Station:** Determines financial contribution of each station.

# Customer Behavior Analysis**
- **Most Active Customers:** Identifies users with high engagement.
- **Subscription Plan Trends:** Analyzes usage distribution among different subscription types.
- **Battery Level Patterns:** Shows energy consumption efficiency before and after charging.

# Performance by Revenue Analysis**
- **Total Revenue by Month:** Monitors revenue generation trends.
- **Energy Consumption vs. Revenue:** Evaluates profitability based on energy usage.
- **Utilization Rate:** Helps determine station efficiency and demand.

# DAX Queries Used
1. **Total Charging Sessions:** `CALCULATE(COUNT(Sessions[Session ID]))`
2. **Revenue Per Station:** `SUMX(Stations, Stations[Cost Per Session] * Stations[Total Sessions])`
3. **Average Energy Consumption:** `AVERAGE(Sessions[Energy Consumed (kWh)])`
4. **Peak Hour Usage:** `MAX(ChargingData[Session Count])`
5. **Utilization Rate Calculation:** `(Total Sessions / Available Slots) * 100`


# Key Business Impact
- **Improved Operational Efficiency:** Identified peak usage times to optimize resource allocation.
- **Enhanced Revenue Forecasting:** Provided insights into profitable stations and revenue streams.
- **Better Customer Experience:** Helped in subscription plan optimization and service improvements.
- **Data-Driven Decision Making:** Enabled strategic placement of charging stations in high-demand areas.


# Conclusion
This Power BI project effectively showcases the power of data-driven insights in optimizing EV charging infrastructure. The dashboard provides actionable insights that help businesses enhance their operations, improve customer satisfaction, and maximize revenue.
