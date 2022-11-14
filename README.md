# Amazon_Vine_Analysis
## Overview of the analysis: 
The main purpose is to analyze the amazon product reviews to find if there is any positivity bias toward favorable reviews from Vine(paid) members when compared to non-Vine(unpaid) members.
I chose the US jewellery dataset. Then I used PySpark to perform the ETL process to extract the dataset, transform the data, connect to an AWS RDS instance, and load the transformed data into pgAdmin. Next, I used PySpark to determine if there is any bias toward favorable reviews from Vine members in the jewellery dataset.

## Results: Using bulleted lists and images of DataFrames as support, address the following questions:
![paid vs unpaid analysis](https://github.com/Meghajain84/Amazon_Vine_Analysis/blob/main/finding_bias.PNG)
* How many Vine reviews and non-Vine reviews were there?
    * There were 21 vine reviews vs 7689 non-Vine reviews
* How many Vine reviews were 5 stars? How many non-Vine reviews were 5 stars?
    * There were 11 5-star Vine reviews vs 4444 5-star non-Vine reviews
* What percentage of Vine reviews were 5 stars? What percentage of non-Vine reviews were 5 stars?
    * There were 52.38% of Vine 5-star percentage vs 57.8% of non-Vine 5-star percentage of all helpful reviews
## Summary: In your summary, state if there is any positivity bias for reviews in the Vine program. Use the results of your analysis to support your statement. Then, provide one additional analysis that you could do with the dataset to support your statement.
* Looking at the numbers, I don't see the positivity bias for reviews in the Vine program. Infact, it's slightly less than non Vine review percentage. Total number of reviews is way less for Vine members when compared to non-Vine members.
* I would have also filtered the dataframe for "verified_puchase" equals to 'Y' while creating new dataframe with helpful votes greater than 50%. 
* To further support the analysis, statistical analyis can be done on star_rating


