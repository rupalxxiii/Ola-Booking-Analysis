OLA Data Analytics Project
Project Overview

This project is an end-to-end Data Analytics Dashboard built using SQL, Power BI, and Excel/CSV datasets to
analyze ride booking data for an OLA-like cab service platform.

The project focuses on:
 • Ride booking trends
 • Customer & driver behavior
 • Revenue analysis
 • Cancellation insights
 • Ratings analysis
 • Vehicle performance metrics

The dashboard helps derive actionable business insights from ride-booking operations.
Tech Stack
 • SQL – Data cleaning, querying, and analysis
 • Power BI – Interactive dashboard creation
 • Excel / CSV – Dataset source
 • DAX – Calculated measures and KPIs

Project Files
 Bookings.csv – Raw ride booking dataset
 ola_booking.sql – SQL queries and views
 ola analysis.pbix – Power BI dashboard
 README.md – Project documentation

Dashboard Features
 1. Overall Analysis
 • Ride Volume Over Time
 • Booking Status Breakdown
 • Total Bookings
 • Successful vs Cancelled Rides

2. Vehicle Type Analysis
 • Top Vehicle Types by Ride Distance
 • Vehicle-wise Customer Ratings
 • Vehicle Usage Distribution

3. Revenue Analysis
 • Revenue by Payment Method
 • Top Customers by Booking Value
 • Daily Revenue Trends

4. Cancellation Analysis
 • Customer Cancellation Reasons
 • Driver Cancellation Reasons
 • Cancellation Percentage

5. Ratings Analysis
 • Driver Rating Distribution
 • Customer Rating Distribution
 • Customer vs Driver Ratings Comparison

Dataset Information
The dataset contains ride booking details for Bengaluru city with columns such as:
 • Date
 • Time
 • Booking ID
 • Booking Status
 • Customer ID
 • Vehicle Type
 • Pickup Location
 • Drop Location
 • Ride Distance
 • Booking Value
 • Payment Method
 • Driver Ratings
 • Customer Ratings
 • Cancellation Reasons

Key Insights
 • Majority of bookings were completed successfully.
 • Weekend ride demand was significantly higher.
 • UPI was the most preferred payment method.
 • Prime Sedan and SUV rides generated higher revenue.
 • Customer cancellations were lower compared to driver cancellations.
 • Ratings analysis helped identify service quality trends.

SQL Analysis Performed

 -- Retrieve successful bookings
 SELECT *
 FROM bookings
 WHERE Booking_Status = 'Success';

-- Average ride distance by vehicle type
 SELECT Vehicle_Type,
 AVG(Ride_Distance) AS avg_distance
 FROM bookings
 GROUP BY Vehicle_Type;

-- Total successful booking revenue
 SELECT SUM(Booking_Value)
 FROM bookings
 WHERE Booking_Status = 'Success';

Power BI Visualizations
 • Line Charts
 • Pie Charts
 • Bar Charts
 • KPI Cards
 • Scatter Plots
 • Rating Distribution Charts
 • Revenue Analysis Dashboards

How to Run the Project
SQL:
 1. Import the dataset into MySQL.
 2. Run the SQL queries from ola_booking.sql.

Power BI:
 1. Open ola analysis.pbix.
 2. Refresh the dataset connection.
 3. Explore the interactive dashboard.

Learning Outcomes
 • SQL querying and data analysis
 • Data cleaning and transformation
 • Power BI dashboard development
 • Data storytelling techniques
 • Business KPI analysis

Future Improvements
 • Real-time dashboard integration
 • Predictive ride demand analysis
 • Driver performance forecasting
 • Geo-location based ride analysis

Author
 Rupal Hiwarkar
 Data Analytics Enthusiast
 Skilled in SQL, Power BI, Excel, and Data Visualization

Support
If you like this project, give this repository a star on GitHub and feel free to fork or contribute!
