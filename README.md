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



* What percentage of Vine reviews were 5 stars? What percentage of non-Vine reviews were 5 stars?
