# Amazon Vine Analysis

## Overview of the analysis
### Objective
The purpose of this analysis was to work with data from an AWS dataset, pull it into PySpark in combination with Postgres hosted on AWS. Then, perform data analysis on top of the data available within the PySpark dataframes to draw conclusions. 



## Results
### Answering the following questions:
- How many Vine reviews and non-Vine reviews were there?
  - In total, there are 1,785,997 reviews. 

![Total Reviews](/Resources/Total_Reviews.png)

- How many Vine reviews were 5 stars? 
  - There are 1,607 5 star Vine reviews

![Vine 5 Star Reviews](/Resources/5_Star_Paid_Reviews.png)

- How many non-Vine reviews were 5 stars?
  - There are 1,025,317 non-Vine 5 star reviews

![non-Vine 5 Star Reviews](/Resources/5_Star_Unpaid_Reviews.png)

- What percentage of Vine reviews were 5 stars?
  - Only 0.156% of the 5 stars reviews are from Vine  

![% Vine 5 Star Reviews](/Resources/5_Star_Paid_Pct_Reviews.png)

- What percentage of non-Vine reviews were 5 stars?
  - 99.844% of the 5 stars reviews are from non-Vine 

![% non-Vine 5 Star Reviews](/Resources/5_Star_Unpaid_Pct_Reviews.png)

## Summary
### DB Check
We loaded data into a Postgres DB using PySpark. These were the results: 

![DB Stats](/Resources/Postgres_DB_Update_Checks.png)

### Is there any positivity bias for reviews in the Vine program?

With the analysis performed, we can't say there is no positivity bias given that we only looked at reviews with 5 stars. 
If we were only to take that information into account, then we could say that there is NO positivity bias given that only 0.15% of the Vine reviews were 5 stars.
However, we need to perform the analysis with reviews that are 3+ stars across vine and non-vive to determine if there's an actual positivity bias in the paid reviews. 

