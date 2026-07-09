1. Project Title
📱 PhonePe Analytics Dashboard: Interactive Digital Payment & User Insights

A comprehensive, interactive Power BI dashboard inspired by the PhonePe ecosystem, built to analyze digital payment transactions, customer behavior, user growth, service performance, and geographic trends. The dashboard enables business users to monitor KPIs, explore transaction patterns, and make data-driven decisions through an intuitive and modern analytics experience.

2. Short Description

The PhonePe Analytics Dashboard is an end-to-end Business Intelligence solution developed using Power BI to provide meaningful insights into digital payment transactions and customer engagement. It enables users to analyze transaction performance, monitor user growth, evaluate payment success rates, and explore service-wise and geographical trends using interactive visualizations, dynamic KPIs, bookmarks, slicers, and advanced DAX calculations.

3. Tech Stack

The dashboard was built using the following tools and technologies:

📊 Power BI Desktop – Primary platform used to design and develop interactive dashboards.
📂 Power Query – Used for data extraction, cleaning, transformation, and preparation (ETL).
🧠 DAX (Data Analysis Expressions) – Implemented advanced measures including Time Intelligence, Running Totals, MoM Growth, Rankings, Average Spend, Success Rate, and Dynamic KPIs.
🗂️ Data Modeling – Designed a Star Schema with fact and dimension tables to optimize performance.
🎛️ Bookmarks & Navigation Buttons – Created a multi-page interactive dashboard with seamless navigation between report sections.
🎚️ Slicers & Filters – Enabled dynamic filtering by Month, Service, Generation, Geography, and Payment Status.
🎨 Custom UI Design – Applied a PhonePe-inspired purple theme with modern KPI cards, custom icons, and responsive layouts.
📁 File Formats – .pbix for Power BI development, .xlsx as the data source, and .png for dashboard previews.

4. Data Source

Source: Simulated PhonePe Digital Payments Dataset (Excel)

The dataset contains realistic digital payment records and user information designed to replicate a fintech environment.

📋 Dataset Structure
Table 1: All_Transactions (Fact Table)

This table stores transaction-level information and serves as the primary fact table for analysis.

Columns:

Transaction_ID
User_ID
Amount
Service
Service_Type
Payment_Status
Reason
Date

Table 2: All_Users (Dimension Table)

This table contains customer information and is used for user analytics.

Columns:

User_ID
Name
Age
Join_Date

Using Power Query, an additional calculated column Age Segment was created to categorize users into generational groups:

Gen Z
Millennials
Gen X
Baby Boomers

This transformation enables demographic analysis and customer segmentation throughout the dashboard.

🔄 Data Transformation (Power Query)

Power Query was used to perform the ETL (Extract, Transform, Load) process before building the dashboard. Key transformations included:

Data Cleaning
Data Type Conversion
Renaming Columns
Creating the Age Segment column based on user age
Handling missing values (where applicable)
Preparing data for efficient reporting

🗄️ Data Model
A Star Schema data model was implemented to optimize performance and support interactive reporting.

Fact Table
All_Transactions

Dimension Table
All_Users

A relationship was established using User_ID to enable accurate filtering, aggregation, and cross-analysis between transaction and user data.

5. Features / Highlights
📌 Business Problem

Digital payment platforms process millions of transactions daily across multiple services and regions. Business teams require a centralized analytics solution to monitor transaction performance, user engagement, payment success, and growth trends. Raw transactional data makes it difficult to quickly answer questions such as:

Which services generate the highest transaction volume?
How is transaction value changing over time?
Which customer generation contributes the most?
What is the monthly user growth rate?
Which states drive the highest transaction value?
Who are the top customers by spending?
What is the payment success rate?

🎯 Goal of the Dashboard

The primary objective of this dashboard is to provide an interactive analytics platform that enables users to:

Monitor digital payment performance in real time.
Analyze transaction trends and business growth.
Track customer acquisition and engagement.
Compare service-wise transaction performance.
Evaluate payment success and failure trends.
Explore geographical performance across states.
Support business decision-making through dynamic reporting and KPIs.

📊 Walkthrough of Key Visuals
Executive KPI Cards

The dashboard displays key business metrics at the top of the report, including:

Total Transaction Value
Total Transactions
Registered Users
Average Transaction Value
Average Spend per User
Monthly Transaction Growth
User Growth %
Payment Success Rate

