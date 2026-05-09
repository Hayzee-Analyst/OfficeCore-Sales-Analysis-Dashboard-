# OfficeCore-Sales-Analysis-Dashboard-

<img width="1000" height="523" alt="Image" src="https://github.com/user-attachments/assets/525a473f-3fba-47c9-9cf8-387b0308acb1" />

## Project Overview
This project analyzes sales performance data for OfficeCore Distributors Inc. a mid-sized B2B office supplies distribution company operating across five regional territories in the United States.

The goal was to build an interactive 2 page Power BI dashboard** that provides leadership with clear visibility into company-wide sales performance for better strategic decision-making.

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

An interactive 2 page Power BI dashboard was developed to provide stakeholders with actionable business insights.

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

### The top performing product by a clear margin was the **USB-C Hub Pro**, generating **$26K** in sales 
nearly double most of its competitors and standing out as the undisputed revenue leader.

Following behind were the **Mechanical Keyboard** and two **Whiteboard** variants, each pulling in **$16K**,
showing strong and consistent demand across office and workspace essentials.

**Paper Clips**, **Bluetooth Speaker**, **Desk Organizer**, and **Memory Card** all came in close at **$15K**,
reflecting broad, steady interest across both tech accessories and everyday office supplies.

Rounding out the top 10 was the **USB-C Hub** (standard variant) at **$14K**, suggesting that
the Hub category as a whole holds significant customer appeal across multiple price points.

> **Key Insight:** Accessories and workspace tools dominate the top 10, with the USB-C Hub Pro
> driving the highest individual product revenue — signaling strong demand for connectivity solutions.

 ##  Total Sales by Rep
 <img width="322" height="174" alt="Image" src="https://github.com/user-attachments/assets/02033cb6-f754-41db-990c-cd974b6f4e7b" />

### Sales Rep Performance Breakdown

| # | Sales Rep | Total Sales |
|---|-----------|-------------|
| 1 | Riley Harris | **$29K** |
| 2 | Shawn Nguyen | $28K |
| 3 | Peyton Nguyen | $25K |
| 4 | Rowan Anderson | $25K |
| 5 | Dakota White | $25K |

Riley Harris leads the team with $29K in total sales, closely  followed by Shawn Nguyen at $28K. The remaining three reps Peyton Nguyen, Rowan Anderson, and Dakota White — are all tied at $25K, indicating a strong and consistent mid-tier performance across the team.

## Total Sales by Territory
<img width="275" height="175" alt="Image" src="https://github.com/user-attachments/assets/116e4ecd-dd6e-468b-b3f9-332851bcc5d8" />

### Territory Sales Breakdown

| # | Territory | City | Total Sales |
|---|-----------|------|-------------|
| 1 | North America | Austin | **$32K** |
| 2 | North America | Dallas | $28K |
| 3 | North America | Chicago | $26K |
| 4 | Europe | Boston | $24K |
| 5 | North America | Boise | $21K |

 Austin leads all territories with **$32K** in total sales, making North America the strongest performing region overall. **Dallas** and **Chicago** follow closely, while **Boise** trails as the lowest contributor at **$21K** signaling an opportunity for growth in that territory.

 ##  Sales Performance Matrix  Rep vs Product Category
 <img width="323" height="413" alt="Image" src="https://github.com/user-attachments/assets/87c610e7-00e4-4ab0-a3e0-97ee63dfd5d8" />

### Breakdown by Rep and Category

