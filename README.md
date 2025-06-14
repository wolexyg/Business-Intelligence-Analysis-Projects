## Power BI/Tableau Projects     

# Project 1- Title- Ecommerce Sales Dashboard  
## Problem Statement    
An Ecommerce company based in the US with btranches in Brazil,Canada and Mexico wants to create a Dashboard  and generate
insights for the following;     

-- 1.Create a KPI showing the Total Sales,Total Profit, Profit Margin and Total Orders        
-- 2.For the Visuals,create the following;     

  Top 5 Best Selling Products          
  Top 5 Worst Selling Products        
  Total Sales By Region       
  Total Sales By Month         
  Total Sales and Profit By Month           

<img src="https://i.ibb.co/PGT1fNFH/Ecommerce2.jpg" alt="Ecommerce2" border="0">      

## Key Findings     
-- Total Sales is $313k     
-- Total Profit is $29k     
-- Profit Margin 9.27%    
-- Total Orders is 1330       
-- Average Order Value (AOV): ~$235     
-- Average Profit per Order: ~$21.80      

## Total Sales By Month     
<img src="https://i.ibb.co/N5t1pdr/Total-Sales-By-Month.jpg" alt="Total-Sales-By-Month" border="0">     

-- December is the highest selling Month with a Total Sale of $50.3Million      

## Total Sales By Region   

<img src="https://i.ibb.co/Ld7xZCst/Total-Sales-By-Region.jpg" alt="Total-Sales-By-Region" border="0">    

-- The Central Region came top as the highest selling region with a total sale of $92.66k    

## Sales Rating    

<img src="https://i.ibb.co/r8jRK9H/Sales-Rating.jpg" alt="Sales-Rating" border="0">     

-- Based on Sales Rating,we have over 66.36% of Sales that are good...

## Best Selling Products       

<img src="https://i.ibb.co/WvbZVkGQ/Best-Selling-Products.jpg" alt="Best-Selling-Products" border="0">      

-- Eldon Express and Avery Dura came top as the best selling products with a Tolal Sales of $10.8k    

## Insights    
✅ Healthy Profitability       
A 9.27% profit margin indicates the business is generating reasonable returns. This margin is respectable for many industries, especially if you're selling physical goods or operating in competitive markets.        

📦 Moderate Sales per Order            
With an Average Order Value of ~$235 and ~$21.80 profit per order, your pricing and cost structure appear fairly optimized.        

However, profit per order is relatively low, which may limit scalability unless order volume increases significantly or margins improve.     

⚠️ Scalability Challenge      
Given the relatively low total sales and profit base, growth will require:      

Either higher order volume.          

Increased transaction value, or         

Improved margins to drive substantial bottom-line gains.       

## Recommendations     
🎯 Strategic Recommendations        
1. Increase Average Order Value (AOV)          
Introduce product bundles, upsells, or tiered pricing to encourage higher spend per transaction.      

Use data-driven personalization to suggest high-value items based on buyer behavior.         

2. Optimize for Margin Expansion        
Identify low-margin SKUs and reduce focus or renegotiate supply chain terms.       

Shift marketing emphasis toward higher-margin products or services.       

3. Boost Repeat Purchases      
With 1,330 orders, consider deploying loyalty programs, email retargeting, or subscription models to drive repeat sales and customer lifetime value (CLV).         

4. Explore Order Efficiency       
If operational costs per order are high, consider automating order processing, fulfillment, or customer service to reduce cost per transaction and improve profit per order.         

5. Benchmark Performance        
Compare your profit margin and AOV against industry peers to identify competitive advantages or areas for improvement.     

Use benchmarks to set realistic growth and efficiency targets.              





# Project 2 Title-Accident on Road Analysis  
 ## Project Overview        
The purpose of this Power BI dashboard is to analyze road accident data and identify patterns and trends that can help 
improve road safety. First step is to Import the data into Power BI and clean it to ensure it was accurate and ready for analysis. The data includes information about accidents, such as the number of vehicles involved, severity of the accident, and the location and time of the accident.   

<img src="https://i.ibb.co/JB87dM8/Road-Accident-Analysis.jpg" alt="Road-Accident-Analysis" border="0">          

## Higlights of the Analysis      
Clients wants to create a Road Accident Dashboard for year 2021 and 2022 so that they can have insight on the below requirements-

- Primary KPI - Total Casualties and Total Accident values for Current Year(CY) and YoY growth

- Primary KPI's — Total Casualties by Accident Severity for Current Year and YoY growth

- Secondary KPI's - Total Casualties with respect to vehicle type for Current Year

- Monthly trend showing comparison of casualties for Current Year and Previous Year (PY)

- Casualties by Road Type for Current year

- Current Year Casualties by Area/ Location & by Day/ Night

- Total Casualties and Total Accidents by Location    

## Data Analysis Expressions (DAX) Formulas Used in Measures     

