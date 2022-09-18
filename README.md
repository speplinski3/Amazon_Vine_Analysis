# Analysis of Amazon Reviews by Vine Members

## Overview
* Purpose: To determine if reviews by Vine members are more likely to rate 5-stars on products versus those who are not Vine members.
* Method: By means of extracting, transforming, connecting to an `AWS RDS` instance, and loading data into `pgAdmin`.   `Pyspark` will be used within `Google Colaboratory` to filter and analyze a dataframe.

## Results
`Pyspark` was used within the `Google Colaboratory` notebook to import and read a dataset of Amazon Reviews on Apparel stored via `S3`. Results were filtered by reviews that have more than 20 votes and are considered more than 50% helpful.

![image](https://user-images.githubusercontent.com/103383489/190929966-d15bd329-f088-4c93-9907-0dcaca15f336.png)

* How many Vine reviews and non-Vine reviews were there?

The total count of reviews after filtering by most helpful reviews were **45421**.

Total count of Vine reviews was: **33**.

Total count of non-Vine reviews was: **45388**.

![image](https://user-images.githubusercontent.com/103383489/190930164-b5d9cbde-c024-424f-800a-bcc8862f005c.png)

* How many Vine reviews are 5 stars? How many non-Vine reviews were 5 stars? 

The total count of five-star reviews was **23748**.

Total count of Vine five-star reviews was **15**.

Total count of non-Vine five-star reviews was **21655**.

![image](https://user-images.githubusercontent.com/103383489/190930358-dfb493f7-b79c-4aec-9bf1-9788daf167e9.png)

* What percentage of Vine reviews were 5 stars? What percentage of non-Vine reviews were 5 stars?

Total percentage of 5-star Vine reviews: **45.46%**

Total percentage of 5-star non-Vine reviews: **47.71%**

![image](https://user-images.githubusercontent.com/103383489/190930375-aa47e5da-d82f-4869-8273-beb56bbc33b8.png)


## Summary

While there wasn't much of a difference in positivity bias between 5-star Vine vs. Non-Vine reviews (only 3%), the sample size of Vine reviewers was much smaller than the sample size of non-Vine users. Vine users made up .063% of the total five-star reviews representation, making it far too small to be useful data when comparing paid reviews versus non-paid reviews. A different dataset or an increase in sample size would be suggested.
