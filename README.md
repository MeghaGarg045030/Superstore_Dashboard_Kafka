# Superstore Dashboard 

The Superstore Sales Dashboard is a comprehensive tool developed using the Kafka, ELK (Elasticsearch, Logstash, and Kibana) stack and Flink KSQL Database to visualize and analyze sales data from the huge market. This dashboard extracts valuable insights from a dataset containing detailed information about transactions across various countries and states in different countries.

![image](https://github.com/user-attachments/assets/aa502599-7fd6-4051-8dad-266d412cdee8)


## About Dataset<br>

<a href="https://www.kaggle.com/datasets/anandku79/kpidashboard?select=superstore+%281%29.csv">Dataset Link</a>

<br>

![image](https://github.com/user-attachments/assets/d3d3c1a5-03de-46ba-86aa-0443fe467ce4)


<br>
The dataset captures a comprehensive view of a superstore's operations, offering rich transactional details. It includes information about individual orders such as order IDs, dates, shipping modes, and customer demographics. Additionally, it provides sales and profit metrics, enabling analysis of financial performance. The dataset is segmented by customer types, geographic locations (cities, states, and countries), and product categories, making it valuable for exploring market trends and customer preferences.

Key uses of this dataset include identifying high-value customers,sales trends, assessing delivery performance, evaluating discounts' effects on profitability, and optimizing logistics. It supports predictive analytics, customer segmentation, and operational efficiency improvements.

<br>

### Column description:
- Index: Row index for data reference.<br>
- OrderID: Unique identifier for each order.<br>
- OrderDate: Date when the order was placed.<br>
- ShipDate: Date when the order was shipped.<br>
- ShipMode: Shipping method used (e.g., FirstClass, SecondClass).<br>
- CustomerID: Unique identifier for each customer.<br>
- CustomerName: Name of the customer.<br>
- Segment: Customer segment (e.g., Consumer, Corporate).<br>
- City: City of the customer or delivery.<br>
- State: State of the customer or delivery.<br>
- Sales: Sales revenue generated from the order.<br>
- Quantity: Quantity of items in the order.<br>
- Discount: Discount applied to the order.<br>
- Profit: Profit earned from the order.<br>
- ShippingCost: Cost incurred for shipping.<br>
- OrderPriority: Priority level of the order (e.g., High, Critical).<br>
- DeliveryDays: Number of days taken for delivery.<br>
- OrderYear: Year of the order.<br>
- OrderMonth: Month of the order.<br>
- ISO_CODES: ISO country codes for geographic location.<br>

<br>

## Dashboard
![Complete Dashboard](https://github.com/user-attachments/assets/d27eae90-e264-4bf7-92a9-e4254ce06918)

<br>
<br>

**Description:** The video demonstrates, the dynamic capabilities of the dashboard built using the ELK Stack. The focus is on utilizing controls and filters to interact with the data in real-time. By applying various filters, such as timestamp, state and subcategory, the dashboard dynamically updates to reflect the selected criteria. Controls like dropdown menus, and sliders, allow seamless customization and exploration of the dataset. This interactive approach helps users in data-driven decision-making.

<br>

[ELK_Dashboard_Video.webm](https://github.com/user-attachments/assets/97faec29-08c1-4621-b8ac-98352e7b573f)

<br>

[Video_ELK_2.webm](https://github.com/user-attachments/assets/e78829c3-d911-4843-aa3a-e77eb5418626)

<br>
<br>

## Charts<br>

1. Which age group contributes the most revenue to the business product category wise?<br>

   <ins>**Age Group Sales Distribution by Product Category** </ins>

   **Description:** This bar chart displays sales values for Accessories and Clothing across two age groups: Adults (35-64) and Youth (<25). It helps identify the core 
   customer demographic and their product preferences, supporting targeted marketing strategies and refined efforts for youth-focused campaigns.

   ![Graph -1](https://github.com/user-attachments/assets/cce62f8a-b604-42b6-b68b-4c221c7cda02)

   The graph shows that **Adults (35-54)** generate the highest revenue across all product categories, with **clothing** being the dominant contributor, followed by 
   **Accessories**. **Young Adults (25-34)** rank second in revenue, while **Youth (<25)** contribute the least. This indicates that marketing efforts should focus on 
   **Adults** and enhancing engagement with the **younger age group**.

<br>
<br>

2. How has the revenue trended over time compared to profit?<br>

   <ins>**Revenue and Profit Trend Over Time**</ins>

   **Description:** This line chart illustrates trends in revenue and profit over a specific time period, highlighting fluctuations and divergences between the two metrics. 
   The chart provides insights into financial performance dynamics, helping to analyze volatility drivers and stabilize profits during revenue fluctuations.

   ![Graph -3](https://github.com/user-attachments/assets/bd00d6b9-5ae8-4af3-b02c-01292d6ddbc5)

   The graph shows that revenue is consistently higher than profit over time, with significant fluctuations in both. A notable gap exists between revenue and profit, 
   suggesting high operating costs or expenses. This dynamic environment highlights the need for deeper analysis to identify causes of volatility, manage risks, and 
   leverage periods of growth.

<br>
<br>

3. How does revenue change over time?<br>

   <ins>**Revenue Over Time**</ins>

   **Description:** This line chart tracks revenue over time, showcasing spikes and fluctuations in customer demand or event-driven sales. The chart identifies drivers 
   behind revenue spikes, optimizes strategies for low-revenue periods, and smoothens revenue fluctuations for consistent performance.

   ![Graph -2](https://github.com/user-attachments/assets/cdbebb72-f1dc-49b2-adb7-5cebbe3bbe38)

   Revenue spikes occur periodically without a steady trend, reflecting dynamic customer behavior or event-driven sales. Understanding the drivers of these peaks (e.g., 
   promotions or seasonal demand) can help smooth revenue fluctuations and optimize strategies for periods of lower activity.

<br>
<br>

4. What are the top 5 sub-categories by profit margins, and how do they compare?<br>

   <ins>**Product Profit Margin Analysis by Subcategory**</ins>

   **Description:** This donut chart displays profit margins for various product subcategories, ranking them from highest to lowest. It enables prioritization of high- 
   margin products and exploration of opportunities to improve profitability in lower-margin items.

   ![Graph -4](https://github.com/user-attachments/assets/d86a96f9-05d6-408f-9d50-ff27dfe7c8b4)

   The key insight is that **Bottles and Cages** lead profit margins **(58.52%)**, followed by **Bike Racks (21.98%)** and **Bike Stands (14.58%)**, while **Cameras and 
   Electronics** are relatively low **(4.92%)**. This indicates the need to focus on the most profitable categories to drive profitability further while exploring 
   opportunities to improve lower-margin products.

<br>
<br>

5. Which states have the highest sales revenue for the top 6 products?<br>

   <ins>**Sales Performance Analysis by Products**</ins>

   **Description:** This heat map chart visualizes sales performance by geographic regions, such as California, British Columbia, and England. The chart aids in sustaining 
   growth in high-performing regions and identifies potential for expansion in underperforming markets.
   
   ![Graph -8](https://github.com/user-attachments/assets/b017d811-acbb-4d4e-a16b-93b3a4be2fa0)

   **California** leads in **product sales**, with **British Columbia** and **England** also showing strong performance. Other states show moderate sales, indicating a need 
   to focus efforts on these top-performing regions and products for better overall revenue.

<br>
<br>

6. What are the key regions for further investment and growth opportunities?<br>

   <ins>**Country-Wise Revenue**</ins>

   **Description:** This map shows the revenue contribution of different countries, providing a comparative analysis of global market performance. It guides resource 
   allocation in dominant markets while identifying emerging regions and untapped potential for growth.

   ![Graph -5](https://github.com/user-attachments/assets/894ac8bb-c8b5-4290-a78d-f3848e73b60d)

   The map highlights Country-wise Profit, with **Canada** and the **United States** showing the highest profitability, followed by select regions in **Europe**. **Asia** 
   and **Oceania** show growth potential, while **South America** and **Africa** contribute minimally. A focus on optimizing top markets, while strategies for expanding in 
   Asia and Oceania, and penetrating low-performing regions, can drive global growth.

<br>
<br>

7. How do different product types compare in revenue contribution?<br>

   <ins>**Top Product by Revenue**</ins>

   **Description:** This word cloud chart ranks products by the revenue they generate, highlighting the best and worst-performing items. The chart informs resource 
   allocation for top-performing products and identifies areas for improvement in pricing or demand for underperforming items.
   
   ![Graph -10](https://github.com/user-attachments/assets/c97b54f4-636b-4d6c-b220-e39acd76d552)

   This word cloud highlights the top products by revenue, emphasizing items like the **Hitch_Rack_4_Bike** and **AWC_Logo_Cap**, which stand out as major revenue drivers 
   followed by **All_Purpose_Bike_Stand** and **Mountain_Bottle_Cage**.

<br>
<br>

8. What is the Country wise Ordered Quantity?<br>

   <ins>**Country-Wise Order Quantity**</ins>

   **Description:** This waffle chart displays order quantities by country, comparing sales volumes across different regions. It strengthens sales efforts in leading 
   markets and identifies opportunities to boost demand in underperforming regions for broader penetration.
      
   ![Graph -9 (1)](https://github.com/user-attachments/assets/a73927e5-5caf-4eaa-b131-96f99e67b02b)

   The **United States** leads in order quantity **(109,830 units)**, followed by Australia (61,395 units). While maintaining dominance in the U.S., strategies to boost 
   sales in underperforming regions like Germany and "Others" could unlock additional growth potential.

<br>
<br>

9. What proportion of total revenue is contributed by profit, and how does the average unit cost compare to the average unit price?<br>

   <ins>**Profit as a Part of Revenue**</ins>

   **Description:** This gauge chart illustrates the proportion of profit within total revenue, showcasing overall profit margin efficiency. It evaluates cost management 
   effectiveness, supports reinvestment decisions, and informs pricing strategies to maintain profitability.
   
   ![Graph -6](https://github.com/user-attachments/assets/dc4ff53f-050d-46be-a9b0-6a0da63e912e)

   Profit constitutes 50.3% of total revenue ($1.39M of $2.75M), indicating a healthy profit margin. This reflects efficient cost management, offering opportunities to 
   reinvest profits strategically for growth, optimize costs further, or develop sustainable pricing models to maintain profitability.

<br>
<br>
   
10. What proportion of total revenue is contributed by profit, and how does the average unit cost compare to the average unit price?<br>

    <ins>**Average Unit Cost as a Part of Average Unit Price**</ins>

    **Description:** This gauge chart compares the average unit cost with the average unit price, showing their relationship and cost-to-price ratio. The chart evaluates 
    pricing strategies, highlighting areas for cost reduction and ensuring competitive yet profitable pricing structures.

    ![Graph -7](https://github.com/user-attachments/assets/5d798dc7-17e0-4032-9d9e-d70f2698daf2)

    With an average unit cost of $5.76 making up 42.7% of the average unit price ($13.50), the business maintains a strong profit margin. This cost structure allows 
    competitive pricing while sustaining profitability. Strategic cost reductions or price adjustments could further enhance margins.

<br>
<br>

## Managerial Insights<br>
- Customer-Centric Marketing and Engagement<br>
  - **Prioritize the Adult Demographic (35–54)**: This age group generates the highest revenue across all product categories, particularly Clothing. Allocate marketing resources to campaigns targeting Adults, emphasizing Clothing and related accessories.<br>
  - **Expand Youth Engagement (<25)**: Youth (<25) contribute the least revenue, suggesting an opportunity to develop targeted campaigns and affordable product options to engage and grow this segment..<br>

- Regional Investment Prioritization<br>
  - **Enhance Performance in High-Revenue Markets**: North America (U.S. and Canada) and Europe are the strongest revenue-generating regions. Prioritize resource allocation, marketing, and supply chain optimization in these markets<br>
  - **Develop Potential in Emerging States**: States with moderate sales, such as South America and Africa, could benefit from increased promotional efforts, particularly improving distribution channels or launching region-specific products.<br>

- Profit-Oriented Product Strategy<br>
  - **Promote High-Margin Products**: Products like "Hitch_Rack_4_Bike" and "AWC_Logo_Cap" drive significant revenue.. Focus marketing and production efforts on these high-performing items to boost overall profitability.<br>
  - **Revise Strategy for Lower-Margin Products**: Evaluate sub-categories with lower profit margins and assess the feasibility of reducing production or enhancing value propositions.<br>

- Revenue and Profit Optimization<br>
  - **Close Revenue-Profit Gap**: The significant gap between revenue and profit highlights high operating costs. Conduct a cost analysis to identify inefficiencies in manufacturing, logistics, or marketing and implement measures to optimize expenditure.<br>
  - **Revenue and Profit Volatility**: Significant fluctuations in revenue and profit suggest a dynamic business environment. Investigating the underlying drivers of this volatility, such as promotions, seasonal demand, or market-specific factors, is essential. Implementing strategies to stabilize revenue trends while leveraging peak periods can enhance financial performance.<br>
  - **Implement Strategic Pricing Models**: With the average unit price significantly higher than the unit cost, consider introducing price segmentation strategies (e.g., premium pricing for high-demand products) to enhance profitability.<br>

- Market Expansion and Growth Strategies<br>
  - **Strengthen Leadership in Key Regions**: The U.S. leads in order quantities, followed by Australia, highlighting their importance as primary markets. Efforts should focus on maintaining this dominance.<br>
  - **Expand Market Share in Under performing Regions**: Regions like South America and Africa have the lowest revenue and order quantities. Implement localized marketing, improve distribution, and assess product relevance to penetrate these markets effectively.

<br>
<br>

## Conclusion<br>

To drive growth, the business should focus on high-performing markets like the U.S. and Australia while exploring emerging regions such as South America and Africa. Targeted marketing to adults (35–54) and engaging the youth segment will expand the customer base. Prioritizing high-margin products and optimizing costs will improve profitability. Addressing revenue and profit volatility through strategic pricing and cost management will stabilize performance. A balanced approach to market expansion and cost optimization will ensure sustained growth and strengthen the business’s competitive edge.
