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

