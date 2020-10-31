# AWS_ETL_Vine_Analysis

## Overview

The purpose of the Vine ETL analysis was to retrieve an Amazon dataset of my choice and read that into a Spark DataFrame. The dataset I chose was the Video Games dataset because I am a gamer. From here, I created a new DataFrame that contained the review information and Vine information. I cleaned up the dataframe by pulling the reviews with 20+ total votes and at least 50% or greater helpful votes. The final steps included determining how many total 5 star ratings Vine and Non-Vine ratings there were total as well as their respective percentages, then summarizing the results.

### Results

I can say that I was not surprised to see that the paid-Vine results had more 5 star reviews compared to the non-Vine reviews but there were definitely a lot less reviews.


- How many Vine reviews and non-Vine reviews were there?

For the dataset I worked with, there were 94 Vine reviews and 40,471 non-Vine reviews.

https://github.com/jasonatoledo/AWS_ETL_Vine_Analysis/blob/main/Resources/Vine_Reviews.png
https://github.com/jasonatoledo/AWS_ETL_Vine_Analysis/blob/main/Resources/NonVine_5stars.png

- How many Vine reviews were 5 stars? How many non-Vine reviews were 5 stars?

There were 48 Vine reviews that were 5 stars and 15,663 non-Vine reviews that were 5 stars

https://github.com/jasonatoledo/AWS_ETL_Vine_Analysis/blob/main/Resources/Vine_5stars.png
https://github.com/jasonatoledo/AWS_ETL_Vine_Analysis/blob/main/Resources/NonVine_5stars.png


- What percentage of Vine reviews were 5 stars? What percentage of non-Vine reviews were 5 stars?

The percentage of Vine reviews that were 5 stars is 51.06% and the percentage of non-Vine reviews was 38.70%.



Here is the summary DataFrame I created for the challenge:

https://github.com/jasonatoledo/AWS_ETL_Vine_Analysis/blob/main/Resources/AWS_ETL_Summary.png


## Summary

I was not surprised to see that the Vine reviews had a higher % of 5 star ratings than the Non-Vine reviews. As seen above in my AWS_ETL_Summary screenshot, we can clearly see there is a slight bias for Vine subscribers to have more 5 star reviews. If I were to add another analysis to support this, I would also filter the original Vine DataFrame using the "verified_purchase" column values set to "Y" only as the next step in my analysis. I would also try a different dataset from AWS to see if the results are similar to the video games dataset.
