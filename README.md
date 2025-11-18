 
# Sales & Customer Performance Dashboard

## Project Overview  
NexSpace Retail, a growing US-based store dealing in technology, office supplies, and furniture, faced a familiar challenge shared by many retail businesses: **their data lived everywhere except in one place**.

Sales records were in a database.  
Customer information was scattered across several Excel files.  
Product data existed only in XML systems that no one wanted to touch.  

Because everything was disconnected, leadership struggled to answer basic but critical questions:

- *Is discount good for sales?*  
- *Which products do our customers purchase most?*  
- *Are sales increasing, or declining?*

To solve this, I designed and built a fully integrated Excel dashboard using **Power Query** and the **Excel Data Model (Power Pivot)**.  
This project brought together all data sources database tables, folder files, and XML feeds into one automated, unified system.  

The result was an interactive dashboard that tells a complete story of the business, how customers behave, which products category outperform others, and where sales opportunities lie.  
With real-time insights and clear KPIs, NexSpace Retail finally gained the clarity and confidence needed to make informed decisions.


## Business Challenge

The company’s performance data was scattered across multiple systems:

- Sales data stored in a database  
- Customer data spread across multiple files  
- Product data available only in XML format  

This fragmentation made it difficult to:

- Identify trends in customer purchases  
- Evaluate product effectiveness across regions  
- Track sales and profitability in real time  

---

## Project Objective

To connect, clean, and merge all data sources into a single Excel-based model using Power Query, and build interactive dashboards that provide:

- Customer segmentation and value analysis  
- Product performance insights  
- Sales and regional trend tracking  
- High-level business KPIs for strategic decision-making


## Data Integration & Preparation

### Data Sources

| Source   | Type                  | Connection Method       | Purpose                           |
|----------|----------------------|-----------------------|-----------------------------------|
| Sales    | Database (SQL / ODBC) | Power Query Connection | Revenue, Orders, Profit           |
| Customer | Folder (CSV/Excel)    | Folder Import          | Customer profiles and demographics |
| Product  | XML Files             | Power Query XML Import | Product details and pricing       |

### Integration Steps

1. Connected all data sources directly into Excel using **Power Query** (no manual export).  
2. Cleaned and standardized data: removed duplicates, fixed data types, merged columns.  
3. Created relationships using **Customer ID**, and **Product ID** keys.  
4. Loaded the clean model into Excel’s **Data Model** for analysis.


## Methodology

## Data Modeling
- Built relationships between tables (**Sales ↔ Customer ↔ Product ↔ Date**).  
- Created calculated columns such as **Customer Value Category**, **ROI**, **Profit Margin**, **Discounted Amount**, **Discounted Status**, etc.  
- Developed measures for **YoY Growth**, **Revenue**, **Profit**, **Average Order Value**, and more.  

