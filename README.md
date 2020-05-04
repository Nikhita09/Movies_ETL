# Movies_ETL

ETL stands for E - Extract, T - Transform, L - Load. 

## Project Overview:

We will write a Python script that performs all three ETL steps on the Wikipedia and Kaggle data.

#### Objectives:

The goals of this challenge are:

1. Create an automated ETL pipeline.
2. Extract data from multiple sources.
3. Clean and transform the data automatically using Pandas and regular expressions.
4. Load new data into PostgreSQL.

## Resources

Data Source : movies_metadata.csv, ratings.csv, wikipedia.movies.json

Software : Python 3.7.7, Anaconda 2019.07, Conda 4.11.7, Jupyter Notebook, Pandas and SQL. 

## Assumptions

1. We are assuming that 7311 records for the raw wikipedia file is a reasonable number of data points to go ahead with.
2. We are not verifying the wikipedia data as it is updated by multiple sources. We are assuming the good data is accurate enough for analysis.
3. While comparing the columns in Kaggle data and wikipedia data having the same information, we mostly dropped the wikipedia columns as the Kaggle data was more accurate after looking at the scatter plots.
4. If columns in Kaggle data had missing information, it was pulled from the wikipedia columns before dropping the wikipedia columns.  
5. We are dropping columns that have more than 90% null values.
