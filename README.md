# E-Commerce-Analysis-with-PowerBI
Identified insights in the ecommerce datasets with "What-If Analysis", and "Up-Sell and Cross-Sell Strategies", data modeling to EDA, DAX functions, and report design.

<br/><br/>

## Business Goals of the Supply Company:
The online supply company has several key goals:
1. **Uncover insights**: The company aims to gain a deeper understanding of its overall performance and identify improvement opportunities.
2. **Increase their Sales and Customers**:
      - **Upsell Opportunities**: By promoting relevant products during the purchase process, such as offering beach chairs when a customer buys a beach umbrella.
      - **Cross-Sell Opportunities**: Encouraging customers to consider higher-priced alternatives or larger quantities of products, like presenting an offer on organic pet food for regular pet food buyers.
3. **Reduce Operating Expenses**:
    - **Shipping Cost Reductions**:
      - Consolidate multiple shipments into a single one.
      - Optimize package size dimensions and weight to minimize shipping costs.
   
<br/><br/>

## Dashboard Pages:
### ***1st page***: **"Executive summary"**: 
#### Overview:  
At the top, you’ll find a filter for the company’s product description, and 4 important kpis to keep track and monitor the overall performance
  1. Key Performance Indicators (KPIs) displayed:
      - Total Sales
      - Total Profit
      - Profit Margin
      - Shipping Baseline
  2. there are 4 charts:  
      - **map chart** for *Total Sales by State*: This chart reveals our top customer locations.
      - **Clustered Bar chart**, for showing the average customers Life time value (LTV) by state.
        > `The higher the customer’s life time value, the more important the customer is to the company`    
      - a **tree chart** for the *profit % and total sales by category*
      - a **stacked bar chart** for *total sales by description and category*    
When we click on a category in the tree chart, it filters the stacked bar chart. by providing a drill-down view showing the total sales for products by category and sorting them in a descending order. 
<br/><br/>
        > These will benefit us for providing a deeper analysis and insights as well as making a better business decision making,
        > - **Electronics** is the category with the most total sales and profit, with only 2 products.  
        > - Obviously, **California** stands out as the state with the highest sales and customer base.

https://github.com/salmaH4/E-Commerce-Analysis-with-PowerBI/assets/110805003/6005edb1-b189-4b1c-9d24-fae56986912a

<br/><br/>

### ***2nd page***: **Shipping Metrics**
I used **"What-If Analysis"** and **Cross-Sell** dashboard-style page to, 
- present the impact of shipping higher product quantities on sales.
- its effect on the company's profitability.   

At the top, I added:
  1. a **slicer**, to adjust the inputs of what-if shipping quantity and see different outcomes
  2. **3 dynamic metrics**,   
     ` the shipping department told us that shipping more than 1 quantity costs them on average, 70% of the cost of a single unit shipment `
     - ***shipping (Baseline)***, this sums the costs of shipping items iteratively
       | shipment quantity | discount |
       | ------------------------- | -------- |
       | 1 item | 0% |
       | + 1 item | 70% |
       
     - ***shipping (what-If)***, this will calculates the discounted shipping costs based on the following 
       | what-if shipment quantity | discounted shipping cost |
       | ------------------------- | -------- |
       | <= 1 | 100% |
       | <= 2 | 80 % |
       | <= 4 | 60 % |
       | <= 7 | 50 % |
       | <= 9 | 40 % |
       | > 9 | 30 % |
       
     - ***shipping (difference)***, this calculates the shipping cost savings.   
<br/><br/>

  To clearly analyze the impact of shipping quantity and how it effects the company's profits, I used the following charts:
  1. **Line and Clustered column Chart**, this compares the 3 shipping metrics created by each product.
  
       > we can clearly see that when the shippment quantity product is 1 the company will lose `$ 88643`, but as the shippment quantity increases the company's profitability increases as well.
  2. **Area Chart**, to track the shipping savings by transactions date, and showing different possibiltes of running totals what-if scenarios.
  3. **Clustered Column Chart**, showing the average quantity of products being purchased by Category
  4. **Map Chart**, this chart helps Region Managers to focus on How shipping costs impacts the profit grand total through each state in their region.
     
<br/><br/>

https://github.com/salmaH4/E-Commerce-Analysis-with-PowerBI/assets/110805003/c9695ba4-0c59-4529-8978-c2e366b4294f

<br/><br/>

### ***3rd page***: **Market Basket Analysis**:
In this page, I provided the following visuals:
- a **table** that lists each product's description
- a **Line and Stacked Column Chart**, for analyzing the total sales, and profit % for each product.
- a **Clustered Bar Chart**, for the top Purchased Items.
    
    > - This will filter products for a specific products
    > - provides Recommendations for which products should be displayed to customers by attracting their attention to alternative related products. So, with this Up-Sell strategies the profitability and the total sales will increase.

https://github.com/salmaH4/E-Commerce-Analysis-with-PowerBI/assets/110805003/6c42e423-25a3-40a2-8bba-5814fe2b7fef

<br/><br/>





