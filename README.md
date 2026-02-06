# Sales-Operations-and-Analytics
##Data Validation and Cleaning
Applied data validation rules to key columns (OrderID, Order Date, Required Date, Unit Cost, Unit Price, Quantity, and Discount) to prevent incorrect data entry.
Ensured OrderID values were unique except for highlighted duplicates that were intentionally retained.
Checked for inconsistent text entries in Region, Country, City, Channel, and Product Category and standardized spelling and capitalization.
Verified that all dates were in a consistent short-date format across the workbook.
Removed leading and trailing spaces from text fields using TRIM where necessary.
##Handling Missing and Inconsistent Data
Reviewed all blank cells across critical columns and ensured replacements were applied consistently as stated in Step 1.
Cross-checked that no negative values remained in Unit Price or other monetary fields.
Ensured all replaced null values in Discount were clearly reflected in calculations and visuals.
Confirmed that swapped Required Dates (where earlier than Order Dates) were correctly updated.
##Calculations and Derived Fields
###Created a calculated column for Total Sales using:
Total Sales = Quantity × Unit Price × (1 − Discount %).
###Generated a KPI column categorizing performance based on the 25th, 50th, and 75th quartiles:
Below 25th percentile = Low
Between 25th and 75th percentile = Medium
Above 75th percentile = High
##Analysis 
Used PivotTables to categorize total sales by Region, Country, Product Category, and Salesperson.
Analyzed sales trends over time using Order Date as the timeline field.
Identified top-performing and underperforming regions, products, and salespersons based on categorized quartiles.
##Visualization
Created dashboards using charts including:
Sales by Region (Bar Chart)
Sales Trend Over Time (Line Chart)
Sales by Product Category (Donut Chart)
Salesperson Performance (Column Chart)
Ensured charts were clearly labeled with titles, axes, and legends.
