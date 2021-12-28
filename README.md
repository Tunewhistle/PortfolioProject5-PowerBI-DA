# PortfolioProject5-PowerBI-DA
This Power BI project simulates a data analysis process. The flow goes as follows:
1. receive a data analysis request from a customer, 
2. create a business demand overview based on the customer’s request, this overview will be the guideline for data analysts to measure and specify the work
3. extract(find) the right data(dataset/tables) to transform (cleanse)
4. structure the relationships among tables (data modeling)
5. Build a Power BI dashboard
6. Evaluate the finished Power BI dashboard based on acceptance criteria in Business Demand Overview, see whether it fulfills the customer’s requests.
Below are the details of each steps:

## 1. A data analysis request from a customer by email

Hi,
I hope you are doing well. We need to improve our internet sales reports and want to move from static reports to visual dashboards.
Essentially, we want to focus on how much we have sold of what products, to which clients and how it has been over time.
Seeing as each salesperson works on different products and customers, it would be beneficial to be able to filter them also.
We measure our numbers against the budget so I added that in a spreadsheet so we can compare our values against performance.
The budget is for 2021 and we usually look 2 years back in time when we do an analysis of sales.

Let me know if you need anything else!

Best regards,
Jussi
Sales Manager

## 2. Translate the user request into a business demand overview & user stories

Business Demand Overview:
Customer(who made the business request): Jussi- Sales Manager
Value of Change(what value need to be added): Visual dashboard to improve sales reporting and help monitor sales performance
Necessary Systems: Power BI
Other relevant info: Budgets have been delivered in a spreadsheet for 2021

User stories(try to specify from the user point of view what our delivery has to give the user):
|No.|As a (role)|I want (request/demand)|So that I (user value)|Acceptance Criteria|
|---|-----------|-----------------------|----------------------|-------------------|
|1|Sales Manager|A dashboard overview of internet sales|Can follow customers and sales of products better|A Power BI dashboard that updates data regularly |
|2|Sales Manager|A dashboard overview of internet sales|Follow sales overtime against budget|A Power BI dashboard with graphs and KPIs comparing against budget|
|3|Sales Representatives|A detailed overview of internet sales per customer|Can follow up my customers, and see who buys the most and who we can sell more to|A Power BI dashboard that allows me to filter data for each customer|
|4|Sales Representatives|A detailed overview of internet sales per product|Can follow up products that I sell the most|A Power BI dashboard which allows me to filter data for each product|

## 3. Decide what datasets are needed, collect, cleanse and transform data
Thought process:
1. As the user wants to see the sales of products and the difference between sales and budget, sales and budget data are needed.
2. As the user wants to filter the data by customers and products, customer and product data are needed as well.
3. As sales happen over time, a date table is good to have.
4. Data content and its purpose can also be considered at this stage. 

Here are the summary of the data source for data analysis and visualization:

|Table names| |
|-----------|----------|
|Sales|Fact table|
|Budget|Fact table|
|Customers info|Dimension table|
|Products info|Dimension table|
|Calendar|Dimension table|

After the datasets are accquired, they are uploaded to Power BI and cleansed in Power Query for modeling and visualization.

## 4. Data modeling
Structure the relationships, each relationship's cardinality and direction.

![Screenshot of data structure](/Screenshots/screenshot-of-data-structure.PNG)

## 5. Data visualization
Start creating the dashboard with the user requests and stories in mind, select the right visual elements and filters to best serve the purpose. Here are the screenshot of the dashboard. The project file can be found in this repository.

Screenshot of the page-Sales Overview

![Screenshot of page1](/Screenshots/dashboard-page1.PNG)

Screenshot of the page-Customer Details

![Screnshot of page2](/Screenshots/dashboard-page21.PNG)

Screenshot of the page-Product Details

![Screnshot of page3](/Screenshots/dashboard-page3.PNG)



