# Relationships in Power BI

## 🧾 Overview
- Relationships in between the tables and the visualizations.

## 🛠️ Tools & Technologies
- Power BI

## 📂 Dataset
  - Source - Relationships in Power BI
  - Format - Excel
  - Includes - Apocolypse Store , Apocolypse Sales , Customer Information

## 🚀 How to Use
1. Download the 'Relationships in Power BI.xlsx' file.
2. Select all the three sheets and Load in Power BI Desktop.
3. Select 'Model view' from the left hand-side pane.
4. We can see three tables of Customer Information , Apocolypse Sales and Apocolypse Store.
5. Double click on the relation between Customer Information and Apocolypse Sales.
6. As Customer column can have duplicate values , select Customer Id in From and To tables and click 'Save'.
7. Select Cross-filter direction as 'Both'.
8. Select 'Report View' from the left hand-side pane.
9. Select 'Table' from the Visualizations.
10. Select State from Customer Information table.
11. Select 'New Measure' from Home section.
12. Measure = count('Apocolypse Store [Product Id]').
13. Select the Measure from 'Apocolypse Store' table from Data section.
14. In the Model view Make the Cross-filter direction as Both for both the relations to get the accurate data.

- So we understood the relationships in between the tables and the visualizations.

## 📷 Dashboard Preview

<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/fec64f65-dda1-40cd-aa08-36ab066dc6ca" />


<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/eb3bee38-43d6-4997-a158-e4b22d8b0b76" />



