
# OLA Data Analyst Project

![Power Bi](https://img.shields.io/badge/power_bi-F2C811?style=for-the-badge&logo=powerbi&logoColor=black)
![Microsoft Excel](https://img.shields.io/badge/Microsoft_Excel-217346?style=for-the-badge&logo=microsoft-excel&logoColor=white)
![MYSQL](	https://img.shields.io/badge/MySQL-005C84?style=for-the-badge&logo=mysql&logoColor=white)


## About the Project

This project demonstrates a comprehensive analysis of a dataset containing 20,000 rows of Ola data using **SQL**, **Excel**, and **Power BI**. The primary objective is to extract valuable insights from raw data and present them effectively through interactive visualizations.

### Key Features:
1. **SQL for Data Extraction & Preparation**:
   - Queried a dataset of 20,000 rows to extract relevant information.
   - Cleaned and prepared the data for analysis.
   - Managed complex data structures to address real-world problems.

2. **Excel for Data Analysis**:
   - Conducted in-depth analysis using tools like sorting, pivot tables, and advanced formulas.
   - Summarized data to extract actionable insights.

3. **Power BI for Dashboard Creation**:
   - Created interactive and visually engaging dashboards to present findings.
   - Highlighted trends and key metrics using dynamic visualizations.

4. **End-to-End Workflow Execution**:
   - Executed the complete analytics workflow, from raw data to insightful dashboards.

---

## SQL Queries & Solutions

### Key Queries:
1. **Retrieve all successful bookings**:
    ```sql
    CREATE VIEW Successful_Bookings AS
    SELECT * FROM bookings
    WHERE Booking_Status = 'Success';
    ```
    ![Retrieve all successful bookings](https://github.com/theaadycode/OLA-Data-Analyst-Project/blob/main/SQL%20ss/solution%201.png)

2. **Find the average ride distance for each vehicle type**:
    ```sql
    CREATE VIEW ride_distance_for_each_vehicle AS
    SELECT Vehicle_Type, AVG(Ride_Distance) AS avg_distance
    FROM bookings
    GROUP BY Vehicle_Type;
    ```
    ![average ride distance for each vehicle type](https://github.com/theaadycode/OLA-Data-Analyst-Project/blob/main/SQL%20ss/solution%202.png)

3. **Get the total number of cancelled rides by customers**:
    ```sql
    CREATE VIEW cancelled_rides_by_customers AS
    SELECT COUNT(*) FROM bookings
    WHERE Booking_Status = 'Canceled by Customer';
    ```
    ![total number of cancelled rides by customers](https://github.com/theaadycode/OLA-Data-Analyst-Project/blob/main/SQL%20ss/solution%203.png)

   *(Refer to the document for all SQL queries and answers.)*
[SQL queries and answers.](https://github.com/theaadycode/OLA-Data-Analyst-Project/blob/main/POWER%20BI%20DASHBOARD/1.png)

---

## Power BI Visualizations

### Visualizations:
- **Ride Volume Over Time**: Time-series chart showing the number of rides per day/week.
- **Booking Status Breakdown**: Proportion of different booking statuses using pie/doughnut charts.
- **Top 5 Vehicle Types by Ride Distance**: Bar chart ranking vehicle types.
- **Average Customer Ratings by Vehicle Type**: Column chart showing ratings.
- **Cancelled Rides Reasons**: Bar chart highlighting reasons for cancellations.
- **Revenue by Payment Method**: Stacked bar chart displaying revenue distribution.
- **Top 5 Customers by Total Booking Value**: Leaderboard visual listing top customers.
- **Ride Distance Distribution Per Day**: Histogram or scatter plot.
- **Driver Ratings Distribution**: Box plot of ratings across vehicle types.
- **Customer vs. Driver Ratings**: Scatter plot comparing ratings.

### Placeholder for Dashboard Screenshots:
Please include screenshots of your Power BI dashboard below:

![OLA DATA ANALYTICS PROJECT](https://github.com/theaadycode/OLA-Data-Analyst-Project/blob/main/POWER%20BI%20DASHBOARD/1.png)
![OVERALL](https://github.com/theaadycode/OLA-Data-Analyst-Project/blob/main/POWER%20BI%20DASHBOARD/2.png)
![VEHICLE TYPE](https://github.com/theaadycode/OLA-Data-Analyst-Project/blob/main/POWER%20BI%20DASHBOARD/3.png)
![REVENUE](https://github.com/theaadycode/OLA-Data-Analyst-Project/blob/main/POWER%20BI%20DASHBOARD/4.png)
![CANCELLAION](https://github.com/theaadycode/OLA-Data-Analyst-Project/blob/main/POWER%20BI%20DASHBOARD/5.png)
![RATINGS](https://github.com/theaadycode/OLA-Data-Analyst-Project/blob/main/POWER%20BI%20DASHBOARD/6.png)

---

## Tools & Technologies Used

- **SQL**: Data querying and preparation.
- **Microsoft Excel**: Data analysis and formula-based insights.
- **Power BI**: Interactive dashboard creation.
- **Power Query**: Data transformation and modeling.

---

## End-to-End Workflow Execution
The project covered the following steps:
1. **Data Extraction** (SQL).
2. **Data Cleaning and Preparation** (SQL & Excel).
3. **Data Analysis** (Excel).
4. **Visualization** (Power BI).

---

## How to Access
1. **SQL Queries**:
   - Execute provided queries in your preferred SQL environment after setting up the `Ola` database.

2. **Excel Files**:
   - Refer to the `.xlsx` file for in-depth analysis.

3. **Power BI Dashboard**:
   - Open the `.pbix` file in Power BI Desktop.