1.Total Casualties For Current Year and Year on Year Growth

(a) Current Year To Date Casualties -- CY Casualties Measure

CY Casualties = TOTALYTD(SUM(Data[Number_of_Casualties]), 'Calendar'[Date])

(b) Previous Year Casualties -- PY Casualties Measure

PY Casualties = CALCULATE(SUM(Data[Number_of_Casualties]), SAMEPERIODLASTYEAR('Calendar'[Date]))

(c) Year on Year Growth of Casualties - YoY Casualties Measure

YoY Casualties = ([CY Casualties] - [PY Casualties])/[PY Casualties]

2. Total Accidents for Current Year and Year on Year Growth
   
(a) Current Year Accidents Count -- CY Accidents Count Measure

CY Accidents Count = TOTALYTD(COUNT(Data[Accident_Index]), 'Calendar'[Date])

(b) Previous Year Accidents Count -- PY Accidents Count Measure

PY Accidents Count = CALCULATE(COUNT(Data[Accident_Index]), SAMEPERIODLASTYEAR('Calendar'[Date]))

(c) Year on Year Growth of Accidents - YoY Accidents Measure

YoY Accidents = ([CY Accidents Count]-[PY Accidents Count])/[PY Accidents Count]   

## Key findings      
-  Total Current(CY) Casualties-196k   
-  Total Year Over Year(YOY) Accidents-144k    
-  Current Year(CY)Fatal Casualties-2.9k     
-  Current Year(CY)Serious Casualties-27k      
-  Current Year(CY)Slight Casualties-165.8k

# Insights           
## Accident Severity by Casualties Analysis        
<img src="https://i.ibb.co/nkPnMJq/Road-Accident-KPI-Banner.jpg" alt="Road-Accident-KPI-Banner" border="0">          
Accident Severity by Casualties Analysis entails a comprehensive evaluation of all factors contributing to the severity of accidents, particularly focusing on the number and extent of casualties involved. This analysis encompasses direct elements such as the nature of the accident and injuries sustained, as well as indirect factors like road conditions and environmental influences.          

## Casualties in the Urban/Rural Areas            
  <img src="https://i.ibb.co/qJbtD4C/Casualties-By-Urban-Rural-Areas.jpg" alt="Casualties-By-Urban-Rural-Areas" border="0">       
There is a higher risk of casualties in urban areas compared to rural areas. This is likely due to a combination of factors, including population density, traffic volume, and speed.    
  
 ## Casualties By Vehicle           
  <img src="https://i.ibb.co/mSQHyzM/Casualties-By-Vehicle-Type.jpg" alt="Casualties-By-Vehicle-Type" border="0">          
  Car recorded the highest number of casualties with a total of 155804.Insights on road fatalities by vehicle type reveal cars as the most lethal, likely due to their size, speed, and limited protection for cyclists. Bikes follow closely behind in fatalities. Trucks, driven by experienced professionals, are least involved in fatal crashes. Casualties vary based on factors like speed limits, road type, and safety features, such as airbags and seatbelts.                   

## Current-Year-vs-Previous-Year-Casualties-Monthly-Trend       
<img src="https://i.ibb.co/HYzdGjK/Current-Year-vs-Previous-Year-Casulaties-Monthly-Trend.jpg" alt="Current-Year-vs-Previous-Year-Casulaties-Monthly-Trend" border="0">               

November recorded the highest number of casualties with a record of 20975 in 2021 as compared with 18489 in 2022. The largest discrepancy between CY and PY casualties occurs in April and May, possibly attributed to seasonal factors like increased summer road traffic. However, due to the limited two-year dataset and significant month-to-month variation, drawing conclusive trends about overall casualty trends proves challenging.            
## Casualties By Light Conditions    
<img src="https://i.ibb.co/1f2gMJG/Casulaties-By-Light-Conditions.jpg" alt="Casulaties-By-Light-Conditions" border="0">         
People are more likely to be injured or killed in accidents that occur during daylight hours. This is likely due to a combination of factors, such as increased traffic volume, risky behaviors, and poorer visibility at night.        

## Casualties By Road Type    
<img src="https://i.ibb.co/1qJXg6g/Casualties-By-Road-Type.jpg" alt="Casualties-By-Road-Type" border="0">     
This findings underscore the importance of targeted interventions and resource allocation to enhance safety measures, reduce casualties, and improve overall road safety     

## Casualties By Location    
<img src="https://i.ibb.co/mTZkp0s/Casualties-By-Location.jpg" alt="Casualties-By-Location" border="0">     
The yellow dots represent the locations of accidents.           

## Recommendations   
-  By conducting a thorough assessment, stakeholders can better understand the dynamics of accidents, identify areas for improvement in safety measures, and implement targeted interventions to mitigate severity and enhance overall safety outcomes.   

