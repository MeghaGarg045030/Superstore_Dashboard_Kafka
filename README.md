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
![Complete Graph](https://github.com/user-attachments/assets/c7c400c1-aa3c-4525-9eae-e3d6338e9f29)


<br>
<br>

**Description:** The video demonstrates, the dynamic capabilities of the dashboard built using the ELK Stack. The focus is on utilizing controls and filters to interact with the data in real-time. By applying various filters, such as timestamp, state and subcategory, the dashboard dynamically updates to reflect the selected criteria. Controls like dropdown menus, and sliders, allow seamless customization and exploration of the dataset. This interactive approach helps users in data-driven decision-making.

<br>

[Video.webm](https://github.com/user-attachments/assets/882566ff-2d67-45b8-9495-c318cf56a477)


<br>
<br>

## Charts<br>

1. What is the total revenue generated over the specified time period?<br>

   <ins>**Total Revenue** </ins>

   **Description:** The purpose of this graph is to provide a quick, high-level overview of the total revenue earned. It is a key performance indicator (KPI) often displayed prominently in dashboards to communicate financial performance at a glance.

   ![Graph-1](https://github.com/user-attachments/assets/da5b5d94-e353-49d6-afdc-a056c6079c82)


- The business or project generated a total revenue of 8,731,336 (units depend on the currency or scale used in the data). 
- This figure can serve as a baseline to compare against revenue targets, previous periods, or industry benchmarks.
- If part of a time-series analysis, it could prompt further investigation into what factors contributed to achieving this revenue level.


<br>
<br>

2. What percentage of the total revenue is derived as profit?<br>

   <ins>**Percentage of Profit by Revenue**</ins>

   **Description:** The purpose of this KPI is to highlight the profitability of the business or project relative to its revenue. It is a critical measure of operational efficiency and financial health.

   ![Graph-2](https://github.com/user-attachments/assets/fc1416f5-54d7-4e12-abb1-e7cad1b29184)


   **Profitability Ratio:** The profit margin is 29.317%, indicating that for every 100 units of revenue, the business retains 29.317 units as profit. 
   **Performance Indicator:** A profit percentage of this level could be considered strong or weak depending on the industry. For example, industries like technology may have higher margins, while manufacturing or retail could have lower ones.
   **Actionable Insights:** This metric could prompt further analysis into costs or operational efficiencies if the percentage is below expectations. Conversely, a high profit margin could signal strong cost control and pricing strategies


<br>
<br>

3. What is the average number of days taken for delivery?<br>

   <ins>**Average Delivery Days**</ins>

   **Description:** The purpose of this KPI is to monitor the efficiency of the delivery process and assess whether the organization is meeting delivery time targets. It serves as a critical metric in evaluating customer satisfaction and operational performance.

   ![Graph-3](https://github.com/user-attachments/assets/f6320ca4-a740-4b6e-897e-e73cd18ff6fb)


   **Average Delivery Time:** The average delivery time is 3.097 days, meaning it typically takes just over 3 days to fulfill and deliver orders.
   **Performance Analysis:** If the target delivery time is under 3 days, this metric suggests there might be slight delays in the process. Conversely, if the goal is under 4 days, this is a positive result.
   **Actionable Steps:** If delivery time exceeds expectations, factors such as logistics, supply chain bottlenecks, or operational inefficiencies should be reviewed. Consistently low delivery times could be leveraged as a competitive advantage in marketing efforts.


<br>
<br>

4. How is profit distributed across different business segments (Consumer, Corporate, Home Office)?<br>

   <ins>**Profit by Segment**</ins>

   **Description:** To identify which segment contributes the most or least to overall profitability. This can help focus business strategies on high-performing segments and address challenges in underperforming ones.

      ![Graph-4](https://github.com/user-attachments/assets/23415ae9-f88c-4b6e-a47e-5a5eb7f20895)


   The **Consumer segment dominates profitability**, reflecting strong demand or higher margins, possibly driven by effective marketing and sales efforts or higher transaction volumes. The Corporate segment contributes moderately, suggesting potential for growth through tailored products, bulk discounts, or enhanced services. In contrast, the Home Office segment has the lowest profitability, likely due to low sales volume, higher costs, or limited focus. A deeper analysis is needed to determine whether to invest in growing this segment or reallocate resources to stronger areas.

<br>
<br>

5. How have sales accumulated over time? What is the trend in sales performance over a given period?<br>

   <ins>**Sales Timeline**</ins>

   **Description:** To visualize the growth of sales over time and understand whether there is a consistent increase or decline in sales. It helps track how well sales are progressing and at what rate they are growing.
   
   ![Graph-5](https://github.com/user-attachments/assets/91369747-656c-410f-b07c-84606d1b6dd6)


   The chart shows a **steady increase in sales** over time, suggesting that sales have been growing consistently. The **steep slope** at certain points indicates periods of higher growth, while the **gradual increase** at others shows slower growth. Overall, the trend is **positive**, indicating that sales are continuously rising.


<br>
<br>

6. What are the total sales for each sub-category within the main product categories (Technology, Furniture, and Office Supplies)?<br>

   <ins>**Sales by Category and Sub- Category**</ins>

   **Description:** This graph aims to compare sales performance across different sub-categories within the three main product categories. It helps in identifying which sub-categories contribute the most to total sales and where there may be opportunities for improvement.

   ![Graph-6](https://github.com/user-attachments/assets/4aacb3e8-b087-4c7c-8278-93a4246a4a70)


   Technology leads in sales, driven by Phones and Copiers, with Accessories and Machines contributing less significantly. Furniture follows, with Chairs and Tables dominating, while Bookcases and Furnishings make moderate contributions. Office Supplies lag behind, with Appliances and Storage contributing modestly, and minimal impact from Binders and Paper. Optimizing strategies around high-performing sub-categories like Phones, Chairs, and Copiers, while analyzing weaker sub-categories, could enhance overall sales performance.

<br>
<br>

7. How do discounts affect profit across different sub-categories of products?<br>

   <ins>**Discount Impact on Profit**</ins>

   **Description:** The graph aims to evaluate the relationship between the level of discounts and the corresponding profit for various sub-categories. This information helps in understanding whether higher discounts lead to increased profitability or if they negatively impact the bottom line.
   
   ![Graph-7](https://github.com/user-attachments/assets/23252ffb-442c-4d44-a30c-bd1744e20473)


   Sub-categories with moderate discounts (0.5–0.6) generally maintain better profitability, while higher discounts (>0.7) erode profits. Phones stand out with decent profits even at higher discounts, indicating strong demand. Chairs show the highest profitability within specific discount ranges but suffer from excessive discounts, while Tables and Copiers display moderate profitability that declines with higher discounts. In contrast, Appliances, Bookcases, and Accessories show low profit margins across all discount levels, suggesting discounts are less effective for these sub-categories. Overall, moderate discounts optimize profitability across most sub-categories.

<br>
<br>

8. Which cities contribute the most to revenue, and how is the revenue distributed across various cities?<br>

   <ins>**Citywise Revenue**</ins>

   **Description:** The purpose of this word cloud is to visualize city-wise revenue contributions in a clear and engaging way. Larger fonts indicate higher revenue contributions, helping identify key cities driving sales.
      
   ![Graph-8](https://github.com/user-attachments/assets/03298918-8b1b-44aa-9ead-0f2195a8a4d9)


   Sydney leads in revenue contribution, followed by cities like Gold Coast, Mexico City, London, and Brisbane, indicating key markets or business hubs. Moderate contributors include Jakarta, Bangkok, Manila, Melbourne, and Adelaide, which may offer growth potential. Smaller cities like Thiruvananthapuram and Gorakhpur contribute minimally, reflecting niche or limited markets. The revenue base is geographically diverse, with a stronger focus on regions like Australia and Asia.

<br>
<br>

9. Which customers generate the highest revenue and profitability for the company?<br>

   <ins>**Top 20 Countries by Sales and Profit**</ins>

   **Description:** The purpose of the graph is to identify the top-performing customers in terms of revenue and profit while analyzing the relationship between sales and profit across these key customers. It helps in making data-driven decisions by highlighting which customers contribute the most to overall business performance and where efforts should be focused to nurture high-value customer relationships effectively.
   
   ![Graph-9](https://github.com/user-attachments/assets/8f630c4c-2ae4-4bb2-a5e3-1b1a1d482e50)


   Adrian Barton leads as the top customer, generating the highest sales and profit, followed by significant contributors like Adam Bellavance and Dave Porter. Customers such as Alan Hwang and Ann McFarland show lower profit margins relative to sales, while Chuck Sachs and Jennifer Ferguson have higher profit margins. Among the top 20 customers, performance varies, with some excelling in sales volume and others contributing more through higher profit margins.


<br>
<br>
   
10. Which category generates the most revenue?<br>

    <ins>**Category wise Total Sales**</ins>

    **Description:** The purpose of the graph is to compare sales performance across different product categories and identify how they perform relative to predefined thresholds. It highlights the top-performing categories, such as Technology, while also drawing attention to underperforming ones, like Office Supplies. This allows for a quick assessment of overall performance and helps prioritize actions to boost sales in lagging categories or sustain growth in high-performing ones.
    
    ![Graph-10](https://github.com/user-attachments/assets/60db048a-3f61-4c1e-9032-fc5d6a258107)


    Technology leads in sales with 3,550,216, indicating strong performance, followed by Furniture at 2,976,622, which is near the next performance threshold. Office Supplies trails significantly at 1,677,568. Growth opportunities include pushing Technology sales beyond 4,000,000, boosting Furniture to transition into a higher performance zone, and implementing strategic initiatives to improve Office Supplies sales. A strategic focus on sustaining Technology’s momentum and promoting Furniture and Office Supplies through targeted campaigns or pricing strategies can drive overall growth.

<br>
<br>

11. What is the impact of selecting a specific date on the displayed data?<br>

    <ins>**Date Slider**</ins>

    **Description:** The purpose of the graph is to allow users to filter and analyze data for a specific time period or date. It enables dynamic interaction with the dataset by focusing on orders from a chosen date, providing flexibility for temporal analysis of trends or patterns. This feature ensures ease of use by offering options to apply, cancel, or clear selections, making it an effective tool for targeted analysis of specific time frames.
    
    ![Graph-11](https://github.com/user-attachments/assets/a29d42b7-0688-4696-935e-d997ec425616)


    Interactive filtering allows users to analyze metrics like sales and profit for specific dates, such as April 15, 2015. The "Apply changes" and "Cancel changes" options enhance usability by enabling confirmation or reversal of selections. This feature supports custom analysis, making it valuable for tracking performance during key periods like product launches, seasonal sales, or financial reporting.


<br>
<br>

12. What is the specific year for which data needs to be analyzed or filtered on the dashboard?<br>

    <ins>**Year Slider**</ins>

    **Description:** The purpose of the year slider is to provide an interactive tool for users to filter the data displayed on the dashboard based on a selected year (in this case, 2012). It helps users focus on insights for a specific timeframe.
    
    ![Graph-12](https://github.com/user-attachments/assets/f3f243f1-f4e3-4f90-9d50-50f837f93051)


    This graph does not provide direct insights but acts as a filtering mechanism for the dashboard. By selecting "2012" (or any other year), the user can dynamically adjust the other graphs and visualizations on the dashboard to reflect data corresponding to the chosen year.



<br>
<br>


## Managerial Insights<br>

- Revenue and Profitability Analysis<br>
  - **Total Revenue:**: The organization generated significant revenue of 8,731,336 units, which can serve as a benchmark for evaluating financial performance.<br>
  - **Profitability**: With a profit margin of 29.317%, the business demonstrates operational efficiency. However, further cost analysis might be required if this ratio is below industry standards.<br>

- Segment-Wise Profit Distribution<br>
  - The Consumer segment dominates profitability, highlighting the effectiveness of marketing strategies targeted at individual consumers.<br>
  - The Corporate segment performs moderately, suggesting potential for growth through tailored business solutions.<br>
  - The Home Office segment underperforms, necessitating a strategic review.<br>

- Product Category Insights<br>
  - Technology leads in revenue, driven by sub-categories like Phones and Copiers, which should remain a strategic focus.<br>
  - Furniture and Office Supplies offer opportunities for improvement through marketing or product diversification.<br>

- Discount and Profit Relationship:<br>
  - Sub-categories like Phones and Chairs maintain profitability even with higher discounts, while excessive discounts negatively impact others like Tables and Accessories. A calibrated discounting strategy is essential.<br>

- Geographical Insights<br>
  - Cities like Sydney and London dominate revenue contributions, emphasizing the importance of sustaining operations in these areas.<br>
  - Moderate contributors like Jakarta and Bangkok could benefit from targeted growth initiatives.

<br>
<br>

## Conclusion<br>

The insights derived from this dataset emphasize the organization's strengths in revenue generation, profitability, and market presence. However, there are clear opportunities for growth in underperforming segments, sub-categories, and geographical regions. The positive sales trends and robust consumer demand suggest that the business is well-positioned to capitalize on its strengths while addressing inefficiencies.
To maximize potential, management should focus on:
1.	Enhancing profitability in lagging segments like Home Office.
2.	Optimizing operational efficiencies in shipping and delivery.
3.	Leveraging high-performing sub-categories like Phones and Chairs while reevaluating low-margin ones.
4.	Expanding market reach in moderately contributing cities and customer segments.

With strategic focus and data-driven decision-making, the organization can sustain growth and achieve long-term success.
