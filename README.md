# 🍫 Chocolate Sales Dashboard – Power BI

## 📊 Project Overview

The **Chocolate Sales Dashboard** is an interactive Power BI dashboard developed to analyze chocolate shipment and sales performance.

The dashboard provides a clear view of **revenue, shipment volume, products, categories, regions, salespersons, order status, and yearly/monthly sales trends**.

The main objective of this project is to transform raw chocolate shipment data into meaningful business insights using **Power BI, Power Query, DAX, and data visualization techniques**.

---

## 🎯 Project Objectives

- Analyze overall chocolate sales and revenue performance.
- Track shipment count and number of boxes sold.
- Identify the best-performing salespersons.
- Find the top-selling products.
- Analyze sales performance by category.
- Compare sales across different regions and countries.
- Understand order status distribution.
- Analyze monthly and yearly sales trends.
- Build an interactive dashboard for business decision-making.

---

## 🛠️ Tools & Technologies

- **Power BI**
- **Power Query**
- **DAX**
- **Microsoft Excel**
- **Data Visualization**
- **Data Cleaning & Transformation**

---

## 📁 Dataset

The dataset contains chocolate shipment and sales information.

### Main Shipment Columns

| Column | Description |
|---|---|
| ShipmentID | Unique identifier for each shipment |
| SPID | Salesperson ID |
| PID | Product ID |
| GID | Geography/Region ID |
| Shipdate | Shipment date |
| Amount | Sales amount/revenue |
| Boxes | Number of boxes shipped |
| Order_Status | Current shipment/order status |

### Dimension Data

The dimension data contains additional information about:

- Products
- Product categories
- Cost per box
- Geography
- Regions
- Salespersons
- Sales teams

### Calendar Data

A separate calendar table was used for time-based analysis, including:

- Date
- Month
- Month Name
- Year
- Weekday
- Weekday Name

---

## 📌 Dashboard KPIs

The dashboard includes important Key Performance Indicators (KPIs):

### 💰 Total Revenue

Shows the overall revenue generated from chocolate sales.

### 📦 Shipment Count

Shows the total number of shipments.

### 📦 Total Boxes

Shows the total number of chocolate boxes shipped.

### 👥 Salesperson Performance

Identifies the salespersons contributing the highest sales revenue.

---

## 📈 Dashboard Visualizations

The dashboard contains the following visualizations:

### 1. Total Revenue KPI

Displays the total revenue and compares it with the target.

### 2. Shipment Count

Shows the overall number of shipments.

### 3. Total Boxes

Displays the total number of boxes shipped.

### 4. Best Salesperson

Highlights salespersons with the highest revenue contribution.

### 5. Revenue by Month

A line chart is used to analyze monthly revenue trends.

### 6. Top Performing Category

A donut chart shows the contribution of different chocolate categories.

### 7. Top Selling Products

A bar chart identifies the products generating the highest sales.

### 8. Geography Analysis

Shows sales distribution across different countries/geographies.

### 9. Region Wise Sales

Compares sales performance across regions such as:

- APAC
- Americas
- Europe

### 10. Order Status Analysis

A donut chart shows the distribution of orders based on status:

- Delivered
- Shipped
- Placed

### 11. Yearly Trend

A yearly trend chart is used to compare revenue performance across different years.

### 12. Interactive Filters

The dashboard includes slicers for:

- Year
- Month
- Region
- Category
- Salesperson

These filters allow users to interactively explore the data.

---

## 🔄 Data Preparation

The following steps were performed before creating the dashboard:

1. Imported the Excel dataset into Power BI.
2. Loaded shipment and dimension tables.
3. Checked the data types of columns.
4. Converted the shipment date into a proper Date data type.
5. Created/used a Calendar table for time-based analysis.
6. Created relationships between fact and dimension tables.
7. Used Power Query for data transformation.
8. Created DAX measures for KPIs and analysis.
9. Built interactive visualizations.

---

## 🧮 DAX Measures

Some important measures used in the dashboard include:

### Total Revenue

```DAX
Total Revenue = SUM(Shipments[Amount])
