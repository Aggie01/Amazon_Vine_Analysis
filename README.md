# Amazon_Vine_Analysis
------
------
## Overview:
- **SellBy** wants to know how the reviews of their products compare to the reviews of similar products sold by the competitors.

Type of reviews:
- **Vine** is the review that was written as part of the Vine program (paid).
- **Non-vine** review was not part of the program (unpaid).


## Purpose:
- Analyze the reviews in order to determine if there is any bias toward favorable ones.

## Methodology:
- PySpark to perform the ETL
- AWS RDS
- pgAdmin

## Results:
### Analysis of Amazon reviews, **vine (paid)** vs **non-vine (unpaid)** reveals the following:
- Based on the **total customer number** of reviews there are N=18,512 vine and N=3075,148 non-vine reviews.  
- Of the **total vine**, 8,044 are 5-star which make over 43% of the total customer number.
- The **majority** of the total number of reviews **belongs to non-vine reviews.**
- Non-vine reviews that are 5-star make 58% of the total number.

![](total_comparison_vine_vs_not.png)

- Based on the filtered **helpful votes (20 or more total votes)** there are N=1,080 vine and N=49,659 non-vine reviews.
- Of the **vine helpful votes**, 454 are 5-star which is over 42%.
- The **majority** **belongs to non-vine reviews.** Non-vine reviews make over 46% that are 5-star reviews.

![](comparison_vine_vs_not_percentage.png)

## Summary:
------
TO DO






## Suggestions:
Further analysis of electronics review section is proposed.  "What kind of electronics get the most positive vs most negative reviews?"  This can be from AirPods, IPads to TVs and speakers.  "Product_Id" and "product_category" variables should provide some strong insights.  
Customers rely largely on products reviews to make up their minds for better decision making on purchases; therefore, it is strongly suggested that more specific information about the product category is analyzed.  This can be done based on the the total_votes.
