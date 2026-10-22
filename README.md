# E-Commerce Sales Analysis using Power BI

## Project Overview

This project focuses on analyzing e-commerce sales data using Microsoft Power BI. The main goal is to clean and transform the data, combine multiple datasets, create relationships between tables, and prepare the data for sales analysis.

The project covers the complete data preparation process, from importing CSV files to organizing the data for meaningful business insights.

## Tools Used

- Microsoft Power BI
- Power Query Editor
- CSV datasets

## Datasets

The project uses three datasets:

- **List of Orders.csv** – Contains order information such as Order ID, Order Date, Customer Name, State, and City.
- **Order Details.csv** – Contains sales details, including Category, Sub-Category, Amount, Profit, and Quantity.
- **Sales target.csv** – Contains monthly sales targets for different categories.

## Data Cleaning and Transformation

The following steps were performed using Power Query Editor:

- Imported all three CSV files into Power BI.
- Restricted the List of Orders table to the first 500 rows.
- Changed the Order Date column to the Date data type.
- Converted the Amount and Target columns to Fixed Decimal Number.
- Applied proper case formatting to customer names for consistent capitalization.
- Combined the City and State columns into a new Location column in the format `City, State`.
- Created a Profit Margin column by dividing Profit by Amount and formatting the result as a percentage.
- Added a Profit Status column to classify each record as Loss, Break-Even, or Profit based on its profit value.

## Data Merging

Merged the List of Orders and Order Details tables using Order ID as the common column to create a combined table named **Orders Data**.

This made it easier to analyze order information alongside sales, category, and profit details.

## Handling Missing Values and Duplicates

Checked the datasets for missing values and duplicate records. Missing values were reviewed to determine the appropriate treatment, while duplicate records were evaluated before removal to avoid affecting valid order details.

## Sorting and Filtering

Applied sorting and filtering to explore the data from different perspectives.

- Sorted orders by Order Date in descending order to focus on recent orders.
- Filtered orders by State, including Tamil Nadu, for regional analysis.
- Used Category and other relevant columns to examine specific segments of the sales data.

## Grouping and Aggregation

Created duplicate tables to perform additional calculations and summarize the data.

- Counted orders using Order ID.
- Calculated average profit by Category.
- Calculated total sales Amount by Sub-Category.
- Aggregated sales targets by month to support comparisons between sales performance and targets.

## Data Modeling

Created relationships between the tables in Power BI using the Manage Relationships feature.

- **List of Orders and Order Details:** Connected using Order ID.
- **Order Details and Sales Target:** Connected using Category.

Checked that the relationships were active and reviewed the data model to support analysis across the datasets.

## Key Learning Outcomes

Through this project, I gained practical experience in:

- Importing and transforming data using Power Query.
- Cleaning datasets and handling missing or duplicate records.
- Creating custom and conditional columns.
- Merging datasets using common keys.
- Grouping and aggregating sales data.
- Establishing relationships between tables in Power BI.
- Preparing data for business analysis and reporting.

## Conclusion

This project demonstrates the process of preparing e-commerce sales data for analysis using Power BI. By cleaning, transforming, merging, and modeling the datasets, the data becomes more organized and useful for exploring sales trends, profitability, regional performance, and progress toward sales targets.

