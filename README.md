# Amazon Vine Analysis

![readme.PNG](PNGs/readme.png)


## Overview of the Analysis

The purpose of this assignment was to learn what constitutes big data and how it is handled. The task entailed analyzing Amazon reviews written by members of the paid Amazon Vine program. A dataset containing Amazon reviews of a specific product (shoes in this case), was provided. 

PySpark was used to perform the ETL process and to connect the data to an AWS RDS instance. After the data was transformed, it was loaded into pgAdmin. The main goal of the assignment was to determine if there was bias toward favorable reviews from Vine members in the dataset. In order to analyze the data, we used the following resources: 

- Spark to handle large Datasets
- Spark DataFrames and functions in Google Colab Notebooks
- Cloud Databases with Amazon Web Services
- Cloud Storage with S3 on AWS
- PySpark to perform ETL
- PostgreSQL


## Results

Using the above resources, the product reviews were counted and grouped by star ratings.

***How many Vine reviews and non-Vine reviews were there?***

There were 26,946 reviews in total. Out of that total, 22 were Vine (paid) reviews, and 26,924 non-Vine (unpaid) reviews. 


![vine_pu.PNG](PNGs/vine_pu.png)


***How many Vine reviews were 5 stars? How many non-Vine reviews were 5 stars?***

There was a total of 14,452 5-star reviews. Out of that total, 13 were 5-star Vine reviews, and 12,485 were 5-star non-Vine reviews.


![5-star.PNG](PNGs/5-star.png)


***What percentage of Vine reviews were 5 stars? What percentage of non-Vine reviews were 5 stars?***

- The percentage of total 5-star Vine reviews of total Vine reviews was 59%. 
- The percentage of 5-star Vine reviews of total 5-star reviews was 9%. 

- The percentage of total 5-star non-Vine reviews of total non-Vine reviews was 46%. 
- The percentage of 5-star non-Vine of total 5-star reviews was 86%


![perc.PNG](PNGs/perc.png)


## Summary

The results from the analysis seem to suggest that there was not a strong bias toward the Vine program and five-star reviews. Looking at the percentages, we can see that only 9% of total Vine reviews were 5-star reviews. In other words, the total of 5-star reviews was 14,452. Out of that total, only 13 reviews were part of the Vine program. In general, individuals write a review because they absolutely love the product, or truly dislike the product, especially regarding shoes. 

One additional analysis that I would recommend to fully support the analysis is counting the total of women and 5-star reviews, in comparison to men and 5-star reviews. Women tend to love and buy more shoes than men. They also tend to give their honest opinion, regarding fit and comfort. Because we do not have the gender information for this analysis, these numbers may not be an accurate representation of the product's worth, or distribution of the data.

Additionally, the results of the analysis could be further  examined by looking at the distribution of all stars (1-5) reviews.
