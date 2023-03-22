# Amazon_Vine_Analysis

## Overview of Analysis
- The purpose of this analysis was to determine if there was any form of bias created as a result of the Vine review program. Specifically we wanted to see if customers apart of the  Vine program had a positive/ negative bias towards the subset of products listed on the amazon website as result of being a part of the "paid-for" program. As compared to customers that were not apart of the Vine program, which of course was free. We pulled data from an Amazon AWS bucket on pet supply product reviews and used Pyspark to parse the data and create data sets in order to determine if any bias was present. For more accurate results, we filtered the initial data set from the AWS bucket to show reviews with votes greater than or equal to 20 to pick reviews that are more likely top be helpful in our analysis and to avoid having division by zwero errors. In addition, we continued to filter the reviews further by selecting only reviews where the number of "helpful votes" was equal toor greater than 50% of the "total votes". this was to filter out low valued outliers and to again use data that will be avoerall more helpfulll for the analysis.  

## Results
As a part of this results section, we are lookkng to answer the three main questions listed below:

  1. How many Vine reviews and non-Vine reviews were there?
  
  2. How many Vine reviews were 5 stars? How many non-Vine reviews were 5 stars?
  
  3. What percentage of Vine reviews were 5 stars? What percentage of non-Vine reviews were 5 stars?

- Based off of our analysis, of the reviews we deemed valued. There were a total of 38,010 reviews. With 170 being Vine reviews and 37,840 non Vine reviews. Of the Vine reviews there were only 65 5-star reviews, or we can say that approximately 38.23% of all vine reviews for the pet product customer review dataset were 5-star reviews. Alternativily, of the Non-Vine product reviews there were a total of 20,612 5 star reviews. Based off of those figures, approximately 54.47% of the Non-Vine reviews were 5-star reviews.

## Summary 

 - Considering the results of the analysis discussed above I would come to the conclusion that there is no positivity bias in regards to the reviews in the Vine program. Of the two subsets of data, the reviews from the vine program had a significantly less percentage of 5-star reviews as compared to the Non-Vine program reviews. It would be importaant to state that with such a low number of Vine reviews the data could be impartial. We may not be getting the whole scope of the analysis considering there were significantly less Vine reviews, than Non-Vine reviews. I understand the need to filter the intial data set to show only "helpful" information but it might be best to run the analysis on a larger portion of the initial data set to get a bigger picture of who is providing 5-star reviews in general. It might also be helpful to determine what value on the spectrum of the "star rating" column is deemed as positive or negative. we could then also include reviews that were givin that were equal to or greater than that "positive" star rating ( possibly 4 or 3 ). This would provide a possibly larger data set to draw conclusions from.  IN addtion, we couls also determine which reviews provided a low rating ( 1 or 2 ) and look in to if there was any possible negative bias associated with the Vine reviews/ Non-Vine reviews by running the same analysis. 
