# Week 22 Challenge - Home Sales 

This project uses SparkSQL to determine key metrics about home sales data and utilizes Spark to create temporary views, partition the data, cache and uncache a temporary table, and verify that the table has been uncached.

The following files are included:
* Home_sales.ipynb

Code will generate the following:
* Folder titled home_sales_partitioned
* Folders for homes built between 2010-2017

## Code Overview:
The code creates a Spark DataFrame, a temporary table of the original DataFrame, query returning the average price, rounded to two decimal places, for a four-bedroom house that was sold in each year
A query returning the average price, rounded to two decimal places, of a home that has three bedrooms and three bathrooms. 
A query returning the average price of a home with three bedrooms, three bathrooms, two floors, and is greater than or equal to 2,000 square feet for each year built rounded to two decimal places. 
A query returning the view rating for the average price for homes that are greater than or equal to $350,000, rounded to two decimal places, and outputs the run time for this query.
In addition, the code creates a cache of the temporary "home_sales" table and computes the run time. 
A partition of the home sales dataset by the "date_built" field is created, and the formatted parquet data is read, then creates a temporary table of the parquet data.  The parquet temporary table is queried and the run time is computed. 
Lastly, the "home_sales" temporary table is uncached. 

Resources: Include instructor provided starter code, course materials, Apache Spark documentation, StackOverflow, and Analytics Vidhya.
