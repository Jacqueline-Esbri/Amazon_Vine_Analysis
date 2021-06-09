# Amazon Vine Analysis

![readme.PNG](PNGs/readme.png)


## Overview of the Analysis

The purpose of this assignment was to learn what constitutes big data and how it is handled. The task led to analyzing Amazon reviews written by members of the paid Amazon Vine program. The goal was to determine if there was any bias in relation to favorable reviews from Vine members in the dataset.

A dataset containing Amazon reviews of a specific product (shoes in this case) was provided. PySpark was used to perform the ETL process and to connect the data to an AWS RDS instance. After the data was transformed, it was loaded into pgAdmin.  In order to analyze the data, we used the following resources: 

- Spark to handle large Datasets
- Spark DataFrames and functions in Google Colab Notebooks
- Cloud Databases with Amazon Web Services
- Cloud Storage with S3 on AWS
- PySpark to perform ETL
- PostgreSQL


## Results

Using the above resources, the product reviews were counted and grouped by star ratings. The analysis found the following:


***How many Vine reviews and non-Vine reviews were there?***

- There were 26,946 reviews in total. Out of that total, 22 were Vine (paid) reviews, and 26,924 non-Vine (unpaid) reviews. 


![vine_pu.PNG](PNGs/vine_pu.png)


***How many Vine reviews were 5 stars? How many non-Vine reviews were 5 stars?***

- There was a total of 14,452 5-star reviews. Out of that total, 13 were 5-star Vine reviews, and 12,485 were 5-star non-Vine reviews.


![5-star.PNG](PNGs/5-star.png)


***What percentage of Vine reviews were 5 stars? What percentage of non-Vine reviews were 5 stars?***

- The percentage of total 5-star Vine reviews of total Vine reviews was 59%
- The percentage of 5-star Vine reviews of total 5-star reviews was .09%

- The percentage of total 5-star non-Vine reviews of total non-Vine reviews was 46% 
- The percentage of 5-star non-Vine reviews of total 5-star reviews was 86%


![perc.PNG](PNGs/perc.png)


## Summary

The results from the analysis indicate a positivity bias towards the Vine program. Looking at the percentages, 59% of reviews were 5-star reviews, compared to 46% of 5-star non-Vine reviews. 

To show a Statistically significant quantity, trend, or deviation from the norm, the results could be further examined by calculating the statistical distribution (mean, median, and mode) of the star rating of Vine and non-Vine reviews. 