# Project 3-SuperStore Sales Analysis  
## Project Objectives    
To contribute to the success of the business by Utilizing data analysis techniques,specifically focusing on time series analysis
to provide valuable insights and accurate sales forecasting.        
The objectives can be broken down into  the following detailed components;    
-  Dashboard Creation-Identify KPIs ,design an intuitive and visually appealing dashboard,add interactive  visualizations and filtering
  capabilities to allow users  to explore  the data at various levels of granualarity
-  Data Analysis-Provide valuable insights to business entities regarding the effectiveness of their sales strategies through visualizations and charts
-  Sales Forecasting-Leverage historic data  and apply time series analysis to generate sales forecast for the next 15 days
-  Actionable Insights and Recommendation-End goal is to derive insights  and actionable information that can drive strategic decision-making, support the supermarket's goals for growth,efficiency and customer satisfaction.      

  ## Tools Used    
  -  Microsoft Excel(Dataset)
  -  Power Query(For Data Cleaning)
  -  Microsoft PowerBI(Data Modelling,DAX Calculations,Dashboard Creation)  

 ## Dashboard Creation              
 <img src="https://i.ibb.co/s3SV3yH/Superstore-Sales-Dashboard4.jpg" alt="Superstore-Sales-Dashboard4" border="0">   


 
 
 ## Data Analysis     
 Questions to consider    
 -  Which region has the highest number of  Sales?      
   <img src="https://i.ibb.co/LQYpvy7/Sales-By-Region-Superstore.jpg" alt="Sales-By-Region-Superstore" border="0">
    The Western region is the highest selling region i.e sales 522k(33%)    
    


 -  Which Category has the highest number of sales?       
   <img src="https://i.ibb.co/BBNGtY9/Sales-By-Category-Superstore.jpg" alt="Sales-By-Category-Superstore" border="0">

   Office Supplies has the highest number sales.           

 -  Which is the top selling product Category and Subcategory?.               
   <img src="https://i.ibb.co/BBNGtY9/Sales-By-Category-Superstore.jpg" alt="Sales-By-Category-Superstore" border="0">         
    Office Supplies are the top selling Product Category                                         

   <img src="https://i.ibb.co/XDBrDr3/Sales-By-Sub-Category-Superstores.jpg" alt="Sales-By-Sub-Category-Superstores" border="0">        
    Phones are the top selling Subcategory

 -  Which is the preferred ship mode?.                  

    <img src="https://i.ibb.co/k1vyRR6/Sales-By-Ship-mode-Superstore.jpg" alt="Sales-By-Ship-mode-Superstore" border="0">      
    
    Standard Class is the prefered ship mode.

-  Which Segment recorded the highest sales?         
    <img src="https://i.ibb.co/TrXyz8d/Sales-By-Segment-Superstore.jpg" alt="Sales-By-Segment-Superstore" border="0">
   
   Consumers recorded the highest sales of 753k

  ## Sales Forecasting              
  <img src="https://i.ibb.co/vxCmPF9/Sales-Forecast-Superstore.jpg" alt="Sales-Forecast-Superstore" border="0">              



  ## Actionable Insights     
  -  Consumers contributed to more than half of the Superstores revenue
  -  The most preferred Shipping mode is the Standard Class
  -  Most valuable product is the Office Supplies
  -  Phones are the top selling product Subcategory
  -  California has the highest number of sales
  -  The Western Region emerged as the highest selling region

  ## Recommendations          
  -  Consumer and Corporate segment make up more than 70% of the Customer base segments
  -  Fresh marketing and promotional campaigns to target specific regions with higher sales potential by introducing special promotions and discounts.     
  -  Allocate resources to optimize top performing product categories and subcategories to maximize sales
  -  For least selling products,consider to either drop them from the catalogue or change suppliers and bargain for cheaper price.
  -  We can consider offering multiple shipping options to cater for different customer preferences.


# Project 4-Sales Data Analysis      
## Project Objective 
The Objective of this Analysis is to gain valuable insight that will propel actionable insights and inform the company's strategic decisions. The impact of this analysis on the business and the final outcome.         

<img src="https://i.ibb.co/rdf6LTz/Sales-Analysis-data.jpg" alt="Sales-Analysis-data" border="0">   

The Project can be broken down based on the needs of the stakeholders into;  
- Key Findings-Summary of the sales
- Actionable Insights
- Impact on Business      
- Proposed Strategic Actions     
- Recommendation        
- Conclusion          

## Tools used         
- Microsoft Excel(dataset)
- Power Query(for Data Cleaning)      
- Microsoft Power BI(Data Modelling,DAX Calculation and Dashbard Creation)

## Key Findings
-  The total sales across the years amount to 140.92 Million naira  from 2022 to 2024.
-  Benin has emerged as the top performing region contributing to 42.03 Million
   Naira to the total sales.     
