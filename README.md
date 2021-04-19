
# An Analysis of Kickstarter Campaigns.
Performing analysis on Kickstarter data to uncover trends
## Brief Description of the Kickstarter Analysis
The objective of this analysis is to determine whether there are specific factors that makes a projects campaingn successful. The is based on the Kickstarter data which contains campaign information about different crowd funding project.
At the end of the analysis, we would be able to help Louise determine if she should jump into her first crowd funding campaign and what factors she should consider.
wip:
We can help Louise set up her incentives by first determining how much money people have pledged to campaigns historically. 
### The Analysis
The Kickstarter analysis provided the following insights to Louise
1. With the help of filters, we are able to focus on money raised by various campigns and we are able use data from the Pledged column to research projects with amounts similar Louise's monetary goal
2. A clear highlight of successful, failed, and canceled campaigns. This was achieved with the help of Conditional Formatting. This offers The ability to visually process outcomes at a glance will be very useful for Louise
3. To further assist Louise in her decision making, the analysis provides a percentage funded column. This will help Louise detrmine which projets gets the most donations. we achieved this with the an average funding column ( Percentage Donation) Now we can quickly determine how close a campaign came to reaching---and in some cases, exceeding---their funding goal.
4. The analysis takes the average donation a step further and applied visual cues to help Louise determine success or fail at a glance. we achieed this by we'll apply a range of colors, based on the percentage funded.
5. Another step in our analysis is help Louise determine what incentives she will attach to her funding goal, the analysis help Louise achieve this with Average Donation column, by examinining how much people have pledged to campaigns historically, we would help Louise determine 
  - a fair sense of what funding to expect and 
  - what incentives to offer
6. Since Louise is interested in the play subcategory, the analysis utilizes pivot tables to help visually uncover insights within the theater parent category
7. The story of Pivot Charts
8. The Story of Timing Success: highlight the use of formulas to convert dates
9. The Edinburgh Research (Highlights VLOOKUP Hepls know if they successfully funded)
10. Our analysis employs the measures of central tendency to determine how distributed the kickstarter data is.
11. Similarly, we employed measures of spread how varied our date is.
### The Findings
1. If we filter for only the United States campaigns, we will find that there were 525 successful theater Kickstarters.
2. We have found that while there are only a total of 604 Kickstarter campaigns for plays in Great Britain, the "theater" category is the most successful.

  ![Parent Category Outcomes](https://user-images.githubusercontent.com/67847583/115134457-dbd5bb80-9fd5-11eb-860b-3fccad301a92.png)

3. The month that launched the most successful Kickstarter campaigns was May. However, January, June, July and October all had roughly the same number of failed campaigns launched. This can be determined by examining the points along the trend lines of the chart.

  ![Outcomes Based on Launch Date](https://user-images.githubusercontent.com/67847583/115134453-d2e4ea00-9fd5-11eb-8f87-a5eb3706b4be.png)

4.The mean is larger than the median: skewed to the right

![Descriptive Statistics](https://user-images.githubusercontent.com/67847583/115182619-e52b5a80-a09f-11eb-990e-f7e0a731a284.png)


Based on these statistics, we can determine the following:
 - The mean of each distribution is around the 3rd quartile, so the data follows similar distributions in each subset.
 - The standard deviations are larger than the mean, which means everything below the mean is considered "close" to the center.
 - Some large values are driving all of these distributions. The standard deviations are all roughly twice the IQR in each distribution, except in the failed Kickstarters, where the standard deviation is closer to three times the IQR. There must be some failed Kickstarters with really high goals!



#### Recommendation

![Box Plots - Goal and Pledged](https://user-images.githubusercontent.com/67847583/115134583-06744400-9fd7-11eb-85fd-89a6bbadcae8.png)

From these plots, we can see that the mean campaign goal is around £4,000. This is outside of the range of outliers for amount pledged, so Louise should probably try to get her play produced for less than £4,000. Half of the campaign goals are less than £2,000, which is just over the 3rd quartile for amounts pledged.


