![superstore](supertore.jpg)
# Executive Sales Report
## Author : Millicent Ofobuike
### Data Date: 01-01-2020 – 31-05-2020.

## Background of Data
The dataset is a public data made available by Maven Analytics. To improve my knowledge of Microsoft Excel, Excel was chosen for analysis and visualization.
The dataset was downloaded and saved. 

The columns and rows were checked to understand the dataset. The workbook has 4 sheets (sales table, sales team, store locations and products). A working database of the dataset was created and this is what was worked on. 

##### Questions we will like to answer:

* What is the total profit made from January to May 2020?
* What is the total quantity sold?
* Who are the top 5 sales teams?
* What is the total profit made by month?
* What are the top 10 stores?
* What day of the week had the highest sales?
* What day of the week had the highest profit?
* What sales channel performed the best?
* What is the average sale by month?
* What product had the highest sales?


The **Sales Table** sheet has 10 columns and 20,001 rows with each row representing a specific order of product including the product type,the quantity sold, the team that sold it and the day it was sold.

The **Sales Team** sheet contains 3 columns and 29 rows representing sales team index and sales team's names. 

The **Products** sheet has 2 columns and 49 rows representing product id and product names. 

The **Store Locations** sheet contains 15 columns and 368 rows representing store Id, store names, county, state, etc
We can see there are structural errors.


![dirty](dirty_data.png)

## Data Cleaning

The highlighted column names were renamed to Sales Team Index, Store Index, Product Index, Order Quantity, Unit Price and Unit Cost for easier understanding.

The data types were checked. Sales Date was changed from General to Short Date.

Order Quantity was changed from General to Number. The Unit Price and Unit cost columns were rounded off to remove decimals.
To verify if there were duplicates, all rows and columns were selected, and the remove duplicates ribbon was clicked on. 

Zero duplicates was found. This means there is no duplicated data.

![duplicates](duplicate_pix.png)

The filter ribbon was used to filter each column, on each column, blank cells and misspelt words were checked for and there was none.  

## Data Analysis

New columns (profit, Day and month) were created. Profit column was created by subtracting column Unit price from column unit cost. 

Day and month were extracted by using the day and month extraction functions **=TEXT(B2,”ddd”)** and **=TEXT(B2,”mmm”)**.

Since the Sales Table contains sales team index, store locations index and product index, the VLOOKUP function was used to get the values from their respective sheets and new columns: Sales Team, Store and product columns were added to the table.

![cleaned](cleaned_data.png)

To insert pivot tables, a table containing all cells was created and the table style was changed to none. To make the table more presentable, the cell heights were adjusted and colors were added to the background.

Pivot tables and dashboard sheets were created.

The result was visualized using Excel. 


![chart](chart1.png)

Saturday had the highest quantity of sales.


![chart](chart2.png)

Online had the highest profit.


![chart](chart3.png)

Saturday had the highest profit.


![chart](chart4.png)

![chart](chart5.png)

May had the highest Monthly profit.

##### Reports

![dashboard](sales_dash.png)

![dashboard](sales_dash2.png)

## Observations
* The total profit made from January to May 2020 is **(USD2,296,410)**
* The total quantity of products sold from January to May 2020 is **(110,402)**
* **(Paul Holmes, Donald Reynolds, Joshua Little, Adam Hernandez, Nicholas Cunningham)** are the top 5 sales team.
* **(Saturday)** had the highest number of sales and highest profit.
* **(Clock)** had the highest quantity sold and highest profit.


