# Home Sales Data Analysis with SparkSQL

## Purpose

The purpose of this assignment is to analyze key metrics from home sales data using SparkSQL.

## Steps

1. **Loaded Data**  
   Loaded home sales data from an AWS S3 bucket into a PySpark DataFrame.

2. **Created Temporary Table**  
   Created a temporary SQL table (`home_sales`) for querying.

3. **Analyzed Data Using SparkSQL**  
   Answered the following questions:
   - What is the average price of 4-bedroom homes sold per year?
   - What is the average price of 3-bedroom, 3-bathroom homes by year built?
   - What is the average price of 3-bedroom, 3-bathroom, 2-floor homes with at least 2,000 sq ft by year built?
   - What is the average home price for each view rating, considering only homes priced at $350,000 or above?

4. **Caching for Performance**  
   Cached the temporary table and compared query runtimes before and after caching to evaluate performance gains.

5. **Data Partitioning**  
   Partitioned the data by `date_built` and saved it in Parquet format to enhance query efficiency.

6. **Performance Comparison with Partitioned Data**  
   Created a temporary view from the partitioned data and re-executed queries to compare performance.

7. **Uncached Table Verification**  
   Uncached the temporary table and verified the uncaching using PySpark methods.