-  Additionally,Quarter 4 stands out as the highest selling quarter with 35.69 Million naira in sales across the years.
-  Product E emerged as the best selling product across all regions with 28.4 million naira in sales.

  ## Sales By Year    
  <img src="https://i.ibb.co/2kLbfx4/Total-Sales-over-years.jpg" alt="Total-Sales-over-years" border="0">  
  The above line chart shows the Sales by year indicating an overall upward sales trend from 2022 to 2024.    

  ## Top Performing Region      
  <img src="https://i.ibb.co/KqsKZ0Y/Sales-By-Region-Sales.jpg" alt="Sales-By-Region-Sales" border="0">       
  The bar Chart highlights sales by region with Benin as the top performing region with a total sales of 42.03 Million naira.         

  ## Quarterly Sales Performance   
  <img src="https://i.ibb.co/Mkc6Xf9/Total-Sales-Over-Quarter.jpg" alt="Total-Sales-Over-Quarter" border="0">      

  ## Top Product Performance     
  <img src="https://i.ibb.co/cLRVbNs/Sales-By-Product.jpg" alt="Sales-By-Product" border="0">       
  Product E is the highest selling product achieving a total sales of 28.4 Million Naira across all the regions. This indicates  a strong preference and Market demand for Product E in all the regions.  
  
 ## Daily Sales Performance     
 <img src="https://i.ibb.co/wYWmg43/Total-Sales-By-Day.jpg" alt="Total-Sales-By-Day" border="0">   
 This line chart shows that there are more sales on weekends than on weekdays.    

 # Actionable Insights    
 - From our analysis, it is evident that Benin is a critical market contributing nearly 30% to our total sales.
 - Quarter 4 consistently emerges as the most lucrative period likely due to seasonal factors.
 - Product E came top as the best selling product across all regions indicating a strong preference of this product above all the other product.
 - Sales are significantly higher on Weekends compared to weekdays, suggesting that customers are likely to make more purchase during the weekend.

## Impact on Business    
-  Implementing these recommendations can significantly boost our overall sales and revenue.
-  By establishing dominance in key regions like Benin, we cam position ourselves as a market leader
-  Improved forecasting and resource allocation based on sales trend will also enhance our operational efficiency
-  Success in Benin can be used as a model for expanding into similar markets, potentially uncovering new revenue streams.
-  Enhanced marketing and targeted strategies can attract new customers and retain existing ones, leading to sustainable business growth.

    

## Proposed Strategic Actions    
I propose two strategic actions;    
-  Firstly, expand our presence in Benin by increasing our marketing budget and sales team.
-  Secondly, enhance our Quarter 4 readiness by developing targeted promotions and ensuring adequate inventory levels.

## Recommendations    
-  Based on this analysis, I will recommend focusing on Benin by enhancing our marketing and sales efforts.
-  Additionally, we can also optimize our Quarter 4 strategies by strengthening our campaigns and managing inventory efficiently to maximize sales during the peak period. We can also investigate the strategies and market conditions that have led to the increase  of sales in Benin and Quarter 4.,then apply these insights to other regions and quarters to elevate the overall sales performance.
-  Given the strong performance of Product E across all regions, allocate more marketing resources to promote Product E.
-  Optimizing Weekend Strategies: We can implement special promotions, discounts or events on weekends to capitalize on higher foot traffic and sales. This can further boost weekend sales across all products lines.


## Conclusion    
In conclusion, by leveraging these insights and implementing the recommended strategies, the business can enhance its market position, drive revenue growth, and improve operational efficiency, leading to a better overall business outcomes.     

## Project 5-Car Sales Analysis       
## Project Overview    
Our company is a car dealership that sells various car models. To effectively track and analyse our sales performance, we need a comprehensive Car Sales Dashboard in Power BI.     
<img src="https://i.ibb.co/Bqzvnvz/Car-Sales-Dashboard-pic.jpg" alt="Car-Sales-Dashboard-pic" border="0">         
<img src="https://i.ibb.co/Q6myxfD/Car-Sales-Dashboard-pic2.jpg" alt="Car-Sales-Dashboard-pic2" border="0">            

## Objectives     
The objective of this project is to design and develop a dynamic and interactive Car Sales Dashboard using Power BI. The dashboard will visualize critical KPIs related to our car sales, helping us understand our sales performance over time and make data-driven decisions.  
## Problem Statement 1: KPI’s Requirement          
The dashboard should provide real-time insights into key performance indicators (KPIs) related to our sales data. This will enable us to make informed decisions, monitor our progress, and identify trends and opportunities for growth.        
## 1.	Sales Overview:               
•	Year-to-Date (YTD) Total Sales        
•	Month-to-Date (MTD) Total Sales           
•	Year-over-Year (YOY) Growth in Total Sales           
•	Difference between YTD Sales and Previous Year-to-Date (PTYD) Sales           
## 2.	Average Price Analysis:         
•	YTD Average Price        
•	MTD Average Price        
•	YOY Growth in Average Price              
•	Difference between YTD Average Price and PTYD Average Price        
## 3.	Cars Sold Metrics:                     
•	YTD Cars Sold         
•	MTD Cars Sold        
•	YOY Growth in Cars Sold          
•	Difference between YTD Cars Sold and PTYD Cars Sold   