| Rep Name | Computer Accessories | Electronics | Furniture | Network |
|----------|---------------------|-------------|-----------|---------|
| Skyler Green | $3.28K | $2.44K | $2.02K | $1.97K |
| Shawn Nguyen | $1.67K | $8.13K | $3.14K | $3.16K |
| Rowan Anderson | $3.80K | $5.68K | $1.24K | $4.32K |
| Riley Harris | $3.05K | $5.70K | $2.30K | $4.46K |
| Reese Smith | $1.92K | $2.41K | $2.08K | $1.90K |
| Peyton Wright | $2.59K | $3.21K | $2.49K | $2.64K |
| Peyton Torres | $1.06K | $5.72K | $2.04K | $1.67K |
| Peyton Smith | $2.72K | $2.56K | $2.66K | $1.80K |
| Peyton Nguyen | $3.10K | $6.05K | $2.27K | $2.07K |
| Marley Torres | $3.34K | $3.98K | $1.32K | $1.62K |
| Logan Scott | $1.88K | $464.52 | $1.54K | $1.44K |
| Jules Wilson | $2.49K | $6.51K | $2.35K | $917.27 |
| Hayden Johnson | $1.32K | $4.41K | $1.43K | $2.98K |
| Finley Wright | $622.38 | $978.80 | $1.11K | $952.90 |
| Finley Harris | $1.14K | $4.86K | $3.18K | $3.19K |
| Finley Garcia | $958.53 | $5.98K | $1.32K | $3.04K |
| **Total** | **$52.02K** | **$103.68K** | **$52.53K** | **$54.55K** |

Key Insight:** **Electronics** dominates all categories with a total of **$103.68K**, nearly double every other category. **Shawn Nguyen** is the standout Electronics performer at **$8.13K**. **Computer Accessories** and **Furniture** are closely matched at**$52.02K** and **$52.53K** respectively, while **Network** sits at **$54.55K**  suggesting balanced demand across the remaining three categories.

##  Sales Performance Matrix — Rep, Region & Order Summary
<img width="301" height="189" alt="Image" src="https://github.com/user-attachments/assets/328a160d-60b2-4811-8b7d-9b6e5b59c077" />

### Breakdown by Rep, Region, Orders and Units Sold

| Rep Name | Region | Total Order | Unit Sold | Total Sales |
|----------|--------|-------------|-----------|-------------|
| Riley Harris | North | $12.4K | 320 | **$29K** |
| Shawn Nguyen | East | $11.8K | 298 | $28K |
| Peyton Nguyen | West | $10.2K | 275 | $25K |
| Rowan Anderson | Central | $9.8K | 260 | $25K |
| Dakota White | North | $9.5K | 245 | $25K |
| Avery Smith | East | $8.7K | 230 | $22K |
| Finley Harris | South | $8.2K | 215 | $20K |
| Casey Hall | East | $7.9K | 200 | $19K |
| Finley Anderson | South | $7.4K | 190 | $18K |

Riley Harris** from the **North** region leads across all metrics  highest total orders, units sold, and total sales at **$29K**. The **East** region  has the most rep representation, showing strong team coverage. **South** region  reps trail slightly, indicating a potential area for targeted growth.

##  Recommendations

Based on the analysis of OfficeCore Distributors Inc. sales performance data,
the following recommendations are proposed for leadership consideration:

1. Double Down on the East and North Regions With both regions accounting
for over 53% of total sales, leadership should increase resource allocation,
sales headcount, and marketing efforts in these territories to sustain and
grow their dominance.

2. Investigate the Summer Sales Spike Revenue peaked between June and July
exceeding $60K. Understanding what drove that surge whether promotions,
seasonal demand, or rep activity  could help replicate that performance in
weaker months like October.

3. Address the Fall Sales Decline Sales hit their lowest point in October
at approximately $21K. A targeted Q4 sales strategy such as end of year
promotions, bundle offers, or rep incentives should be introduced to close
the seasonal gap.

4. Leverage the USB-C Hub  Pro's Success  As the top selling product at
$26K, leadership should ensure consistent stock availability, explore upselling
opportunities, and study what makes it perform to apply those lessons to
lower-performing products.

5. Invest in the South and West Regions  Both regions lag significantly
behind East and North. A structured growth plan including territory expansion,
rep training, or localized pricing strategies could unlock untapped revenue
potential in these underperforming areas.













 


## Author
**Azeez Akinkunmi Folarin**  
Aspiring Data Analyst  

📧 Email: azeezfola@gmail.com  
📱 Phone: 07080421822  

Open to internships, freelance gigs, and job opportunities.
