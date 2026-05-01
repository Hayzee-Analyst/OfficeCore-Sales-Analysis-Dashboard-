# OfficeCore-Sales-Analysis-Dashboard-

<img width="1000" height="523" alt="Image" src="https://github.com/user-attachments/assets/525a473f-3fba-47c9-9cf8-387b0308acb1" />

## Project Overview
This project analyzes sales performance data for **OfficeCore Distributors Inc.**, a mid-sized B2B office supplies distribution company operating across five regional territories in the United States.

The goal was to build an interactive **2-page Power BI dashboard** that provides leadership with clear visibility into company-wide sales performance for better strategic decision-making.

---

## Business Problem
Leadership lacked centralized visibility into sales operations, making it difficult to:

- Track high-performing vs underperforming sales representatives
- Identify top-performing and low-performing products
- Monitor regional sales distribution across territories
- Analyze month-over-month sales trends efficiently

Decision-making was largely manual and dependent on spreadsheet analysis.

---

## Business Objectives
The dashboard was designed to help stakeholders:

- Monitor revenue performance
- Track sales targets by representatives
- Analyze product profitability
- Evaluate regional sales contribution
- Identify sales trends and business opportunities


# Data Dictionary – OfficeCore Sales Analysis Dashboard

This document describes the datasets, fields, and data types used in the OfficeCore Sales Performance Analytics Project.

---

## 1. Sales Representatives Table

| Column Name | Description | Data Type |
|---|---|---|
| Sales Rep ID | Unique identifier assigned to each sales representative | Text |
| Rep Name | Full name of sales representative | Text |
| Region | Geographic sales region assigned to rep (North, South, East, West, Central) | Text |
| Territory | Specific city/territory handled by the sales representative | Text |

---

## 2. Orders Table

| Column Name | Description | Data Type |
|---|---|---|
| Date | Date transaction/order was placed | Date |
| Order ID | Unique identifier for each customer order | Text |
| Product ID | Unique identifier for each product sold | Text |
| Quantity | Number of units purchased per transaction | Whole Number |
| Sales Rep ID | Sales representative responsible for sale | Text |

---

## 3. Products Table

| Column Name | Description | Data Type |
|---|---|---|
| Product ID | Unique identifier assigned to each product | Text |
| Product Name | Name of product sold | Text |
| Category | Product classification/group | Text |
| Unit Price | Selling price per product unit | Decimal Number |

---


## Data Preparation & Transformation

Data cleaning, transformation, and restructuring were performed using **Power Query Editor in Power BI** to ensure data quality and consistency before analysis.

### Data Cleaning Tasks Performed
- Handled inconsistent and incomplete records
- Treated missing/empty values using appropriate cleaning techniques
- Standardized column formats and naming conventions
- Corrected and assigned appropriate data types to all fields
- Removed unnecessary errors and formatting inconsistencies

### Data Modeling
A star-schema data model was built by connecting three core tables:

- Orders Table
- Products Table
- Sales Representatives Table

Relationships were established to enable efficient filtering, aggregation, and cross-table analysis.

<img width="1210" height="675" alt="Image" src="https://github.com/user-attachments/assets/d27776b6-516e-4e57-9a64-38d047171d74" />


### DAX & Calculations
Created a dedicated **Calendar Table** using DAX for seamless time intelligence analysis.

<img width="1072" height="737" alt="Image" src="https://github.com/user-attachments/assets/a7f26a7e-573b-455e-b5ed-8e2f9a33669a" />

Additional DAX measures were created for key business metrics, including:

- Total Sales
- Total Quantity Sold
- Total Orders
- Average Order Value(AOV)

---

## Data Visualization

An interactive **2-page Power BI dashboard** was developed to provide stakeholders with actionable business insights.

### Dashboard Features
- KPI Cards for Sales, Orders, Average Order value, and Quantity Sold
  
<img width="357" height="217" alt="Image" src="https://github.com/user-attachments/assets/22e55dc5-c54c-441a-a134-24c33329c3bd" />


# Insights
## Sales Trend Analysis
<img width="709" height="253" alt="Image" src="https://github.com/user-attachments/assets/7d8ad6c1-c883-4fdf-bf38-13d6253587bf" />


### Sales Trend Insight

Sales performance started strong in January, declined in February, and remained relatively stable throughout the spring months.

Revenue peaked between **June and July**, exceeding **$60K**, indicating the strongest sales period of the fiscal year.

A significant decline was observed after summer, with sales dropping steadily through fall and reaching the lowest point in **October** at approximately **$21K**.

A mild recovery was recorded toward the end of the year, suggesting a clear seasonal sales pattern characterized by **strong summer performance and weaker fall sales**.

## Total Sales by Reion
<img width="308" height="178" alt="Image" src="https://github.com/user-attachments/assets/04d43425-b8fd-47a1-8250-ff4cea4895dd" />

### Regional Sales Breakdown

The donut chart below illustrates the distribution of total sales across five regions:

| Region   | Sales Share |
|----------|-------------|
| East     | 27.95%      |
| North    | 25.96%      |
| Central  | 19.44%      |
| South    | 14.83%      |
| West     | 11.81%      |

 The East and North regions together account for over 53% of total sales,
 making them the primary revenue drivers of the business.

 ##  Total Sales by Product Name
 <img width="329" height="386" alt="Image" src="https://github.com/user-attachments/assets/4c252ef2-2fd1-4410-87f9-531f49e35b50" />

### Product Sales Breakdown

| # | Product | Total Sales |
|---|---------|-------------|
| 1 | USB-C Hub – Pro | **$26K** |
| 2 | Mechanical Keyboard | $16K |
| 3 | Whiteboard (variant 1) | $16K |
| 4 | Whiteboard (variant 2) | $16K |
| 5 | Paper Clips (10-pack) | $15K |
| 6 | Bluetooth Speaker | $15K |
| 7 | Desk Organizer | $15K |
| 8 | Memory Card | $15K |
| 9 | USB-C Hub | $14K |
| 10 | Laser Printer | $13K |
| 11 | Photo Paper Pack | $13K |
| 12 | SSD 1TB | $13K |
| 13 | Network Card | $12K |
| 14 | Portable Projector | $12K |
| 15 | Whiteboard (variant 3) | $11K |
| 16 | USB Wi-Fi Adapter (v1) | $11K |
| 17 | Ergonomic Chair | $11K |
| 18 | Network Card (v2) | $11K |
| 19 | USB Wi-Fi Adapter (v2) | $11K |
| 20 | USB-C Hub – P | $11K |
| 21 | Ink Cartridge | $10K |
| 22 | Laser Printer (variant) | $10K |

 The USB-C Hub – Pro is the clear top performer at $26K 
 significantly ahead of every other product. The next tier clusters tightly between
 $15K–$16K, showing consistent demand across office and tech accessories.












 


## Author
**Azeez Akinkunmi Folarin**  
Aspiring Data Analyst  

📧 Email: azeezfola@gmail.com  
📱 Phone: 07080421822  

Open to internships, freelance gigs, and job opportunities.