## Problem Statement 2: Charts Requirement     
-  YTD Sales Weekly Trend: Display a line chart illustrating the weekly trend of YTD sales. The X-axis should represent weeks, and the Y-axis should show the total sales amount.      
-  YTD Total Sales by Body Style: Visualize the distribution of YTD total sales across different car body styles using a Doughnut Chart.            
- 	YTD Total Sales by Color: Present the contribution of various car colors to the YTD total sales through a Doughnut chart.           
-  YTD Cars Sold by Dealer Region: Showcase the YTD sales data based on different dealer regions using a map chart to visualize the sales distribution geographically.            
-  Company-Wise Sales Trend in Grid Form: Provide a tabular grid that displays the sales trend for each company. The grid should showcase the company name along with their YTD sales figures.           
-  Details Grid Showing All Car Sales Information: Create a detailed grid that presents all relevant information for each car sale, including car model, body style, colour, sales amount, dealer region, date, etc

  ## Insights    
  ## YTD Sales Weekly Trend   
  <img src="https://i.ibb.co/7WFQgT3/YTD-Sales-Weekly-trend.jpg" alt="YTD-Sales-Weekly-trend" border="0">      


  ## YTD Total Sales By Body Style     
  <img src="https://i.ibb.co/YP20tyn/YTD-Total-Sales-By-Body-Style.jpg" alt="YTD-Total-Sales-By-Body-Style" border="0">        

  ## YTD Total Sales By Color     
  <img src="https://i.ibb.co/YZhkTv4/YTD-Total-Sales-By-Color.jpg" alt="YTD-Total-Sales-By-Color" border="0">         

  ## YTD Cars Sold By Dealer Region          
  <img src="https://i.ibb.co/p0pbWPd/YTD-Total-Sales-By-Dealer-Region.jpg" alt="YTD-Total-Sales-By-Dealer-Region" border="0">     

  ## Company-Wise Sales Trend     
  <img src="https://i.ibb.co/ssXrrp2/Company-wise-Sales-Trend.jpg" alt="Company-wise-Sales-Trend" border="0">       

  ## Details Grid Showing All Car Sales Information      
  <img src="https://i.ibb.co/QYBhCQv/Car-Sales-Details.jpg" alt="Car-Sales-Details" border="0">      

  ## Key Findings               
  -  Strong YOY Sales Growth: The company achieved a 23.59% increase in year-over-year (YOY) sales, with YTD total sales reaching $371.2 million, a difference of $70.8 million from the previous year.
  -  High MTD Sales Performance: Monthly-to-date (MTD) total sales are $54.2 million, indicating strong sales momentum for the current month.     
  -  Slight Decrease in Average Price: The YTD average price per car is $28,000, showing a minor decline from the prior year’s average of 0.22 thousand, a YOY drop of 0.79%.
  -  Notable Increase in Cars Sold: The number of cars sold YTD is 13.3 thousand, an increase of 2.6 thousand compared to last year, reflecting a 19.73% YOY increase.
  -  Stable MTD Average Price: The MTD average price is $28.26 thousand, showing relatively steady pricing.

## Actionable Insights  
-  Sales Expansion: With sales growth above 20% YOY, further investment in high-performing sales regions or digital channels can capitalize on the current momentum.       
-  Pricing Adjustments: Despite the high sales volume, the slight drop in average price suggests potential room for improved pricing strategies or premium offerings, especially since demand appears strong.               
- Inventory Management: With the 19.73% growth in cars sold, reviewing inventory and supply chain strategies may ensure the company can sustain this demand without shortages or delays.

  ## Impact on Business
  -  Revenue Growth: The significant YOY sales growth positively impacts overall revenue and could strengthen the company’s market share in the industry.     
  -  Market Position: The increase in units sold implies the brand is resonating well with consumers, which could enhance customer loyalty and brand reputation.    
  -  Profit Margins: Slightly lower average prices may slightly impact margins, depending on cost structure, but higher sales volumes could offset this.        

   ## Recommendations    
  -  Enhance Sales Channels: Invest in expanding high-performing sales channels or exploring new marketing initiatives to sustain the YOY growth trend.    
  -  Optimize Pricing: Consider targeted price increases in areas or segments where demand is strongest or where customers are less price-sensitive.      
  -  Focus on Premium Offerings: Explore adding premium car models or feature-rich versions to elevate the average price and capture more value per sale.     
  -  Strengthen Inventory Planning: Monitor inventory closely to ensure the supply meets rising demand without risk of overstock or shortages.
 
  # Project 6-Adidas Sales Analysis
  ## Project Overview     
   Through this PowerBI-driven analysis, Adidas aims to empower its decision makers with the data driven  insights, fostering strategic growth and competitiveness in the dynamic sports and athletic industry.               
