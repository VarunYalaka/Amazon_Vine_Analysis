# Amazon_Vine_Analysis

## Overview of Project: 
Amazon Vine is an invitation-only program which selects the most insightful reviewers in the Amazon store to serve as Vine Voices. Vine Voices have the unique opportunity to order items free of charge and share their product experiences with Amazon customers to help them make informed buying decisions. In this project, I analyzed Amazon reviews written by Amazon Vine members. 

### Data set URL: https://s3.amazonaws.com/amazon-reviews-pds/tsv/amazon_reviews_us_Sports_v1_00.tsv.gz

## Tools and technologies used:
Below tools and technologies are used to perform the ETL process. 

* Pyspark

* AWS  (Amazon RDS and S3)

* PostgreSQL

* Pandas

* Google Colab Notebook

## Analysis Results:

* Performed ETL on Amazon Sports product reviews. As a first step loaded amazon data into spark data frame. 

![Screenshot 2022-12-20 at 9 57 27 PM](https://user-images.githubusercontent.com/44387918/208838234-9452193a-6026-4544-bad1-0dab8823ab45.png)

* Customers_table DataFrame.

![Screenshot 2022-12-20 at 9 57 40 PM](https://user-images.githubusercontent.com/44387918/208838263-d2ab615b-ad9f-44e1-a055-f1eb739c180e.png)


* Products_table DataFrame and dropped duplicates.

![Screenshot 2022-12-20 at 9 57 59 PM](https://user-images.githubusercontent.com/44387918/208838375-72857b8b-7e10-4613-a35e-0e1f77277c5f.png)

* Review_id_table DataFrame.

![Screenshot 2022-12-20 at 9 58 15 PM](https://user-images.githubusercontent.com/44387918/208838399-cc60beb0-a4cf-4fd3-98b8-8c0593010b54.png)

* Vine_table. DataFrame.


![Screenshot 2022-12-20 at 9 58 22 PM](https://user-images.githubusercontent.com/44387918/208838459-2a5f39ba-411d-4104-8baf-354d3ac39563.png)

* Number of vine reviews and non-vine reviews. 

![Screenshot 2022-12-20 at 10 09 38 PM](https://user-images.githubusercontent.com/44387918/208838525-8369ccfe-8e78-47d8-a264-692c4a1d6501.png)


* Number of 5 star reviews. 

![Screenshot 2022-12-20 at 10 09 43 PM](https://user-images.githubusercontent.com/44387918/208838497-439b2e7d-5d70-4df8-8cb4-5490ef54b0f4.png)

* 5 star reviews percentage. 

![Screenshot 2022-12-20 at 10 09 33 PM](https://user-images.githubusercontent.com/44387918/208838569-7b9d1b85-fa90-4fcd-970b-29f8959bd280.png)

 
## Summary: 

There’s no positivity bias observed for reviews in the Vine program. If you observed the five star percentage for paid vs non-paid there’s no significant difference observed. 0.4 % for Vine = Yes and 0.5% for Vine =No. Means more 5 star percentage from non paid reviews. 

## Additional analysis
* Number of vine table rows are 63329 and the verified purchase count is 42713. 

![Screenshot 2022-12-20 at 10 49 06 PM](https://user-images.githubusercontent.com/44387918/208840284-2813f81d-e20c-4e76-a260-a75c3c9aae41.png)


* Non paid review users are real and verified their purchases.
Verified purchase percenatage = 67.44 %

![Screenshot 2022-12-20 at 10 48 51 PM](https://user-images.githubusercontent.com/44387918/208840270-9d424916-dfb4-42d6-8f68-45c00e3ded32.png)