![Data Modelling](https://github.com/dorischioma/Sales-Performance-Analysis/blob/main/Data%20Modelling.png)  


### Dashboard Development
- Designed **5 interactive dashboards** using Excel charts, slicers, and KPIs.  
- Grouped visuals logically to tell a clear, actionable story.  
- Applied **icon indicators** (▲▼ for growth) for intuitive insights.


## Dashboards & Insights

### Overview dashboard
![Overview Dashboard](https://github.com/dorischioma/Sales-Performance-Analysis/blob/main/Overview%20Dashboard.png)  

 
### Insights  
#### 1. Strong Revenue Growth but Margin Pressure
The business generated **$2.3M in revenue** with a healthy YoY increase. However, **profit margin sits at 12.47%**, showing a slight decline due to rising operational costs and heavy use of discounts. This indicates the need for tighter cost control and more strategic discounting.

#### 2. Heavy Discount Usage Reduces Profitability
There were **3,448 discounted orders** amounting to **$322.69K** in discount value. While discounts helped drive sales volume, they are contributing to lower profit margins. A review of discount strategy will improve profitability.

#### 3. Customer Base Is Active and Growing
With **793 customers** generating **37,894 orders**, the business enjoys a strong repeat-purchase pattern. This shows healthy customer engagement and presents opportunities to build loyalty programs or targeted upsells.

#### 4. Regional Performance Shows Clear Gaps
The **West region** leads with **$765K in revenue**, while Central and South regions lag behind. These underperforming areas represent untapped growth opportunities for targeted marketing and improved distribution strategies.

#### 5. Noticeable Seasonality in Sales
Sales peak around **May–June**, with dips toward late Q3. Understanding this seasonal behavior can help management optimize inventory, promotions, and workforce planning.

#### 6. Shipping Efficiency Is Moderate with Room for Improvement
Average delivery time stands at **3.96 days**, with most orders fulfilled within **2–5 days**. 

#### 7. Standard Class Shipping Dominates
**60% of customers** select Standard Class shipping, indicating cost sensitivity. This opens opportunities for:  
- Introducing incentives for faster shipping  
- Reducing the cost of Standard Class through logistics optimization


### Customer Dashboard
![Customer Dashboard](https://github.com/dorischioma/Sales-Performance-Analysis/blob/main/Customer%20Dashboard.png)  

### Insights

#### 1. Consumer Segment Dominates the Customer Base
The **Consumer segment (409 customers)** is the largest group compared to Corporate and Home Office.  
This implies the business is largely B2C-driven, and initiatives targeted at individual consumers will generate the fastest return.

#### 2. Senior Customers Drive the Highest Purchase Volume
Senior customers have the highest number of orders (**3,265**) and the highest average purchase value (**$238**).  
They are the most valuable demographic, indicating strong loyalty and high purchasing power.

#### 3. Young Adults and Middle-Age Groups Show Moderate Value
Young Adults and Middle-Age customers generate a reasonable number of orders but have lower average purchase values (**$225–$235**) than Seniors.  
These groups could be further nurtured with:  
- Targeted upselling  
- Bundles  
- Loyalty discounts  

#### 4. Loyal Customers Are the Revenue Powerhouse
The **Loyal customer segment** delivers the highest revenue (**$1.8M**) with a higher profit compared to other customer types, these customers dominate the customer base and are by far the largest, meanwhile, Active, One-time Buyers, and New customers are extremely few, this shows low customer acquisition and limited new customer activation. The business is heavily dependent on existing loyal customers. Growth is likely coming more from retention than acquisition, which can be risky long-term.  
  
#### 5. Senior and Young Adult Segments Yield the Highest Profit
In the profit-by-age chart:  
- Senior group: **$108K profit**  
- Young Adults: **$55K profit**  

These two demographics represent the highest profit potential and should be prioritized for targeted campaigns.


### Product Dashboard
![Product Dashboard](https://github.com/dorischioma/Sales-Performance-Analysis/blob/main/Product%20Dashboard.png)  

### Insights

#### 1. Technology Products Are the Most Preferred Across All Age Groups
All age groups especially Seniors and Young Adults show their highest spending in the **Technology** category.  
This indicates strong overall demand and suggests technology offers the highest revenue potential for future product expansion.

#### 2. Phones and Chairs Are the Best-Selling Products
From the Top 5 Best-Selling Products chart:  
- Phones (**$331K**)  
- Chairs (**$328K**)  
- Storage, Tables, and Binders follow  

These products are the **volume drivers**, and inventory levels for these items must remain high to avoid stockouts.

#### 3. Supplies and Art Are the Worst-Performing Categories
Worst-performing items include:  
- Supplies (**$47K**)  
- Art (**$27K**)  
- Envelopes, Labels, and Fasteners  

These low-performing products may require:  
- Targeted promotions  
- Bundling  
- Portfolio re-evaluation  

#### 4. Discounts Are Causing Heavy Losses in Certain Product Categories
From the Least Profitable Discounted Subcategories:  
- Tables (**-$17.2K**)  
- Bookcases (**-$3.4K**)  
- Supplies (**-$1.8K**)  

These products are losing money even when sold, mainly due to **excessive discounting**. A pricing review is required to stop margin leakage.

#### 5. Copiers and Paper Deliver the Highest Profit Under Discount
Even with discounts, some categories still generate strong profit:  
- Copiers (**$56K**) — highest profit after discount  
- Paper (**$34K**)  
- Envelopes and Labels also perform well  

This suggests discounting works well only in selected product lines and can be used strategically to boost sales without hurting margins.

#### 6. Binder and Paper Are the Most In-Demand Products
From the Top 5 In-Demand Products chart:  
- Binders (**1,525 orders**)  
- Paper (**1,370 orders**)  
- Furnishings, Phones, and Storage follow  

These products have **high order counts** and should be prioritized in:  
- Stock planning  
- Warehouse allocation  
- Supply chain forecasts  

#### 7. Senior Customers Drive the Highest Product Spend
Senior customers consistently have the highest spending across:  
- Furniture  
- Office Supplies  
- Technology  

This means the older demographic directly influences product performance, and **personalized offers** for this group can boost revenue further.  

### Sales Dashboard  
![Sales Dashboard](https://github.com/dorischioma/Sales-Performance-Analysis/blob/main/Sales%20Dashboard.png)  

### Insights
#### 1. Daily sales trend  
- Sales peak on **Monday–Tuesday**, averaging around **$380K–$420K**.  
- The lowest sales occur on **Wednesday–Thursday**, dropping to about **$200K–$230K**.  
- Sales recover again from **Friday–Saturday**, stabilizing around **$350K+**.  

#### 2. Quarterly sales trend
- **Q2** recorded the highest sales at **$841K**, significantly outperforming all other quarters.  
- **Q1** follows with **$636K**, while **Q3** declines sharply to **$386K**.  
- **Q4** slightly recovers to **$436K**, but remains below the first half of the year.  


#### 3. Discount vs Revenue
- Revenue peaks in **May** at approximately **$350K–$380K**, aligning with a slight increase in discount amounts.  
- A major revenue drop occurs in **July and August**, falling below **$200K** even though discount levels remain relatively steady.  
- Revenue remains moderate from **September to December** (**$220K–$260K** range).  

#### 4. Discount vs Profit
###### Jan–May:
- Discounts rise from **~$20K → ~$55K**  
- Profit rises from **~$15K → ~$45K**

##### Jun–Aug:
- Discounts fall to **~$10K**  
- Profit also drops to **~$10K**

##### Sep–Oct:
- Discount increases reignite profit recovery (**~$30K**)

##### Nov–Dec:
- Both metrics stabilize around **~$20K**

### Geo map Dashboard
![Geo map Dashboard](https://github.com/dorischioma/Sales-Performance-Analysis/blob/main/Geo%20Map%20page.png)  

### Insights  
#### Best Overall States (Strong Revenue, Margin & Customer Base)
- California: High revenue ($451K) + high margin (13%) + most customers.  
- New York: High revenue ($280K) + high margin (21%).  
- Texas: Strong revenue ($193K) + stable margin (11%).  
- Pennsylvania: High revenue ($143K) + solid 10% margin.  

#### High-Revenue but Low-Profit States  
- North Carolina: $117K revenue but –4% margin (loss).  
- Florida: $50K revenue but only 2% margin.
- Colorado: $58K revenue with 2% margin.  

#### High Margin but Low Revenue States (Growth Opportunity)  
These states show strong profit margins but low revenue due to small customer bases:  
- Maryland (27% margin, $2K revenue)  
- Nevada (23% margin, $1K revenue)  
- D.C. (22% margin, $2K revenue)  
- New Mexico (22% margin, $6K revenue)  
- South Dakota (30% margin, $3K revenue)  


## Conclusion  
- The business is experiencing strong growth and high customer activity, but profit margins are being held back by rising costs and extensive discounting. Strategic improvements in discount control, regional expansion, and shipping efficiency can significantly boost overall performance.
- The business is supported primarily by **Consumer-segment, senior, and loyal customers**, who generate the highest revenue and profit. Loyal customers are being rewarded with discounts, which is good for retention, but the discount amount is very high compared to other groups. Strategic focus and conversion of occassional, active and one-time buyers segments will drive stronger long-term customer profitability and customer acquisition. 
- Technology dominates as the highest-performing category, supported by strong customer preference across all age groups. However, unprofitable discounting, especially in **Tables, Bookcases, and Supplies** is dragging down product margins. Best-sellers like **Phones, Chairs, Binders, and Paper** continue to drive both demand and revenue, signaling where the company should concentrate inventory and promotional efforts.
- Mid-week drop indicates lower buying activity; the business performs strongest at the start and end of the week.
- Sales momentum is strongest in the first half of the year, with a major peak in Q2. The low Q3 performance may indicate seasonal slowdown or reduced consumer activity.
- Discounts do not strongly drive revenue. Even with stable discounting, revenue dips in mid-year, suggesting external factors like seasonality or reduced demand.
- Profit and discount amount show a **strong positive correlation** throughout the year.  

## Recommendations
- Reduce Discounts in Loss-Making States
- Protect & Invest in High-Value States
- Expand in High-Margin Small States
- Address Low Margin States
  - Oregon, Arkansas, Florida, Colorado.
  - Investigate:
    - Shipping cost?
    - Discount abuse?
    - Channel profitability?
- Build State-Specific Strategies:
    - High revenue + high margin → Growth & retention focus
    - Low revenue + high margin → Market expansion
    - High revenue + low margin → Cost correction
    - Low revenue + low margin → Consider deprioritizing
- Focus on Loyal and Young Adult/Senior customers, who generate the highest revenue and purchase value.
- Strengthen Customer Acquisition by Increaseing marketing to grow the “New” and “Active” segments.
- Reevaluate Discounts for Loyal Customers by Checking if you can reduce discount levels without harming loyalty.
- Convert More Occasional to Loyal, They are already generating revenue, With targeted promotions, they can become the next biggest profitable group.
- Expand Technology product offerings, especially Phones and Computer Accessories.
- Reassess or reposition low-performing product categories (Supplies, Art).
- Reduce deep discounts on unprofitable items like Tables and Bookcases, or consider phase-out.
- Increase inventory for high-demand products (Binders, Paper, Phones) to maintain fulfillment efficiency
- Shift from broad discounting to targeted, data-driven promotions.  
- Apply discounts mainly to Elastic products (Copiers, Paper) that remain profitable even with price cuts.
- Prepare inventory in advance for mid-year peak months.  
- Spread out promotional spending to avoid heavy profit drops in Q2 and Q4.  
- Introduce cross-sell bundles during peak periods to increase revenue without heavy discounts.  
- Strengthen logistics and reduce delivery delays by working with better carriers or optimizing routes.


  

