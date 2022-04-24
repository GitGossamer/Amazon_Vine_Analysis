# Amazon_Vine_Analysis
Mod 16 - Big Data

# Overview of the analysis of the Vine program: The purpose of this analysis is well defined (3 pt)
The purpose of this analysis was to analyze Amazon reviews written by members of the paid Amazon Vine program, a service that allows manufacturers and publishers to receive reviews for their products. Companies like SellBy pay a small fee to Amazon and provide products to Amazon Vine members, who are then required to publish a review.
In this project, we had access to approximately 50 datasets, each one containing reviews of a specific product, from clothing apparel to wireless products. We picked just one of these datasets (Furniture) and used PySpark to perform the ETL process to extract the dataset, transform the data, connect to an AWS RDS instance, and then load the transformed data into pgAdmin. 
Additionally, we used PySpark, Pandas to determine whether there was any bias toward favorable reviews from Vine members in your dataset. 

## Results: There is a bulleted list that addresses the three questions for unpaid and paid program reviews (7 pt)
•	How many Vine (PAID) reviews and non-Vine (UNPAID) reviews were there?
 ![Total number of PAID Reviews](https://user-images.githubusercontent.com/96449605/164954574-2e224a85-0860-4e01-93f9-89b943b4c492.png)
 ![Number of Reviews_UNPAID](https://user-images.githubusercontent.com/96449605/164954586-799d8931-d58a-49d5-9601-ae6a06ec8fdb.png)

 •	How many Vine (PAID) reviews were 5 stars? How many non-Vine (UNPAID) reviews were 5 stars?
 ![5 Star Reviews_PAID](https://user-images.githubusercontent.com/96449605/164954609-6912db0d-04cb-4978-a3cb-c1b13f062622.png)
 ![Number of 5 Star Reviews_UNPAID](https://user-images.githubusercontent.com/96449605/164954618-9a0a41c3-357e-4705-ba58-78bf92750160.png)

 •	What percentage of Vine (PAID) reviews were 5 stars? What percentage of non-Vine (UNPAID) reviews were 5 stars?
 ![Percent of 5 Start Reviews_PAID](https://user-images.githubusercontent.com/96449605/164954635-d371b70d-57a7-4d1e-ad41-d76eec0eb846.png)
 ![Percentage of 5 Star Reviews_UNPAID](https://user-images.githubusercontent.com/96449605/164954655-ab4cfb82-94e2-4871-a790-4ebd08e7527e.png)

 
### Summary: The summary states whether or not there is bias, and the results support this statement (2 pt); An additional analysis is recommended to support the statement (2 pt)

In Summary, it’s unclear whether or not there is good value in the Vine program service.
On the negative side, it would seem that there isn’t good value in having the Vine program because of the completely unbalanced volume ratio of Vine (21 Paid) reviews compared to non-Vine (6,690 Un-Paid) reviews.
On the positive side, there is some value in having the Vine program service because new products need to have some reviews in order to kickstart their sales, otherwise there’s the possibility of them not being touched with a  10 ft cattle prod. 
With those two arguments being as they are, there’s still only a marginal 0.039% difference between the paid Vine reviews (0.476%) and the unpaid Vine reviews (0.515%). So the long and the short of it is that there’s really not that much of an incentive for the Vine program service for people to write positive 5-star reviews for products.

