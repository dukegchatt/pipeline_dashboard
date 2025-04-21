# pipeline_dashboard

Overview
This Power BI dashboard provides comprehensive visibility into logistics operations by analyzing Good Invoice (GI) data across multiple warehouses. The dashboard offers real-time insights into key operational metrics including delivery orders, productivity trends, and pallet utilization.
Features

Multi-Warehouse Analysis: Track performance across 6 warehouses (CA S11, TX S35, NJ S31, IL S34, Canada S37, WA S36)
Comprehensive Metrics: Monitor DO counts, productivity, quantities, pallet trends, and KPIs
Time-Based Analysis: Filter data by months and years with interactive slicers
Dynamic Calculations: View counts for specific selections or averages when multiple periods are selected

Data Pipeline
The dashboard is powered by a sophisticated data pipeline:

Data Sourcing & Cleaning: Raw data is processed using Excel and Python
Storage & Integration: Cleaned data is uploaded to Azure Blob Storage
Data Warehouse: Data is transferred to Snowflake for structured storage
Visualization: SQL queries pull relevant data into Power BI for visualization

Key Metrics
Primary KPIs

Delivery Orders (DO): Total count and weighted values
Workday: Current operational workdays (80)
Manpower: Current manpower allocation (29.28)
Productivity KPI: Current value of 58.92 against a goal of 78.24 (-24.7%)

Secondary Metrics

DO Count Per Week: Weekly trend of delivery orders
Count by WH: Breakdown of counts by warehouse location
Productivity Trend: Performance over time periods
Quantity Trend: Volume of goods processed
Pallet Trend: Pallet utilization tracking
Pallet Average: Current average of 5,558 pallets

Type Breakdown

SP: 44.93% (292,885 units)
Other categories including TZ, LT, CP, PN, and FT with varying percentages

Usage Instructions
Filtering Data

Use the left sidebar to filter by warehouse location (CA S11, TX S35, etc.)
Use year and month selectors at the bottom of the sidebar for time-based filtering
When a specific month is selected, the dashboard shows counts for that period
When multiple months are selected, the dashboard displays averages

Interpreting Visuals

Line charts show trends over time periods
Bar charts compare performance across warehouses
The pie chart breaks down invoice types
KPI indicators show performance against targets

Technical Details

Platform: Microsoft Power BI
Data Sources:

Snowflake data warehouse
Azure Blob Storage


Maintenance

Data is processed through the ETL pipeline described above
Updates to the dashboard can be made through the Power BI service
For data source changes, adjustments may be needed in the Python scripts and SQL queries
