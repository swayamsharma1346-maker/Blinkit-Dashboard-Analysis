# Blinkit-Dashboard-AnalysisBlinkit Sales Analysis Dashboard Using Power BI

Blinkit Sales Analysis Dashboard | Power BI


Project Overview
The Blinkit Sales Analysis Dashboard is an interactive business
intelligence report created in Microsoft Power BI. It analyzes grocery
sales using product-level and outlet-level information. The report is
designed to help users explore sales performance, compare product
categories, and understand how outlet characteristics relate to sales.

The supplied Power BI file is a .pbit template. It contains the
report layout and data model definitions; a connected or loaded dataset
is needed to populate the visuals with live values.

Business Objective
The purpose of this dashboard is to provide a consolidated view of
Blinkit's grocery sales data and make it easier to explore:
- Sales contribution by item type and fat-content category.
- Sales across outlet location tiers, outlet sizes, and outlet types.
- Sales trends by outlet establishment year.
- Outlet-level performance measures such as total sales, number of
  items, average sales, average rating, and item visibility.
  
Tools and Technologies
- Microsoft Power BI Desktop -- report creation and interactive
  visualizations.
- Power Query -- data preparation and transformation workflow.
- DAX -- measures used for KPI calculations.
- Power BI Data Model -- tables, fields, and relationships used by
  the report.
  
Dataset and Data Model
The template contains two model tables:
1. BlinkIT Grocery Data
The report model contains the following fields:

  Field                       Description
  Item Fat Content            Fat-content category of the product
Item Identifier             Unique product/item identifier
Item Type                   Grocery product category
Outlet Establishment Year   Year the outlet was established
Outlet Identifier           Outlet identifier
Outlet Location Type        Outlet location tier
Outlet Size                 Outlet size category
Outlet Type                 Outlet category/type
Item Visibility             Visibility measure for the item
Item Weight                 Weight of the item
Sales                       Sales value
Rating                      Item/customer rating field in the source model

2. Metrics
A supporting Metrics table is included in the model. It contains:
- Metrics
- Metrics Fields
- Metrics Order
  
This table is used for the report's metric-selection functionality.
Key Performance Indicators (KPIs)
The dashboard includes four KPI measures:
  KPI                     DAX calculation                             What it represents
  Total Sales             SUM('BlinkIT Grocery Data'[Sales])        Sum of sales

  Avg Sales               AVERAGE('BlinkIT Grocery Data'[Sales])    Average sales value

  NO. of Items            COUNTROWS('BlinkIT Grocery Data')         Number of item records
Avg rating              AVERAGE('BlinkIT Grocery Data'[Rating])   Average rating
The actual KPI values depend on the dataset loaded into the Power BI
template and the filters selected in the report. They are not stated
here because the supplied .pbit file does not provide verified,
populated KPI results.

Dashboard Visualizations
The supplied report definition includes these visuals:
1. KPI Cards -- show Total Sales, Avg Sales, NO. of Items, and Avg
   rating.
2. Sales by Item Type -- Bar Chart -- compares total sales across
   grocery item categories.
3. Sales by Item Fat Content -- Donut Chart -- compares sales
   across fat-content categories.
4. Sales by Outlet Establishment Year -- Line Chart -- displays
   sales across outlet establishment years.
5. Sales by Outlet Location Type -- Funnel Chart -- compares sales
   across location tiers.
6. Sales by Outlet Size -- Donut Chart -- shows the sales
   distribution by outlet size.
7. Outlet Performance -- Matrix/Table -- compares outlet type using
   Total Sales, NO. of Items, Avg Sales, Avg rating, and Item
   Visibility.
8. Outlet Location and Fat Content -- Clustered Bar Chart --
   compares sales by outlet location type and item fat content.
Interactive Filters

The report includes slicers for:
- Item Type
- Outlet Size
- Outlet Location Type
A metric-selection control is also included through the Metrics table.
Selecting a filter changes the report visuals according to the selected
category.
DAX Measures Used
Total Sales =
SUM('BlinkIT Grocery Data'[Sales])

Avg Sales =
AVERAGE('BlinkIT Grocery Data'[Sales])

NO. of Items =
COUNTROWS('BlinkIT Grocery Data')

Avg rating =
AVERAGE('BlinkIT Grocery Data'[Rating])
How to Open and Use the Template
1. Install and open Microsoft Power BI Desktop.
2. Open Blinkit Dashboard Analysis.pbit.
3. When prompted, provide the required source dataset or data-source
   details.
4. Confirm that the source columns match the fields used in the model.
5. Load or refresh the data.
6. Review the KPI cards and charts.
7. Use the Item Type, Outlet Size, and Outlet Location Type slicers to
   explore different segments.
Suggested Repository Structure
Blinkit-Sales-Analysis-Dashboard/
│
├── README.md
├── Blinkit Dashboard Analysis.pbit
├── Dataset/
│   └── blinkit_grocery_data.xlsx
└── Dashboard_Screenshots/
    └── dashboard_overview.png
Only include the dataset and screenshots if you have those files and
have permission to share them.
Business Questions This Dashboard Can Help Explore
- Which grocery item types contribute the most to sales?
- How does sales contribution differ by item fat content?
- Which outlet location tier contributes more sales?
- How do sales compare across outlet sizes and outlet types?
- How have sales varied across outlet establishment years?
- How do average rating and item visibility differ across outlet
  types?
Conclusion
The Blinkit Sales Analysis Dashboard brings product and outlet sales
information into a single interactive Power BI report. Its KPI cards,
charts, matrix, and slicers allow users to examine sales from multiple
perspectives and explore patterns that may support retail reporting and
business decision-making.

Author
Swayam Sharma

Project: Blinkit Sales Analysis Dashboard

Screenshot/
Show what the dashboard looks like.
Example:https://github.com/swayamsharma1346-maker/Blinkit-Dashboard-Analysis/blob/main/Blinkit%20Dashboard.png

Technology: Microsoft Power BI
