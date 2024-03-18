# ATLIQ MART DIWALI AND SANKRANTI CAMPAIGN ANALYSIS 

### Problem Statement:

**AtliQ Mart** is a retail giant with over 50 supermarkets in the southern region of India. All their 50 stores ran a massive promotion during the Diwali 2023 and Sankranti 2024 (festive time in India) on their AtliQ branded products. Now the sales director wants to understand which promotions did well and which did not so that they can make informed decisions for their next promotional period. 

Sales director Bruce Haryali wanted this immediately but the analytics manager Tony is engaged on another critical project. Tony decided to give this work to Peter Pandey who is the curious data analyst of AtliQ Mart. Since these insights will be directly reported to the sales director, Tony also provided some notes to Peter to support his work.

### About the dataset:

The data i.e. provided to us, is for different sales event happened during the two Campaigns ran by the mart in Diwali and Sankranti season. We are provided with fact_table which contains **`event_id,store_id,product_code, the base price of the product before any promotion, quantity sold immediately preceding the start of the campaign (serving as a baseline for comparison with promotional sales), the quantity of the product sold after the promotion was applied and promo type`** which was applied in campaign for that product (e.g. percentage discount, BOGOF(Buy One Get One Free), cashback). There are other various dimensions table provided for the information about the products, stores and campaigns which can be joined two the fact table using various ids provided in the same.

### Analysis:  

There are several columns which can be derivated from the information provided to us: <br>
**1. Total revenue per event before the promo start <br>
 2. Total revenue per event after the promo start <br>
 3. Difference in these revenue (Increamental revenue per event id) <br>
 4. Percentage change (Incremental revenue per event id / Total revenue per event before the promo start) <br>
 5. Difference of quantity sold before and after the promo (Increamental units sold per event id \[ISU])**

These columns were used to review the impact of the campaigns on the revenue and sales so that stakeholders can easily identify and take action in the region of improvements based on these insights. 

### Dashboard:

![Dashboard](/Atliq_mart_problem/d_final.png)

### Insights:

1. Diwali campaign was observed to be more impactful as it saw 94% increamental overall revnue as compared to Sankranti(54%)
2. Tier 1 city stores (like Bengaluru, Chennai, Hyderabad) saw most gains in revenue during the promo season as compared to other cities.
3. 94% of Incremental Revenue generated during the diwali season was observed from the `500 cashback` on `Home_essential_Combo_of_8_products`
4. The impact from 50% discount promo on `Personal Care` items was negative for both the Campaigns.
5. Among the tier 2 cities the average incremental revnue per store from the Madurai and Mysore Stores are quite high. This needs to be futher investigated if the stakeholders are looking for business expansion in these cities. 
6. Performance based on incremental revenue was lowest for the stores in Trivendrum and Mangalore
7. `500 Cashback` and `BOGOF` are top 2 promotion types whereas `33% off`, `25% off` are bottom 2 promotion types (for the products on which these were applied)
8. The ISU% increase during the Sankarnti Campaign are very high compared to the Diwali Campaigns which is reverse in case of Increamental Revenue, indicating that people bought cheaper products in Sankranti compared to Diwali



