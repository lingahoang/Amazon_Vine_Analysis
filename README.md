# Amazon_Vine_Analysis

### Project Overview

__Executive Summary__

In this module, we are analyzing Amazon customer reviews to see whether there are bias between Vine paid vs. non-paid reviews. The process including import series of dataset from Amazon, using Google Collab to run pyspark and then finally load the finished dataframe into pgAdmin dataframe. 

Data Sources

[Pet Product Amazon Review](https://s3.amazonaws.com/amazon-reviews-pds/tsv/amazon_reviews_us_Pet_Products_v1_00.tsv.gz)


## Deliverable 1: Perform ETL on Amazon Product Review

The Pet Product dataset was extracted as a DataFrame 

![PET PRODUCT DATAFRAME](https://github.com/lingahoang/Amazon_Vine_Analysis/blob/main/Deliverable%20Images/Show%20DataFrame.png)

All four tables was successfully created and loaded into pgAdmin. 

| ![CT](https://github.com/lingahoang/Amazon_Vine_Analysis/blob/main/Deliverable%20Images/customer_id.png)      | ![PT](https://github.com/lingahoang/Amazon_Vine_Analysis/blob/main/Deliverable%20Images/product_id.png)        | 
| --------------------------------------------- |:---------------------------------------------:| 
| __Customer_id Table__ | __Product_id Table__ | 

 
| ![RT](https://github.com/lingahoang/Amazon_Vine_Analysis/blob/main/Deliverable%20Images/review_id.png)      | ![VT](https://github.com/lingahoang/Amazon_Vine_Analysis/blob/main/Deliverable%20Images/vine_table.png)        | 
| --------------------------------------------- |:---------------------------------------------:| 
| __Review_id Table__ | __Vine Table__ | 
  

## Deliverable 2: Determine Bias of Vine Reviews 

__Retrieve all votes that is equal or > 20__
![All votes](https://github.com/lingahoang/Amazon_Vine_Analysis/blob/main/Deliverable%20Images/%231.png)

__Retrieve all votes where `helpful_votes` divided by `totqal_votes` is greater and equal to 50%__ 
![](https://github.com/lingahoang/Amazon_Vine_Analysis/blob/main/Deliverable%20Images/%232.png)

__Retrieve all Paid Reviews__
![Paid Reviews](https://github.com/lingahoang/Amazon_Vine_Analysis/blob/main/Deliverable%20Images/%233.png)

__Retrieve all Unpaid Reviews__
![Unpaid Review](https://github.com/lingahoang/Amazon_Vine_Analysis/blob/main/Deliverable%20Images/%234.png)

__Review Totals__
![Review Total](https://github.com/lingahoang/Amazon_Vine_Analysis/blob/main/Deliverable%20Images/%235.png)


## Deliverable 3: 

__Results__

. How many Vine reviews and non-Vine reviews were there?

- There are 170 paid and 37,840 non-Vine reviews. 

. How many Vine reviews were 5 stars? How many non-Vine reviews were 5 stars?

- There are 65 reviews was 6 stars, and 20,612 non-Vine reviews were 5 stars. 

. What percentage of Vine reviews were 5 stars? What percentage of non-Vine reviews were 5 stars?

- There are 38% of Vine reviews that were 5 stars, and 55% of non-Vine reviews were 5 stars. 

## Summary

Based on the analysis, we can concluded that Vine members did not show any bias in their product rating as the percentage of 5-star rating are fairly comparable to non-Vine review as 38% versus 55%. 














