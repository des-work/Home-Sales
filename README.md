# Home Sales Analysis with PySpark

## Overview
This assignment uses PySpark to conduct a comprehensive analysis of home sales data, addressing specific questions through SparkSQL queries. The tasks encompass computing average prices for distinct conditions, caching data for optimization, and comparing query runtimes.

## Instructions
1. **File Renaming and Initialization:**
   - Rename the `Home_Sales_starter_code.ipynb` file to `Home_Sales.ipynb`.
   - Import the necessary PySpark SQL functions for the assignment.

2. **Data Loading and Temporary Table:**
   - Read the `home_sales_revised.csv` data into a Spark DataFrame.
   - Create a temporary table named `home_sales` to facilitate further analysis.

3. **Answering Questions with SparkSQL:**
   - Leverage SparkSQL to address the following questions:
      - What is the average price for a four-bedroom house sold for each year? (Rounded to two decimal places)
      - What is the average price of a home for each year it was built with three bedrooms and three bathrooms? (Rounded to two decimal places)
      - What is the average price of a home for each year with three bedrooms, three bathrooms, two floors, and is greater than or equal to 2,000 square feet? (Rounded to two decimal places)
      - What is the "view" rating for homes costing more than or equal to $350,000? Determine the runtime for this query. (Rounded to two decimal places)

4. **Data Caching:**
   - Cache the `home_sales` temporary table for enhanced performance.
   - Confirm if the table is successfully cached.

5. **Cached and Uncached Query Runtimes:**
   - Utilizing the cached data, execute a query filtering out view ratings with an average price greater than or equal to $350,000. Ascertain the runtime and compare it to the uncached runtime.

6. **Parquet Data Analysis:**
   - Partition the formatted parquet home sales data based on the "date_built" field.
   - Establish a temporary table for the parquet data.
   - Run a query filtering out view ratings with an average price greater than or equal to $350,000. Ascertain the runtime and compare it to the uncached runtime.

7. **Uncaching and Verification:**
   - Uncache the `home_sales` temporary table.
   - Verify that the table is no longer cached using PySpark.

8. **GitHub Submission:**
   - Download the completed `Home_Sales.ipynb` file.
   - Upload it to your "Home_Sales" GitHub repository.

For any queries or assistance, feel free to reach out. Best of luck!
