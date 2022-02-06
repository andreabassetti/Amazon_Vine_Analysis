# Amazon_Vine_Analysis

## Purpose 

The purpose of this project was to analyze Amazon reviews written by members of the paid Amazon Vine program. The Amazon Vine program is a service that allows manufacturers and publishers to receive reviews for their products. Companies like SellBy pay a small fee to Amazon and provide products to Amazon Vine members, who are then required to publish a review. I randomly chose the grocery data set form here: https://s3.amazonaws.com/amazon-reviews-pds/tsv/index.txt I used PySpark to perform the ETL process to extract the dataset, transform the data, connect to an AWS RDS instance, and load the transformed data into pgAdmin. Next, I used PySpark to determine if there is any bias toward favorable reviews from Vine members in the dataset. 

## Results:

In the char below are the results found in the pyspark analysis. 
|      |  Paid  |  Unpaid  |
|------|-------|-------|
|Total Reviews|61|28287|
|Five Star Reviews|20|15689|
| % of Five Star Reviews|32.78%|55.46%|


## Summary:

Looking at the results above, it is clear that there is a bias for higher five star ratings in the unpaid cluster. From this, you can conclude that it may not be worth to pay amazon for reviews in the groceries product category. 