- Enhanced understanding of sales dynamics and performance driven.       
- Identification of geographical areas with high and low potential sales.         
- Insights into product performance, aiding in inventory and marketing decisions         
- Informed pricing and margin strategies for improved profitability.         
- Actionable recommendations for optimizing sales and profit across various dimensions.   
  <img src="https://i.ibb.co/mHBJTPC/Adidas2.jpg" alt="Adidas2" border="0">              

# Problem Statement         
## Key Performance Indicators(KPIs)         
**Total Sales Analysis**         
- Understand the overall sales performance of Adidas over time        
**Profitability Analysis**          
- Evaluate the total profit generated by Adidas across different dimensions.      
**Sales Volume Analysis**            
- Examine the total units sold to gain insights into product demands              
**Pricing Strategy**              
- Determine the average price per unit to access the pricing strategy         
**Margin Analysis**          
- Evaluate the average margin to understand the overall profitability of sales.

## Charts Requirements         
- Total Sales By Month(Area Chart)-Visualize the monthly distribution of total sales to identify peak periods.      
- Total Sales By State(Filled Map)-Geographically represent total sales across different states using a filled map.     
- Total Sales By Region(Donut Chart)-Use a donut chart to represent  the contribution of different regions to total sales.     
- Total Sales By Product(Bar Chart)- Analyze the sales distribution among various Adidas products using a bar chart.   
- Total Sales By Retailer(Bar Chart)-visualize the contribution of different retailers to total sales using a bar chart     
  <img src="https://i.ibb.co/mHBJTPC/Adidas2.jpg" alt="Adidas2" border="0">
  
## KEY FINDINGS       
- Total Sales-$900M     
- Operating Profit-$332M      
- Sales Volume-$2M     
- Price Per Unit-$45      
- Operating Margin-42%      
- Product Contribution: A bar chart depicting product category contributions, with Men’s Street Footwear dominating.     
- Retailer Breakdown: A bar chart ranking retailer performance, with West Gear leading the chart.     
- Trend Analysis: An  Area chart showing monthly sales, highlighting July and August peaks.

  ## Top Performing Retailer    
  <img src="https://i.ibb.co/7N0yF0X/Total-SALES-By-Retailer.jpg" alt="Total-SALES-By-Retailer" border="0">                                     
  
    ## West Gear leads as the top retailer, generating $242,964,333 in total sales.        

  ## Highest Grossing product
  <img src="https://i.ibb.co/8PddbfS/Total-sales-By-Product.jpg" alt="Total-sales-By-Product" border="0">                                     
  
    ## Men’s Street Footwear takes the spotlight as the highest-grossing product, contributing $208,626,244 to total sales.      

  ## Total Sales By Month
  <img src="https://i.ibb.co/s15hMhs/Total-Sales-By-Month-Adidas2.jpg" alt="Total-Sales-By-Month-Adidas2" border="0">                      
  
    ## The highest sales by Month are July and August indicating  peak periods for July and Augiust          

# Data Storytelling: Business Insights Overview   
## Key Performance Metrics
**Total Sales**: The business achieved an impressive $900M in total sales, reflecting robust market presence and strong customer demand.
Operating Profit: A noteworthy $332M operating profit was realized, indicating a healthy profitability framework.      
**Sales Volume**: With 2M units sold, the business demonstrates significant product demand.        
**Price Per Unit**: The average price per unit stands at $45, signifying competitive pricing in the market.      
**Operating Margin**: An outstanding 42% operating margin highlights the efficiency of cost management and revenue generation strategies.     
<img src="https://i.ibb.co/R0KgWxp/KPIs.jpg" alt="KPIs" border="0">        

## Top Performing Retailer      
- West Gear leads as the top retailer, generating $242,964,333 in total sales.       
- This retailer's dominance could be attributed to effective marketing, customer loyalty,     
or superior product assortment.      
## Highest Grossing Product           
- Men’s Street Footwear takes the spotlight as the highest-grossing product, contributing $208,626,244 to total sales.     
- This category's strong performance signals a trend in consumer preferences for stylish and functional men’s footwear.  
## Profitability and Efficiency:          
- The 42% operating margin and significant operating profit reflect strong cost-control measures and strategic pricing.
This financial health provides opportunities for reinvestment in growth areas.       
## Retailer and Product Insights:           
- West Gear and Men’s Street Footwear are standout performers, signaling key areas to scale or replicate success.     
- Focused marketing and inventory optimization for these segments can yield further gains.     
## Seasonality:          
- The sales surge in July and August offers an opportunity to strengthen summer campaigns and inventory planning.

  # Recommendations
  ## Expand High-Performing Product Lines:       