These KPIs are fully interactive and update dynamically based on the selected filters and slicers.

📈 Monthly Transaction Trend (Line Chart)

Displays the monthly trend of transaction value, allowing users to monitor business performance over time, identify seasonal patterns, and evaluate month-over-month growth.

Business Insight:

Tracks transaction growth trends.
Identifies peak and low-performing months.
Supports performance monitoring over time.
👥 User Growth Over Time (Area Chart)

Visualizes the cumulative growth of registered users over time, providing insights into customer acquisition and platform adoption.

Business Insight:

Monitors user acquisition trends.
Evaluates platform growth.
Helps assess customer expansion over time.
🆕 Monthly Registration of Users (Column Chart)

Shows the number of newly registered users each month based on their registration date.

Business Insight:

Measures monthly customer acquisition.
Identifies registration trends.
Evaluates the effectiveness of user onboarding initiatives.
💰 Transaction Value by Service (Column Chart)

Compares the total transaction value generated by different PhonePe services such as Recharge, Bill Payments, UPI, Insurance, Investments, and Shopping.

Business Insight:

Identifies high-revenue services.
Supports service performance evaluation.
Helps prioritize business strategies for top-performing categories.
💳 Transactions by Service (Column Chart)

Displays the total number of transactions performed across various services.

Business Insight:

Highlights the most frequently used services.
Measures customer engagement by service.
Assists in understanding service popularity.
📊 Transactions by Payment Status (Bar Chart)

Breaks down transactions based on their payment status, including Successful, Failed, and Pending transactions.

Business Insight:

Monitors payment reliability.
Identifies failed transaction patterns.
Supports operational improvements to increase payment success rates.
🥧 Weekday vs Weekend Transactions (Pie Chart)

Compares transaction activity between weekdays and weekends to analyze customer payment behavior.

Business Insight:

Identifies peak transaction periods.
Helps businesses optimize promotional campaigns and operational planning.
Reveals customer usage patterns throughout the week.
🏆 Top 5 Users by Transaction Value (Column Chart)

Ranks the top five users based on their total transaction value.

Business Insight:

Identifies high-value customers.
Supports customer segmentation.
Helps businesses design targeted loyalty and retention strategies.
👨‍👩‍👧‍👦 Transactions by Generation (Tooltip)

An interactive tooltip appears when hovering over the Transaction by Generation visual, providing additional insights beyond the main chart.

The tooltip displays:

Total Transactions
Transaction Value
Registered Users
Average Transaction Value
Average Spend per User

Business Insight:

Compares transaction behavior across Gen Z, Millennials, Gen X, and Baby Boomers.
Helps understand demographic spending habits.
Supports customer segmentation and targeted marketing.
🏷️ Transaction Value by Service Type (Tooltip)

A custom tooltip provides a detailed breakdown of transaction value by Service Type whenever users hover over service-related visuals.

The tooltip includes:

Total Transaction Value
Total Transactions
Average Transaction Value
Payment Success Rate
Percentage Contribution

Business Insight:

Enables deeper analysis of individual service categories.
Highlights service-wise revenue contribution.
Assists in identifying the most profitable service types.
🎛️ Interactive Filters & Slicers

The dashboard includes dynamic slicers that allow users to explore data from multiple perspectives.

Available slicers:

Month
Service
Generation

All visuals update instantly through cross-filtering, enabling flexible and interactive analysis.

🔖 Bookmarks & Navigation

The dashboard incorporates Bookmarks and Navigation Buttons to create a seamless user experience.

Users can navigate between:

🏠 Overview
💳 Transactions
👥 Users

This provides an application-like interface, improving usability and enabling faster access to different analytical views without leaving the report page.

6.Screenshots

Show what the dashboard looks like. Example:
<img width="1920" height="1080" alt="Screenshot (1225)" src="https://github.com/user-attachments/assets/316d2001-bab6-4e85-a0a7-d5231871a362" />
<img width="1920" height="1080" alt="Screenshot (1226)" src="https://github.com/user-attachments/assets/e5ee66c1-3cc4-44df-9505-515b47bb8ab3" />
<img width="1920" height="1080" alt="Screenshot (1227)" src="https://github.com/user-attachments/assets/017d8e68-da39-49f8-87f1-02353e9a823a" />



