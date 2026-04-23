# DAX in Power BI

## 🧾 Overview
To create measures and Calculated columns. Use COUNT , SUM , SUMX , WEEKDAY and IF DAX functions.

## 🛠️ Tools & Technologies
  - Power BI Desktop

## 📂 Dataset
  - Source - DAX in Power BI
  - Format - Excel
  - Includes - Apocalypse Store , Apocalypse Sales

## 🚀 How to Use
1. Download the 'DAX in Power BI.xlsx' file.
2. DAX mean Data Analysis Expressions.
3. It is a library to build formulas.
4. We can use to create measures and calculated columns.
5. In 'DAX in Power BI.xlsx' file we have two tables 'Apocalypse Store' and Apocalypse Sales'.
6. If we view the relationship of the tables in Power BI Desktop in the Model view we can observe that they are linked with the 'Product_Id' column.
7. If we look into the table data we can understand that 'Apocalypse Sales' is having the data like what a customer purchased , the product_id , order_id , the date he purchased , and the no. of units sold.
8. And in 'Apocalypse Store' table we are having the product details like the product_id , product_name , how much is the production_cost and at what price it is listed.
9. Now to calculate how many orders they sold we can count by a DAX function.
10. Click right click on Apocalypse Sales from right side Data pane and select 'New Measure'.
11. We can name it as 'Count of Sales = COUNT('Apocalypse_Sales'[ Order Id])'.
12. To visualize we can select Table from Visualizations.
13. The no of orders they sold are '74'.
14. To have the no. of order per customer need to visualize with columns in Visualizations in the right hand side pane.
15. To calcuate and count how many units sold per order.
16. Select Product Name from 'Apocalypse Store' table.
17. To Sum the no.of units sold.
18. Select New measure in Apocalypse Sales table.
19. Sum of Products = SUM('Apocalypse Sales'[Units Sold]).
20. Now a new chart is created with the product name and the no.of units sold per product.
21. And the Total would be 3001.
22. To calculate Profit.
23. Select New Measure in Apocalypse Store.
24. Profit = (SUM('Apocalypse Store'[Price]) - SUM('Apocalypse Store'[Production Cost])) * SUM('Apocalypse Sales'[Units Sold]).
25. Select Table from Visualizations.
26. Now to see the SUM and SUMX difference select Table view.
27. Go to 'Home'.
28. Select 'New Column'.
29. Name it as Profit_column and paste the same formula.
30. We can see that the new Profit_Column is having the same value in all rows.
31. To calculate profit of each customer we need individual iteration so we need to use SUMX.
32. Select New Column from Home.
33. Profit_Column_SUMx = SUMx('Apocalypse Sales' , ('Apocalypse Store'[Price] - 'Apocalypse Store'[Production Cost]) * 'Apocalypse Sales'[Units Sold]).
34. Now we can view Profit gained respectively per Customer.
35. In 'Apocalypse Sales' table we have a 'Date_Purchased' column , to view the data of the column along with the weekday need to change format of the column in column tools section.
36. To view in which number the day of the week is, ex: Sunday is 1 and Saturday is 7.
37. Select Create New Column , name it Day of Week = Weekday('Apocalypse Sales'[Date_Purchased'],2).
38. To view the difference between 'Date_Purchased' and 'Day of Week'.
39. Go to Report view.
40. Select 'Date Purchased' and 'Units sold' select column chart, and we can view that it is not generated properly to calculate.
41. Select 'Day of Week' and 'Units sold' select column chart , 'Day of Week' as X-axis.
42. Enable Data lables in Visualizations section.
43. Now we can properly view in which day of the week we sold the highest and the lowest.
44. Now to check as per the 'Units Sold' whether it is a big order or small order use 'IF' function.
45. Select 'Create New Column' , name it 'Order Size'.
46. Order Size = IF('Apocalypse Sales'[Units Sold]>25 , "Big Order" , "Small Order").

## 📷 Dashboard Preview

<img width="1920" height="1013" alt="Screenshot (50)" src="https://github.com/user-attachments/assets/2657999d-ee13-4ed7-85d7-935e484ea799" />

