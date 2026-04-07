# Data Cleaning in Power Query

## 🧾 Overview
- Clean the data and transform for visualization.

## 🛠️ Tools & Technologies
  - Power BI Desktop
  - Power Query

## 📂 Dataset
  - Source - Data Cleaning in Power Query
  - Format - Excel
  - Includes - Location , Products , January-22 , February-22 , March-22 , April-22 , Grand Total

## 🚀 How to Use
1. Download the 'Data Cleaning in Power Query.xlsx' file.
2. Open Power BI Desktop.
3. Select Import Data from Excel and select the excel file.
4. Tick Pivot Table and Purchase Overview sheets and click Transform Data.
5. Now it redirects to Power Query for Data cleaning.
6. To visualize and analyse we need proper data , data with null values will not be providing the perfect output.
7. Select Purchase Overview from the left hand-side Query pane.
8. We will be working in this sheet.
9. The top two rows are null , in the Home section select 'Remove rows' , provide the count as 2 to remove the top two rows.
10. Top two rows are now removed.
11. The column headers are inappropriate.
12. In Transform section select 'Use First Row as Headers' option.
13. Now Location , Products , Dates and Grand Total are updated as headers.
14. Even the data types of the columns are updated accordingly.
15. As the Date column values are incosistent , change the data type to standard value.
16. Select the data type option and click on 'Fixed Decimal Number' and click on 'Replace current'.
17. Apply the same to all the Date columns.
18. Now as we see there are few Location specific total rows which are not necessary.
19. To remove select the column header arrow button and click on 'Remove empty'.
20. This removes all the rows which are null or empty in the Location column.
21. Another way to do this is by filtering.
22. In Products column select the arrow button and in 'Text Filters' select 'Does not contain' click 'Insert' and Type 'Total' and click on 'Ok'.
23. This removes all the rows which are having the word 'Total' in the Products column.
24. Now to remove the 'Grand Total' column select column , navigate to the Home section and select 'Remove Columns'.
25. This removed the 'Grand Total' column.
26. To change the data type of the newly created Attribute column click data type and select 'Date'.
27. Change the name of the 'Value' column to 'Product Cost'.
28. Change the name of the 'Location' column to 'Store'.
29. All the applied steps will be visible on the right hand-side pane at 'Applied Steps'.
30. Click on 'Close & Apply' for all the changes to save in Power Query and redirect to Power BI.

- So we made the first row as header and removed the empty rows , changed the data type to fixed Decimal number , Unpivot the Date columns , renamed columns to Store and Product Cost.
- We made the data ready for visualization.

## 📷 Dashboard Preview

<img width="1920" height="1026" alt="Data Cleaning with Power Query" src="https://github.com/user-attachments/assets/c9ef7186-a241-4dbb-911f-e94201c6affc" />