- Invest in product innovation and marketing for Men’s Street Footwear to capitalize on its market appeal.      
- Explore complementary products to cross-sell within the footwear category.        
## Strengthen Partnership with West Gear:        
- Enhance collaborations with West Gear, leveraging their success to pilot new launches and exclusive collections.   
- Use their sales insights to refine retailer strategies for other partners.       
## Leverage Seasonality:       
- Develop targeted promotions and inventory strategies for July and August to maximize seasonal sales spikes.     
- Consider launching campaigns earlier to capture pre-season interest.     
## Optimize Price-Performance:       
- With a $45 price per unit, ensure products maintain competitive pricing without compromising the operating margin.    
- Assess the feasibility of premium pricing for high-demand categories like Men’s Street Footwear.      
  
# Project 7-Financial Loan Analysis
## Objectives:   
The main objective of this project is to analyse various KPIs metrics that can be used to access loan applications.    
 <img src="https://i.ibb.co/jv1tngvD/Bank-loan-report.jpg" alt="Bank-loan-report" border="0"> 
 
 <img src="https://i.ibb.co/1YvXwKT5/Bank-loan-Overview.jpg" alt="Bank-loan-Overview" border="0">       

 <img src="https://i.ibb.co/prWNpszb/BANK-LOAN-REPORT-DETAILS.jpg" alt="BANK-LOAN-REPORT-DETAILS" border="0">             

## Problem Statement                                        
## Key Performance Indicators (KPIs) Requirements:                                              
-- 1.	Total Loan Applications: We need to calculate the total number of loan applications received during a specified period. 
Additionally, it is essential to monitor the Month-to-Date (MTD) Loan Applications and track changes Month-over-Month (MoM).                            
-- 2.	Total Funded Amount: Understanding the total amount of funds disbursed as loans is crucial. We also want to keep an eye on the MTD Total Funded Amount and analyse the Month-over-Month (MoM) changes in this metric.                           
-- 3.	Total Amount Received: Tracking the total amount received from borrowers is essential for assessing the bank's cash flow and loan repayment. We should analyse the Month-to-Date (MTD) Total Amount Received and observe the Month-over-Month (MoM) changes.                            
-- 4.	Average Interest Rate: Calculating the average interest rate across all loans, MTD, and monitoring the Month-over-Month (MoM) variations in interest rates will provide insights into our lending portfolio's overall cost.                                       
-- 5.	Average Debt-to-Income Ratio (DTI): Evaluating the average DTI for our borrowers helps us gauge their financial health. We need to compute the average DTI for all loans, MTD, and track Month-over-Month (MoM) fluctuations.          

## Key Findings       
## KPIs     
-- 1.Loan Applications    
•	Total Applications: 36.8K         
•	MTD Applications: 4.3K       
•	MoM Growth: +6.9%   


-- 2. Loan Funding Performance
•	Total Funded: $435.8M      
•	MTD: $54M       
•	MoM Growth: +13%      

-- 3. Collection Efficiency         
•	Total Received: $473.1M        
•	MTD: $58.1M           
•	MoM Growth: +15.8%        

-- 4. Interest Rate Trends        
•	Avg Rate: 12.05%       
•	MTD: 12.4%       
•	MoM Change: +3.5%     

-- 5. Debt-to-Income (DTI) Ratio        
•	Avg DTI: 13.33%       
•	MTD: 13.7%      
•	MoM Increase: +2.7%     

## Good Loan Issued    
<img src="https://i.ibb.co/XZHZ5VDS/Good-loan-issued.jpg" alt="Good-loan-issued" border="0">       



## Bad Loan Issued   
<img src="https://i.ibb.co/fYvCny24/Bad-Loan-Issued.jpg" alt="Bad-Loan-Issued" border="0">    

## Insights       
-- Loan applications continue to grow steadily MoM, indicating sustained borrower demand.   
-- Funded amounts are rising at a faster pace than applications — potential increase in approval rates or loan sizes.     
-- Repayment trends are healthy with a notable 15.8% growth — outpacing disbursal increases.    
-- Rising interest rates may increase revenue per loan but could deter sensitive borrowers.     
-- Slight uptick in DTI suggests growing borrower obligations. Risk of default may increase if trend continues.    

 ## Recommendation   
 -- Enhance marketing outreach to further capitalize on increasing demand trends.   
 -- Review underwriting practices to ensure sustained credit quality amidst higher funding rates.    
 -- Consider rewarding early or regular payers with interest discounts or loyalty programs to retain good borrowers.    
 -- Monitor competitive rates and test rate elasticity in key borrower segments.     
 -- •	Tighten approval criteria for borrowers with DTI > 15%.    
 -- •	Offer financial planning resources to educate borrowers on responsible borrowing.  

 ## Conclusion         
 -- Demand and repayment trends are strong.    
