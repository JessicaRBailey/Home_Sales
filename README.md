# Home_Sales
Challenge 22

Please see code in Home_Sales_colab.ipynb.

In this project we use google colab, python, spark, and parquet to analyze a dataset of home sales.  The dataset contains columns such as the year the house was built, how many bedrooms, bathrooms, and floors it has, its price and rating by potential buyers, among a few more columns.  This allows us to write sql queries using spark to find information such as the average price of a 4 bedroom home.  

After filtering the dataset to answer a few questions, we use one query, for the average rating of homes priced at or above $350,000 to test several big data methods.  Our first method of using only spark and a temporary view takes 0.66 seconds.  Our next method, using a cached table, takes a reduced time of 0.59 seconds.  Finally, we use parquet to partition the table by the date_built column and we see our lowest runtime of 0.43 seconds.  
