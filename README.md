# Supply Chain Analysis - Power Bi

### Link to [Interactive Dashboard on novyPro](https://www.novypro.com/profile_about/ibrahim-saiied-1?Popup=memberProject&Data=1741967114105x160840138809370300) 

<div align="center">
    <img src="https://github.com/user-attachments/assets/65303d11-0c9e-4093-8c22-fa4582861c7b" alt="image" width="400" height="400">
</div>


## Introduction
<details>
   <summary><strong>📌 Overview (click)</strong></summary>

 ### **Overview**  
> This Power BI project provides a detailed analysis of **MaxAB** performance, covering **KPIs Performance**, **Shipping**, and **Customers needs**.  
> The analysis aims to uncover **insights** across various **properties and cities**, offering **data-driven recommendations** to **enhance Customer Retention** and **improve overall operational efficiency**.  

</details>


<details>
   <summary><strong>📂 Data Sources (click)</strong></summary>

### **Data Sources**  
> The primary dataset used for this analysis is the **"fact_order_lines.csv"** file containing detailed information about each Order made by the customers.  

**▼ 📑Dataset Files Explanation** [[Download]](https://raw.githubusercontent.com/ibrahim-saiied/Hotel-Hospitality-Analysis_Power-Bi/refs/heads/main/Data%20Set/Data%20Set.rar)  


1. **Dim_date File**  
   > - **<ins>date</ins>**: Represents the dates present in **Mar, Apr, May, June, July and Aug**.  

2. **dim_customers File**  
   > - **<ins>customer_id</ins>**: Unique ID for each **customer in each city**.  
   > - **<ins>customer_name</ins>**: Name of each **customer**.  
   > - **<ins>city</ins>**: The **location** of the **customer**.  

3. **dim_products File**
   > - **<ins>product_name</ins>**: Name of each **product**.  
   > - **<ins>product_id</ins>**: Unique ID for each **product**.  
   > - **<ins>category</ins>**: Indicates to which **category** (**Dairy**, **Food**, **Beverages**) the **product type** belongs.  

5. **fact_orders_aggregate File**  
   > - **<ins>order_id</ins>**: Unique ID for each **order**.
   > - **<ins>customer_id</ins>**: Unique ID for each **customer**.
   > - **<ins>order_placement_date</ins>**: Date of **date of request the order** by the **customer**.  
   > - **<ins>On Time (OT)</ins>**: **1** = Delivered on time, **0** = Not delivered on time.
   > - **<ins>In Full (IF)</ins>**: **1** = Delivered in full, **0** = Not delivered in full.
   > - **<ins>On Time & In Full (OTIF)</ins>**: **1** = Delivered on time & in full, **0** = Not meeting both conditions.


6. **dim_targets_orders File**  
   > - **<ins>customer_id</ins>**: Unique ID for each **customer**.
   > - **<ins>On-Time Target (%)</ins>**: Expected on-time delivery rate per customer.
   > - **<ins>In-Full Target (%)</ins>**: Expected full-quantity delivery rate per customer.
   > - **<ins>OTIF Target (%)</ins>**: Expected on-time and in-full delivery rate per customer.

7. **Fact_bookings File**  
   > - **<ins>order_id</ins>**: Unique **Order ID** for each **customer**.
   > - **<ins>order_placement_date</ins>**: Date of **date of request the order** by the **customer**.  
   > - **<ins>customer_id</ins>**: Unique ID for each **customer**.
   > - **<ins>product_id</ins>**: Unique ID for each **product**.
   > - **<ins>order_qty</ins>**: the number of products requested by the **customer** to be delivered.
   > - **<ins>agreed_delivery_date</ins>**: the date **agreed** to deliver the products.
   > - **<ins>actual_delivery_date</ins>**: the **actual** date delivered the product to the customer.
   > - **<ins>delivered_qty</ins>**: the number of products that are actually delivered to the customer.
   
</details>

<!-- ------------------------------------------------------------------------------------------- -->

## Case Study
**MaxAB** is a growing **FMCG** manufacturer in **Alx, Egypt**.
It operates in three cities (Alex, Suez, Damietta) and plans to expand to Tier 1 cities within two years.
However, some key customers have not renewed their contracts due to service issues, likely caused by late or incomplete deliveries.
Management wants to solve this problem before expanding and has asked to track service levels for all customers.

## Main 𝐊𝐏𝐈𝐬
- **<ins>OT %</ins>**: On time delivery percentage
- **<ins>IF %</ins>**: In Full delivery percentage
- **<ins>OTIF %</ins>**: On time and In Full delivery percentage

## Process
1) Explore, understand and validating all data.
2) Importing and clean data and Adding some columns to aid in data analysis, such as a column to identify the day type weekend or weekday with power query. 
3) Data modeling
4) Creating Measures using DAX
5) Creating the Dashboard

## Measures
;
<img src="https://github.com/user-attachments/assets/8e63c714-c090-40d7-b143-ff4ab9fd8274" alt="image" width="175" height="320" style="display: block; margin: 0;">

## Data Model
![image](https://github.com/user-attachments/assets/968911ef-421b-477a-b89f-9c8e0477378f)

## Dashboard
<img width="1500" alt="Group 3" src="https://github.com/user-attachments/assets/c341a5fc-7298-4893-833c-f795d340a8a4" />
<img width="1500" alt="Group 3" src="https://github.com/user-attachments/assets/fc42b045-a0bb-42bc-8d79-25ecba9a4f11" />
<img width="1500" alt="Group 3" src="https://github.com/user-attachments/assets/705fdf2d-0f69-44b3-acf7-200de479fc7c" />

## Important Insights
1) **Service Level Performance**
   - The average OT%, IF%, and OTIF% are noticeably lower than the targeted levels. This indicates a significant gap between actual performance and goals.
   - Each customer's values fall significantly short of the targets, indicating that not a single customer has met the desired service levels.
 2) **Overall Trend**
    - Average performance by both month and city consistently remains low, suggesting a significant and widespread issue in achieving the set targets.
 3) **Product Shortages**
    - Dairy products account for 78.7% of the total shortfall, with milk (across all size variations) being The most affected.
    - There is a need to focus more on dairy production and offer a wider variety of sizes to suit customer needs.
 4) **Delivery Performance**
    - Only 59.1% of orders were delivered on time or early, while 40.9% faced delays.
    - These key customers experience the highest rate of quantity shortages, increasing the risk of losing them.
5) **Key Customer Risks**
   - Out of 15 customers, the top 6 (Lotus Mart, Acclaimed Stores, Red Stores, Rel Fresh, Cool Blue, and Propel Mart) constitute 53% of total orders, making them key customers.
   - These key customers experience the highest rate of quantity shortages, increasing the risk of losing them.
   - Specifically, Lotus Mart, Acclaimed Stores, and Cool Blue show noticeably lower OT%, OTIF%, and even IF% levels, suggesting they are unlikely to renew their contracts unless improvements are made.
  
## Potential Loss of Key Customers
probably **Acclaimed Stores**, **Cool Blue** & **Lotus Mart** are the Key customers who would certainly not willing to renew the contract

## Recommendation
Focus on improving service levels and delivery performance, particularly for dairy products and key customers, to close the gap with targets and mitigate the risk of contract non-renewals.
