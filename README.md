# Amazon_Vine_Analysis
------
------
## Overview:
- **SellBy** wants to know how the reviews of their products compare to the reviews of similar products sold by the competitors.
- **Vine** is the review that was written as part of the Vine program (paid).
- **Non-vine** review was not part of the program (unpaid).


## Purpose:
- Analyze the reviews in order to determine if there is any bias toward favorable ones.

## Methodology:
- PySpark to perform the ETL
- AWS RDS
- pgAdmin

## Results:
Analysis of Amazon reviews, **vine (paid)** vs **non-vine (unpaid)** reveals the following:
- Based on the **total number** of reviews there are N=1080 vine and N=49659 non-vine reviews.  
- Of the **total vine**, 454 are 5-star which make 42% of the total number.
- The **majority** of the total number of reviews **belongs to non-vine reviews, N=23034.**
- Non-vine reviews make over 46% of the total number.

Tabulated results:

![](comparison_vine_vs_not_percentage.png)

## Summary:
------
TO DO

Tabulated results:
![](total_comparison_vine_vs_not.png)


## Suggestions:
