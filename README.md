
# Project Overview

 
##Sales & Customer Performance Dashboard**

## Description  
NexSpace Retail, a growing US-based store dealing in technology, office supplies, and furniture, faced a familiar challenge shared by many retail businesses: **their data lived everywhere except in one place**.

Sales records were in a database.  
Customer information was scattered across several Excel files.  
Product data existed only in XML systems that no one wanted to touch.  

Because everything was disconnected, leadership struggled to answer basic but critical questions:

- *Is discount good for sales?*  
- *Which products do our customers purchase most?*  
- *Are sales increasing, or declining?*

To solve this, I designed and built a fully integrated Excel dashboard using **Power Query** and the **Excel Data Model (Power Pivot)**.  
This project brought together all data sources—database tables, folder files, and XML feeds—into one automated, unified system.  

The result was an interactive dashboard that tells a complete story of the business:  
how customers behave, which products category outperform others, and where sales opportunities lie.  
With real-time insights and clear KPIs, NexSpace Retail finally gained the clarity and confidence needed to make informed decisions.


---

# Business Challenge

The company’s performance data was scattered across multiple systems:

- Sales data stored in a database  
- Customer data spread across multiple files  
- Product data available only in XML format  

This fragmentation made it difficult to:

- Identify trends in customer purchases  
- Evaluate product effectiveness across regions  
- Track sales and profitability in real time  

---

# Project Objective

To connect, clean, and merge all data sources into a single Excel-based model using Power Query, and build interactive dashboards that provide:

- Customer segmentation and value analysis  
- Product performance insights  
- Sales and regional trend tracking  
- High-level business KPIs for strategic decision-making


# Data Integration & Preparation

## Data Sources

| Source   | Type                  | Connection Method       | Purpose                           |
|----------|----------------------|-----------------------|-----------------------------------|
| Sales    | Database (SQL / ODBC) | Power Query Connection | Revenue, Orders, Profit           |
| Customer | Folder (CSV/Excel)    | Folder Import          | Customer profiles and demographics |
| Product  | XML Files             | Power Query XML Import | Product details and pricing       |

## Integration Steps

1. Connected all data sources directly into Excel using **Power Query** (no manual export).  
2. Cleaned and standardized data: removed duplicates, fixed data types, merged columns.  
3. Created relationships using **Customer ID**, **Product ID**, and **Region** keys.  
4. Loaded the clean model into Excel’s **Data Model** for analysis.




# Methodology

## Data Modeling
- Built relationships between tables (**Sales ↔ Customer ↔ Product ↔ Date**).  
- Created calculated columns such as **Customer Value Category**, **ROI**, **Profit Margin**, **Discounted Amount**, **Discounted Status**, etc.  
- Developed measures for **YoY Growth**, **Revenue**, **Profit**, **Average Order Value**, and more.  

![Data Modelling](https://github.com/dorischioma/Sales-Performance-Analysis/blob/main/Data%20Modelling.png)  


## Dashboard Development
- Designed **5 interactive dashboards** using Excel charts, slicers, and KPIs.  
- Grouped visuals logically to tell a clear, actionable story.  
- Applied **conditional formatting** and **icon indicators** (▲▼ for growth) for intuitive insights.


# Dashboards & Insights

## Overview dashboard
![Overview Dashboard](https://github.com/dorischioma/Sales-Performance-Analysis/blob/main/Overview%20Dashboard.png)  

 
**Key Metrics:** Profit, Revenue, ROI, Orders, Discounts, Delivery Time    
The business is experiencing strong growth and high customer activity, but profit margins are being held back by rising costs and extensive discounting. Strategic improvements in discount control, regional expansion, and shipping efficiency can significantly boost overall performance.

### Key Insights

### 1. Strong Revenue Growth but Margin Pressure
The business generated **$2.3M in revenue** with a healthy YoY increase. However, **profit margin sits at 12.47%**, showing a slight decline due to rising operational costs and heavy use of discounts. This indicates the need for tighter cost control and more strategic discounting.

### 2. Heavy Discount Usage Reduces Profitability
There were **3,448 discounted orders** amounting to **$322.69K** in discount value. While discounts helped drive sales volume, they are contributing to lower profit margins. A review of discount strategy will improve profitability.

### 3. Customer Base Is Active and Growing
With **793 customers** generating **37,894 orders**, the business enjoys a strong repeat-purchase pattern. This shows healthy customer engagement and presents opportunities to build loyalty programs or targeted upsells.

### 4. Regional Performance Shows Clear Gaps
The **West region** leads with **$765K in revenue**, while Central and South regions lag behind. These underperforming areas represent untapped growth opportunities for targeted marketing and improved distribution strategies.

### 5. Noticeable Seasonality in Sales
Sales peak around **May–June**, with dips toward late Q3. Understanding this seasonal behavior can help management optimize inventory, promotions, and workforce planning.

### 6. Shipping Efficiency Is Moderate with Room for Improvement
Average delivery time stands at **3.96 days**, with most orders fulfilled within **2–5 days**. Improving deliveries in the **4–7 day category** can enhance customer satisfaction and competitiveness.

### 7. Standard Class Shipping Dominates
**60% of customers** select Standard Class shipping, indicating cost sensitivity. This opens opportunities for:  
- Introducing incentives for faster shipping  
- Reducing the cost of Standard Class through logistics optimization


## Customer Dashboard
![Customer Dashboard](https://github.com/dorischioma/Sales-Performance-Analysis/blob/main/Customer%20Dashboard.png)  

  
The business is supported primarily by **Consumer-segment, senior, and loyal customers**, who generate the highest revenue and profit with minimal discount dependency. Low-value and declining customers are discount-heavy and cost the business more than they contribute. Strategic focus on high-value segments and conversion of one-time buyers will drive stronger long-term customer profitability.


### Key Insights

### 1. Consumer Segment Dominates the Customer Base
The **Consumer segment (409 customers)** is the largest group compared to Corporate and Home Office.  
This implies the business is largely B2C-driven, and initiatives targeted at individual consumers will generate the fastest return.

### 2. Senior Customers Drive the Highest Purchase Volume
Senior customers have the highest number of orders (**3,265**) and the highest average purchase value (**$238**).  
They are the most valuable demographic, indicating strong loyalty and high purchasing power.

### 3. Young Adults and Middle-Age Groups Show Moderate Value
Young Adults and Middle-Age customers generate a reasonable number of orders but have lower average purchase values (**$225–$235**) than Seniors.  
These groups could be further nurtured with:  
- Targeted upselling  
- Bundles  
- Loyalty discounts  

### 4. Loyal Customers Are the Revenue Powerhouse
The **Loyal customer segment** delivers the highest revenue (**$943K**) with lower discount usage compared to other categories.  
This confirms that loyalty programs work, and these customers should remain a priority for retention strategies.

### 5. One-Time Buyers Present a Growth Opportunity
One-time buyers contribute **$835K in revenue** but consume **$120K in discounts**, suggesting many buy only during promotions.  
Turning even a small percentage of this group into loyal customers can significantly increase profit.

### 6. Declining Customers Have High Discount Dependency
The declining customer group has very low revenue (**$2K**) but extremely high discount usage (**$316**), indicating:  
- Low engagement  
- Heavy reliance on discount campaigns  

This group should be deprioritized, with resources reallocated to more profitable customer types.

### 7. High-Value Customers Generate Most Revenue and Highest Profit
From the Customer Value chart:  
- High-value customers: **$1.21M revenue** and **$394K profit**  
- Medium-value customers: less  
- Low-value customers: **$248K revenue** but negative profit due to discounts  

Implications:  
- Focus retention efforts on high-value customers  
- Motivate medium-value customers to increase purchase frequency  
- Reduce discount exposure to low-value customers

### 8. Senior and Young Adult Segments Yield the Highest Profit
In the profit-by-age chart:  
- Senior group: **$108K profit**  
- Young Adults: **$55K profit**  

These two demographics represent the highest profit potential and should be prioritized for targeted campaigns.


## Product Dashboard
![Product Dashboard](https://github.com/dorischioma/Sales-Performance-Analysis/blob/main/Product%20Dashboard.png)  


Technology dominates as the highest-performing category, supported by strong customer preference across all age groups. However, unprofitable discounting—especially in **Tables, Bookcases, and Supplies**—is dragging down product margins. Best-sellers like **Phones, Chairs, Binders, and Paper** continue to drive both demand and revenue, signaling where the company should concentrate inventory and promotional efforts.


### Key Insights

### 1. Technology Products Are the Most Preferred Across All Age Groups
All age groups — especially Seniors and Young Adults — show their highest spending in the **Technology** category.  
This indicates strong overall demand and suggests technology offers the highest revenue potential for future product expansion.

### 2. Phones and Chairs Are the Best-Selling Products
From the Top 5 Best-Selling Products chart:  
- Phones (**$331K**)  
- Chairs (**$328K**)  
- Storage, Tables, and Binders follow  

These products are the **volume drivers**, and inventory levels for these items must remain high to avoid stockouts.

### 3. Supplies and Art Are the Worst-Performing Categories
Worst-performing items include:  
- Supplies (**$47K**)  
- Art (**$27K**)  
- Envelopes, Labels, and Fasteners  

These low-performing products may require:  
- Targeted promotions  
- Bundling  
- Portfolio re-evaluation  

### 4. Discounts Are Causing Heavy Losses in Certain Product Categories
From the Least Profitable Discounted Subcategories:  
- Tables (**-$17.2K**)  
- Bookcases (**-$3.4K**)  
- Supplies (**-$1.8K**)  

These products are losing money even when sold, mainly due to **excessive discounting**. A pricing review is required to stop margin leakage.

### 5. Copiers and Paper Deliver the Highest Profit Under Discount
Even with discounts, some categories still generate strong profit:  
- Copiers (**$56K**) — highest profit after discount  
- Paper (**$34K**)  
- Envelopes and Labels also perform well  

This suggests discounting works well only in selected product lines and can be used strategically to boost sales without hurting margins.

### 6. Binder and Paper Are the Most In-Demand Products
From the Top 5 In-Demand Products chart:  
- Binders (**1,525 orders**)  
- Paper (**1,370 orders**)  
- Furnishings, Phones, and Storage follow  

These products have **high order counts** and should be prioritized in:  
- Stock planning  
- Warehouse allocation  
- Supply chain forecasts  

### 7. Senior Customers Drive the Highest Product Spend
Senior customers consistently have the highest spending across:  
- Furniture  
- Office Supplies  
- Technology  

This means the older demographic directly influences product performance, and **personalized offers** for this group can boost revenue further.




