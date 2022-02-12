# Amazon_Vine_Analysis
Amazon_Vine_Analysis


## Overview
In this project, we have access to approximately 50 datasets. Each one contains reviews of a specific product, from clothing apparel to wireless products.  We picked Gift Cards datasets. 
We used PySpark to perform the ETL process to extract the dataset, transform the data, connect to an AWS RDS instance, and load the transformed data into pgAdmin. And then used PySpark again to determine if there is any bias toward favorable reviews from Vine members in our dataset. 


## Results

### Deliverable 1: Perform ETL on Amazon Product Reviews

* **Amazon_Reviews_ETL.ipynb** :  
![click here for : Amazon_Reviews_ETL.ipynb file](https://github.com/dhaval-28/Amazon_Vine_Analysis/blob/main/Amazon_Reviews_ETL.ipynb)

* **The customers_table DataFrame** :  
<p align="center">
<img src = "https://github.com/dhaval-28/Amazon_Vine_Analysis/blob/main/Images/Customer_Table_DF.png" /><br>
</p>

* **The products_table DataFrame** :  
<p align="center">
<img src = "https://github.com/dhaval-28/Amazon_Vine_Analysis/blob/main/Images/Products_Table_DF.png" /><br>
</p>

* **The review_id_table DataFrame** :  
<p align="center">
<img src = "https://github.com/dhaval-28/Amazon_Vine_Analysis/blob/main/Images/review_id_table_DF.png" /><br>
</p>

* **The vine_table DataFrame** :  
<p align="center">
<img src = "https://github.com/dhaval-28/Amazon_Vine_Analysis/blob/main/Images/vine_table_DF.png" /><br>
</p>


### Deliverable 2: Perform ETL on Amazon Product Reviews

* **5-star reviews for the two types of review (paid vs unpaid)** :  
<p align="center">
<img src = "https://github.com/dhaval-28/Amazon_Vine_Analysis/blob/main/Images/Del-2.png" /><br>
</p>

**| Attempt | #1 | #2 | #3 |**
| Attempt | #1 | #2 | #3 |
| Attempt | #1 | #2 | #3 |
| Attempt | #1 | #2 | #3 |

## Results

### State if there is any positivity bias for reviews in the Vine program
There are zero paid 5 start reviews. Our dataset is for gift cards and it seems like companies don't pay for gift card reviews. It's hard to detremine bias as there is not enough data to conclude paid reviews. Unpaid reviews has 87% positive reviews. So even unpaid reviews are also very positive.

We could perform the similar analysis for next best rating - (rating 4) and see if there is any bias. 

NOTE : it's very strange situation where there is no paid reviews which makes it harder to do any meaningful compariosn between paid vs unpiad. 



