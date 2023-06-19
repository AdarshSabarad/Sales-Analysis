# Sales-Analysis

The Python code is meant to analyze sales data. It imports necessary libraries, merges multiple CSV files into a single file, cleans up the data, adds additional columns, and performs various calculations and visualizations to analyze the sales data. Here's a breakdown of what the code does:

1. Imports the necessary libraries, including pandas and os.
2. Merges multiple CSV files into a single file using the `glob` module.
3. Reads the merged CSV file into a DataFrame called `all_data`.
4. Drops rows with missing values (NaN) from the DataFrame.
5. Removes rows where the "Order Date" column starts with "Or".
6. Converts the "Quantity Ordered" and "Price Each" columns to numeric data types.
7. Adds a "Month" column extracted from the "Order Date" column.
8. Adds a "Sales" column calculated by multiplying "Quantity Ordered" and "Price Each".
9. Calculates the total sales for each month and plots a bar chart showing the month-wise sales.
10. Extracts the city from the "Purchase Address" column and adds a "city" column to the DataFrame.
11. Calculates the total sales for each city and plots a bar chart showing the city-wise sales.
12. Converts the "Order Date" column to datetime data type.
13. Extracts the hour and minute from the "Order Date" column and adds "Hour" and "Minute" columns to the DataFrame.
14. Plots a line chart showing the number of orders received at each hour of the day.
15. Identifies products that are often sold together by grouping rows with the same "Order ID" and concatenating the corresponding products into a "Grouped" column.

Overall, the code performs various data cleaning, transformation, and analysis tasks to gain insights into sales data.
