# Sales-Operations-and-Analytics
This project involves cleaning, transforming, and analyzing a sales dataset in Excel. 
The goal was to improve data quality, create meaningful insights, and build dashboards 
for decision-making.

The dataset contains sales records including OrderID, Region, Country, City, Product Category, 
Salesperson, Unit Cost, Unit Price, Discount, Quantity, Order Date, and Required Date.

- Highlighted duplicate values (kept them, did not remove).
- Formatted:
  - Order Date and Required Date to short date
  - Unit Cost and Unit Price to currency
  - Discount to percentage
  - Quantity to numbers
- Replaced blank values:
  - City → "Not Provided"
  - Salesperson → "Unknown"
  - Channel → "Not Provided"
- Replaced negative Unit Price values with blanks.
- Replaced 7 discount values above 30% with null.
- Used an IF formula to swap Required Dates that were earlier than Order Dates.
- Calculated 25th, 50th, and 75th percentiles and categorized performance as Low, Medium, High.

- Created a Total Sales column: Quantity × Unit Price × (1 − Discount %).
- Built PivotTables to summarize sales by Region, Product Category, and Salesperson.
- Analyzed trends over time using Order Date.

Dashboards includes:
- Sales by Region (Bar Chart)
- Sales Trend Over Time (Line Chart)
- Sales by Product Category (Donut Chart)
- Salesperson Performance (Column Chart)

## Documentation & Outputs 
**Files in this repository:** - `Excel_Assignment_and_Brief_worked.xlsx`
– Original workbook - `staging Data` – Cleaned dataset
- Dashboard sheet – Inside the Excel workbook
- PivotTables summary sheets – Inside the Excel workbook

- ## Tools Used
- Microsoft Excel
- Power Query
- PivotTables
- Excel formulas
