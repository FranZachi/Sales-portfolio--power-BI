# Sales-portfolio--power-BI
Sales dashboard- Portfolio- Power BI

Dashboard link: https://app.powerbi.com/groups/me/reports/d3ed328b-23b2-4321-9412-9bffadcbaa09/be06d85a0c19752d2d3c?experience=power-bi


1)	Introduction:

Data analysis has become a fundamental retail component, providing a clear and comprehensive overview of sales performance in real time. This approach allows managers to quickly identify trends, analyse consumer behaviour, and monitor key performance indicators (KPIs), such as total sales and average transaction value across others.
With such insights readily available, businesses can make more informed and agile decisions, adjust marketing strategies, optimise inventory, and enhance the overall customer experience. In today’s competitive market, the ability to respond quickly to accurate data is crucial for success
This project seeks to apply and demonstrate my expertise using the Power BI tool. For this purpose, I have utilised a sales database sourced from the Kaggle website. It is important to note that this database is not based on real-time data or actual business operations but serves solely for educational purposes. The dataset includes four product categories: food, clothing, furniture, and electronics, and the analysis will focus on examining sales trends and customer behaviour within these sectors.

2)	Methodology
   
The dataset contains information that simulates sales transactions across different products, regions, and customers. Each row represents an individual sales event with various associated details. The table consists of fourteen columns:

1)	Product_ID: Unique identifier for each product sold. Randomly generated for practice purposes.
2)	Sale_Date: The date when the sale occurred. Randomly selected from the year 2023.
3)	Sales_Rep: The sales representative responsible for the transaction. The dataset includes five random sales representatives (Alice, Bob, Charlie, David, Eve).
4)	Region: The region where the sale took place. The possible regions are North, South, East, and West.
5)	Sales_Amount: The total sales amount for the transaction, including discounts if any. Values range from 100 to 10,000 (in currency units).
6)	Quantity_Sold: The number of units sold in that transaction, randomly generated between 1 and 50.
7)	Product_Category: The category of the product sold. Categories include Electronics, Furniture, Clothing, and Food.
8)	Unit_Cost: The cost per unit of the product sold, randomly generated between 50 and 5000 currency units.
9)	Unit_Price: The selling price per unit of the product, calculated to be higher than the unit cost.
10)	 Customer_Type: Indicates whether the customer is a New or Returning customer.
11)	 Discount: The discount applied to the sale, randomly chosen between 0% and 30%.
12)	 Payment_Method: The method of payment used by the customer (e.g., Credit Card, Cash, Bank Transfer).
13)	 Sales_Channel: The channel through which the sale occurred. Either Online or Retail.
14)	 Region_and_Sales_Rep: A combined column that pairs the region and sales representative for easier tracking.
I used Power BI as the tool to explore this project. I applied DAX measures to tackle the challenge of creating an interactive dashboard that offers insights for decision-making and provides a consolidated view of the company’s key metrics and performance indicators (KPIs).

3)	Project Steps:

3.1) Verification and Data Collection: The database is in Excel. First, it was necessary to verify if the table had various information, such as sales data: customers, products, transactions, regions, etc.

3.2) Importing and Loading Data: The file was in the format excel.csv with 106KB size. 
This database was imported into Power BI. After loading it, I checked the table in Power Query to see if it needed cleaning or adjustments.
After analysing the fourteen columns, I found that the date column contained insufficient information. Therefore, it was necessary to create a new column for date-based analysis.

3.3) Creation of a Date Column: Using DAX Measures methodology, I accessed Power Query, created a new column, and named it 'calendar_date.' The table has the following columns: Month, Month Name, and Year (2023 and 2024).