--  Credit risk is rising modestly (via DTI), requiring proactive risk management.    
--  Interest rates should be managed carefully to maintain borrower affordability.      

# Project 8-Ecommerce Sales Analysis       

## Problem Statement                   
A US Based e-commerce Sales company wants to create a Sales Dashboard showing information of YTD Sales and generate insights for the following scenarios:         
-- Create a KPI Banner showing YTD sales, YTD Profit, YTD Quantity Sold and YTD Profit Margin      
-- Find Year on Year Growth for each KPI and show a YTD Sparkline for each measure in the KPI to understand the monthly trend for each fact.           
-- Find the YTD Sales, PYTD Sales, YoY Sales Growth for different customer category. Add a trend icon for each category.           
-- Find the YTD Sales performance for each state           
-- Top 5 and bottom 5 Products By  Sales        
-- YTD Sales By region to know the best and worst performing region all over the country.                
-- YTD Sales By shipping type to get the best shipping type by percentage.        

<img src="https://i.ibb.co/twtjs4gS/Ecommerce1.jpg" alt="Ecommerce1" border="0">    


## Key Findings    
## KPIs       
-- YTD Sales is $11.53 Million   
-- YTD Profit is $1.34 Million   
-- YTD Quantity is 107.2k    
-- YTD Profit Margin is 11.58%     

## Top 5 Products       

<img src="https://i.ibb.co/DHJvLC1r/Top-5-Products-By-YTD-Sales.jpg" alt="Top-5-Products-By-YTD-Sales" border="0">        

-- Staple Envelope came top as the 5 best selling Products with a YTD Sales of $57k    

## Bottom 5 Products     

<img src="https://i.ibb.co/N6RGZpdk/Bottom-5-Products-By-YTD-Sales.jpg" alt="Bottom-5-Products-By-YTD-Sales" border="0">    

-- Rediform S.O.S came out as the worst selling Product.       

## YTD Sales By Shipping Type   

<img src="https://i.ibb.co/Mkdp5FLw/YTD-Sales-By-Shipping-Type.jpg" alt="YTD-Sales-By-Shipping-Type" border="0">    

-- Standard Class came top as the highest YTD Sales of $7M (60.51%)    

## YTD Sales By Region      

<img src="https://i.ibb.co/jkB8QC34/YTD-Sales-By-Region.jpg" alt="YTD-Sales-By-Region" border="0">       

-- Western Region is the highest selling region with a YTD Sales of $3.72M (32.22%)    

## Sales By State    

<img src="https://i.ibb.co/tP21YZN1/Sales-By-State.jpg" alt="Sales-By-State" border="0">      

-- California is the highest selling State with a YTD Sales of $2.3 Million        

# Insights        

📊 Business Performance Insights (YTD)           
✅ Positive Trends                
Profit Growth Despite Sales Dip:                          
Profit grew by 4.5% YoY, reaching $1.34M, even though sales slightly declined (-0.83% YoY).     
➤ Indicates improved cost efficiency, pricing strategy, or shift toward high-margin products.          

Strong Profit Margin Performance:    
YTD profit margin is 11.58%, with a 5.37% YoY increase, showcasing operational improvements and better profitability management.   

⚠️ Areas of Concern        
Decline in Sales Volume:             
YTD quantity sold dropped by 7.29% YoY to 107.2k units.              
➤ This volume decline is disproportionately larger than the sales drop, implying possible price increases, product mix changes, or market share loss.          

Flat Revenue Growth:             
YTD sales at $11.53M, with a marginal YoY decline of 0.83%, suggests stagnant demand or competitive pressures.      

## Recommendation     
🎯 Strategic Recommendations          
## 1. Investigate Volume Decline            
Deep dive into the 7.29% drop in quantity: identify if specific regions, product categories, or customer segments are underperforming.   

Consider promotions, product bundling, or channel optimization to drive volume recovery.        

## 2. Leverage High-Margin Segments         
Double down on products or services contributing to the rising profit margin.        

Analyze the drivers of margin growth (e.g., cost control, product mix) and scale best practices across the business.        

## 3. Enhance Demand Generation         
With flat sales and dropping volume, invest in targeted marketing campaigns, cross-sell/upsell strategies, and customer retention initiatives.        

Reevaluate pricing strategies to ensure competitiveness without eroding margins.       

## 4. Monitor Competitive Dynamics        
Explore whether sales volume decline is due to competitive encroachment or market shifts.        

Benchmark against peers to understand performance gaps and adjust positioning accordingly.        

## 5. Forecast Risks and Sustainability            
Determine if profit improvements are structural (sustainable) or one-off.          

Plan ahead to maintain margins in the face of potential input cost increases or volume pressures.












Installation
Install my-project with npm

  npm install my-project
  cd my-project
