# Amazon_Vine_Analysis
------
------
## Overview:
- **SellBy** wants to know how the reviews of their products compare to the reviews of similar products sold by the competitors.

Type of reviews:
- **Vine** is the review that was written as part of the Vine program (paid).
- **Non-Vine** review was not part of the program (unpaid).


## Purpose:
- Analyze the reviews in order to determine if there is any bias toward favorable ones.

## Methodology:
- PySpark to perform the ETL
- AWS RDS
- pgAdmin

## Results:
### Analysis of Amazon reviews, **Vine (paid)** vs **Non-Vine (unpaid)** reveals the following:
- Based on the **total customer number** of reviews there are N=18,512 Vine and N=3075,148 Non-Vine reviews.  
- Of the **total vine**, 8,044 are 5-star which make over 43% of the total customer number.
- The **majority** of the total number of reviews **belongs to Non-Vine reviews.**
- Non-Vine reviews that are 5-star make 58% of the total number.

![](total_comparison_vine_vs_not.png)

- Based on the filtered **helpful votes (20 or more total votes)** there are N=1,080 Vine and N=49,659 Non-Vine reviews.
- Of the **vine helpful votes**, 454 are 5-star which is over 42%.
- The **majority** **belongs to Non-Vine reviews.** Non-Vine reviews make over 46% that are 5-star reviews.

![](comparison_vine_vs_not_percentage.png)

## Summary:
It is concluded that there was no positive bias from the Vine reviews. The proportion of Vine vs Non-Vine votes is about the same for 5-star. In other words, paid reviews do not guarantee/gear toward positive opinions.  Vine memebers post unbiased opinion and compenstation does not guarantee a positive review.  


## Suggestions:
Further analysis of electronics review section is proposed.  "What kind of electronics get the most positive vs most negative reviews?"  This can be from AirPods, IPads to TVs and speakers.  "Product_Id" and "product_category" variables should provide some strong insights.  
Customers rely largely on products reviews to make up their minds for better decision making on purchases; therefore, it is strongly suggested that more specific analysis about the product id and category is performed.  This can be done based on the total_votes.
