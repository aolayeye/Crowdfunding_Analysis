# Kickstarting with Excel

## Overview of Project

The objective of the Kickstarter analysis is to determine whether there are specific factors that makes a projects campaingn successful. The is based on the Kickstarter data which contains campaign information about different crowd funding project. In our initial analysis of the Kickstarter data we determined the following findings:
1. If we filter for only the United States campaigns, we will find that there were 525 successful theater Kickstarters.
2. We have found that while there are only a total of 604 Kickstarter campaigns for plays in Great Britain, the "theater" category is the most successful.
3. The month that launched the most successful Kickstarter campaigns was May. However, January, June, July and October all had roughly the same number of failed campaigns launched.
4. We also found that the mean goal, mean pledge are both larger than the median goal and median pledge respectively; this means Some large values are driving the distribution of the goal and median data, There must be some failed Kickstarters with really high goals!.
5. For the US market where Louise estimates she would require $12,000, nearly 50% of all US Kickstarter campaingns with $12,000.00 goals were successful while nearly 87% of all GB Kickstarter campaigns with $4,000.00 were successful. We may conclude that the hgher the goal the less likely the campaign will be successful.
6. From our Box Plots analysis, we can see that the mean campaign goal is around £4,000. This is outside of the range of outliers for amount pledged, so Louise should probably try to get her play produced for less than £4,000. Half of the campaign goals are less than £2,000, which is just over the 3rd quartile for amounts pledged.

### Purpose

The Purpose of the analysis is to determine the outcome of campaigns based on goals, and based on launch. At the end of the analysis we would be able to advise Louise on campaign goals to set and which month of the year is the best to begin her crowd funding project.

## Analysis and Challenges
1. As a first step in visualizing outcomes based on launch dates,  we added an a Year column and used the Year() formula to extract the Year the campaign was launched. 
2. Next created pivot tables on Years, and Parent Category as filters, outcomes as columns, and launch date as rows.
3. We then filtered the parent category column to display only the data for theather
4. Next, we created a line chart from the pivot table to visualize the relationship between outcomes and launch month.
5. To visualize Outcomes based on goals, our first step is to create a mini dataset that will hold goal ranges and the percentages of successful, failed, and canceled projects.
6. We used the COUNTIFS() functions to determine the number of successful, failed, and canceled projects based on the goal ranges
7. Next we used the SUM() function to total all outcomes for the different goal ranges, and then used then determined the percentages for each outcome.
8. Finally, we created a line chart of outcomes based on goals

### Analysis of Outcomes Based on Launch Date
1. From the Theater Outcomes Based on Launch Month, we find that the month that launched the most successful Kickstarter campaigns was May. However, January, June, July and October all had roughly the same number of failed campaigns launched. 



![Theater_Outcomes_vs_Launch](2021-04-20-21-33-56.png)



### Analysis of Outcomes Based on Goals
1. Campaigns with goals of $15,000 or less had more than 50% success rate.
2. Beyond $15,000 we see a dip in success rate, though a few campaigns with goals betwen $35,000 to $45,000 recorded higher than 60% suceess rate.
3. While very few campaigns with goals between $35,000 and $45,0000 had more than 65% success rate, more than 60% of all campigns with goals $15,000 or less were successful. This follows from our earlier Box plots analysis where we determined that the higher the goal the less like the campaign is successful

![Outcomes_vs_Goals](2021-04-20-21-27-46.png)


### Challenges and Difficulties Encountered
From our descriptive statistics of Successful, and Failed US Kickstarters we determined:
- The mean of each distribution is around the 3rd quartile, so the data follows similar distributions in each subset.
- The standard deviations are larger than the mean, which means everything below the mean is considered "close" to the center.
- Some large values are driving all of these distributions. The standard deviations are all roughly twice the IQR in each distribution, except in the failed Kickstarters, where the standard deviation is closer to three times the IQR. There must be some failed Kickstarters with really high goals!

## Results

- What are two conclusions you can draw about the Outcomes based on Launch Date?
1. From the Theater Outcomes Based on Launch Month, we find that the month that launched the most successful Kickstarter campaigns was May. However, January, June, July and October all had roughly the same number of failed campaigns launched.
2. The month of May might have been the most successful, it also had the highest number of failed campaigns. This may however be due to the fact May also had a high number campaigns.

- What can you conclude about the Outcomes based on Goals?
1. Campaigns with goals of $15,000 or less had more than 50% success rate.
2. Beyond $15,000 we see a dip in success rate, though a few campaigns with goals betwen $35,000 to $45,000 recorded higher than 60% suceess rate.
3. While very few campaigns with goals between $35,000 and $45,0000 had more than 65% success rate, more than 60% of all campigns with goals $15,000 or less were successful. This follows from our earlier Box plots analysis where we determined that the higher the goal the less like the campaign is successful

- What are some limitations of this dataset?
  While our analysis on outcomes based on launch date, and outcomes based on goals may have revealed the best time of the year to launch a campaign and the optimal campaign goal, it is essential to note that there may be further interactions between the different variables and whether a campaign is successful or not. Our analysis has solely based on continous variables (to determine whether a project is successful or not). If we had more qualitative data or we knew what variables like spotlight and staff_pick means, we may be able to illuminate other factors that are the strongest predictors of campaign outcome

- What are some other possible tables and/or graphs that we could create?
  Additional analysis can be done around length of campaign. This can be done by adding a calculated column that is the difference launch date and deadline. We may then create a pivot chart of campaign length on columns and outcomes on rows. This type of chart may help answer the question of the length of needed to run a campaign in order to be successful.

  This type of chart together with our outcomes based on launch date, and goals, Louise may be able to figure the sweet spot between this 3 variables.
