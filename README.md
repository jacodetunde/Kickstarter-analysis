# Kickstarter-analysis
An analysis of Kickstarter campaigns.
To uncover trends from the data 
![Subcategory.png](path/to/Subcategory.png)
![ParentCategory.png](path/to/ParentCategory.png)
![Datelaunched.png](path/to/Datelaunched.png)

# Overview of Project
Analysis of the Kickstarter campaigns in order to uncover how different campaigns fared in relation to launch dates and funding goals. 
## Analysis and Challenges
##### Outcomes Based on Launch Date
I created a pivot table filtered by Parent Category and Years, with outcomes on the column and as values and Years on the rows. I used this pivot table to create a line chart that show how Kickstarter Theater campaigns fared all through the years. *Attached is the chart created*
![Theater_Outcomes_vs_Launch.png](path/to/Theater_Outcomes_vsLaunch.png)
##### Outcomes Based on Goals
To analyse the outcomes based on goals, the Goals are grouped from 1000 to 50,000 with 4000 intervals, COUNTIFS technique was used to calculate the number of outcomes (successful,failed and canceled) in each goals' interval. Percentage of outcomes are calculated for each group to uncover the pattern of outcomes accross goals interval. *Attached is the chart*
![Outcomes_vs_Goals.png](path/to/Outcomes_vs_Goals.png)
#### Challenges faced.
The first challenge faced, was, how to use COUNTIFS() method to calcualte the number of outcomes in each goals intervals. However, I was able to overcome this challenge by looking at the hints provided and google some additional tips.
The second challenge was confusion between using ROUND() or Percentage metric. Using ROUND() was not showing % on the Y-axis of the  chart, while Percentage metric does. I decided to use Percentage metric instead of ROUND() formula.
## Results
##### Insights from Theater Outcomes based on Launch Date Analysis
1. The trend of Theater Outcomes based on Launch Date is seasonal in nature. The month of May is the Theater most successful campaign. With a fewer pick in february and October, while Theater campaign had relatively no success in December. 
2. It could also be observed that there were no cancellation of campaign in October with fewer successes.
In general, the pattern of movements of the outcomes accross the year shows that there is a positive correlation between failed and successes with the exception of the December. Though, this claim can be investigated further with the aid of regression analysis in order to confirm that.
##### Insights from Outcomes based on Goals 
It can be deduced from this analysis that, the lower the goals, the higher the success rate and the higher the goal the lower the success rate.
However when the goal was between 40000 and 50000 the success rate was higher than the failed rate, this might be due to the income level of the target group that made the pledge. As a result of that there is a need for an additional column on the income level of the persons that pledges towards the Kickstarter campaign for full picture of the outcomes.



