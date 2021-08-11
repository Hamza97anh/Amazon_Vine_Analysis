# Amazon_Vine_Analysis
### Software used
- Pyspark
- RDS
- S3
- Postgres

## Overview
This projects pulls data from Amazon's database and looks at some data about videogame reviews. These reviews are made up of two main catagories, paid and unpaid. Using Pyspark we are able to manipulate and create tables and databases from this very large file. We begine by grouping Customer Id with their respective count in our datalist. Then a data table that groups product_id with their respective titles. Then we group these two tables to make a new table using review_id as primary key. Then we add a new table that will help us diffrentiate out paid vs unpaid reviews by adding a "vine" column to the table. Once all that is done we are able to make a new notebook that would use Pysparks built in analytics tool to produce a set of results that will determine the percent presense of bias in our data. 

## Results
- The number of vine reviews was a very small 94 compared to the normal unpaid 40471.
- The amount of paid 5 star reviews made up just a little over half of the reviews at 48 out of 94 making it 51%
- The amount of unpaid 5 star reviews made up a smaller percentage at approximtly 38%.  

## Summary
  What we can conclude with probable doubt form this analysis is that a paid review is likely to produce more 5 star reviews then a free one. That being likely caused by customers having a more positive atitude about the product and the company and being more leaniant with their review. An unpaid review is more liekly to generate an unbiased result, but overall it is generally accepted that people are more likely to submit a review when they're upset by a product then when they're not. For a solid conclusion, we would look at other review files for other products and then be able to accuratly determine if a paid review would skew the data heavily compared to unpaid. 