![image](https://github.com/user-attachments/assets/5110f1db-37d5-4be6-aa1e-b4d83ebcc7e3)
                                   


After completing this step, I accessed the Visualization Model tab and established the relationship between the tables sales_data (Sale_Date) and calendar_date (Date), thus enabling the interaction and manipulation of the information.

![image](https://github.com/user-attachments/assets/43c6a07f-0432-4f35-aee3-29d636e4758f)
                                   

3.4) Creation of DAX Measures: Creating DAX measures. I used cards using the functionalities of the data model and the filter context of each visualisation of the KPIs.

Sales: Analyse the total sales amount using the annual period (2023).


![image](https://github.com/user-attachments/assets/e58ec0f5-1127-4d68-81dc-0e50de74320f)


Cost: Analyse the efficiency of operational costs with sales for the year (2023).


![image](https://github.com/user-attachments/assets/ff38ac3e-6986-4fc6-89e2-994520ea7149)


Profit: Analyse the overall finances of the company considering all expenses.


![image](https://github.com/user-attachments/assets/4126b3fd-d4aa-4fa7-b6f7-af3ec2dc8665)


Margin: Analyse the company's annual sales profitability by deducting direct costs.


![image](https://github.com/user-attachments/assets/098f43a9-75c6-4d1a-86db-6790923ba199)

 
Total Sales: Analyse the total sales volume made in the Year (2023).


![image](https://github.com/user-attachments/assets/acc6ef1c-b2c5-43f2-9bdf-6f70ded72052)


Sales Month over Month (MoM): Analyse the trends in sales growth or decline to help understand seasonality and purchasing patterns.


![image](https://github.com/user-attachments/assets/3db4cf10-017d-4a88-ab8e-5d55ee496791)


Sales MoM Delta: Checking the patterns of variation.


![image](https://github.com/user-attachments/assets/2a8a7948-d6c1-497f-8672-eaea63864477)


Sales MoM Delta %: Percentage verification of the variation: positive or negative.


![image](https://github.com/user-attachments/assets/27916916-bfdd-4636-be58-b99b6d0513d1)


4)	Creation of Dashboards: Created dashboards to provide comparison charts for dynamic and interactive visualisation of analyses. Through these sales analyses, I was able to identify trends, opportunities for improvement and areas for growth.

4.1) Market Regions: The company operates in various regions: North, East, West, and South, and the chart represents sales revenue in these regions.
Analysis Result: The North region showed the highest sales revenue, while the South region had the lowest. The difference in revenue between the East and West regions is 24,184K.

4.2) Sales per Category (%): Evaluate the percentage of sales performance across the categories: Food, Clothing, Electronics, and Furniture.
Analysis Result: The category with the highest percentage of sales is Clothing (26%), while the lowest is Food (24%). Electronics and Furniture, along with the other categories, each account for 25% of total sales.

4.3) Sales: Channels x Type of Customer: Compare the sales performance in the channels: online and retail with the types of customers: new and returning.
Analysis Result: I observed that the "returning" customer profile showed a higher sales performance through the retail channel than online. The difference between the sales channels is 160,587K. On the other hand, the "new" customer profile showed a difference in sales performance through the online channel of 58,989K compared to the retail channel.

4.4) Channel x Category x Customer Type: A comparison chart regarding payment methods (bank transfer, cash, and credit card), sales channels (online and retail), and their categories (clothing, electronics, food, and furniture).

Analysis Result: Customer behaviour patterns, such as new versus returning customers, were analysed with purchase channels (online vs. retail) and payment methods (bank transfer, cash, and credit card).
In the online channel, the food sector demonstrated the strongest sales performance, while the clothing sector led in retail sales. Both channels saw bank transfers as the predominant payment method. Conversely, the furniture sector recorded the lowest sales performance across both channels.
Regarding cash payments, the furniture category performed best in online sales, while the food sector showed the weakest performance. In the retail channel, the food sector achieved the highest sales, whereas electronics recorded the lowest performance in this channel.
Lastly, for credit card payments in online stores, the electronics sector generated the highest revenue, while the clothing sector excelled in retail sales. Notably, the food sector experienced a decline in sales when comparing online and retail channels for credit card payments.

4.5) Monthly Sales: Chart representing the total sales value conducted annually (2023), the sales value for the current month, and the previous month, along with the profit.
Analysis Result: Regarding the chart of monthly sales evolution, we can observe that July 2023 experienced the lowest sales performance compared to other months.
By examining the tooltip details or clicking directly on the 'Date Month' legend (July), we can see a sales decline of -44K compared to June. Additionally, profit performance was lower, with a total of 17K.
This resulted in total sales of 1.60K, marking July as the month with the weakest performance of the year.


5) Creation of Tooltips: The tooltip feature allows for detailing and contextualising the information in the charts.

5.1) TTP 01: Inserted three cards (Sales, Sales MoM Delta, and Cost).

Sales: Sales values.
Sales MoM Delta: This card shows the absolute difference in sales between the current month and the previous month.
I classified the colours as follows:
Green: When the "Sales MoM Delta" value is positive (i.e., increase in sales).
Red: When the "Sales MoM Delta" value is negative (i.e., sales have decreased). 
Cost: Evaluating costs to gain a deeper understanding of financial performance to sales.
Charts:

Region Chart: Comparison of sales, profit, and cost indices across the four regions (North, East, West, and South).
Sales Monthly: Visualisation of the evolution of monthly sales to the indices of Sales, Sales MoM, Profit, and Cost.

![image](https://github.com/user-attachments/assets/5683f500-c8b1-42e9-acc3-f6d87222a553)

 
5.2) TTP 02: Included the following cards: Sales, Profit, and Cost.
Charts:

Sales: Channel x Customer Type: Comparisons of customer behaviour with sales channels (retail/online) with customer types (new/returning).
Sales per Category: Visualise performance about the indices of sales, profit, and cost across the four categories (clothing, electronics, food, and furniture)

![image](https://github.com/user-attachments/assets/6ff7f6fa-4c88-46fd-ba68-0918446e1c84)


6)	Conclusion 
In this project, I explored the sales area using Power BI, which allowed me to generate valuable insights and contribute to strategic decision-making. The interactive dashboards and dynamic visualisations (Menu: Month and Tooltips) facilitated understanding key performance indicators, providing a solid foundation for informed decisions and effective actions.
