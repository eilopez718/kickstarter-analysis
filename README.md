# An Analysis of Theater-based Kickstarter Campaigns by Launch Date and Fundraising Goal

## Overview of Project
-Client wants to know if the launch date and goal amount of theater-based campaigns
in Kickstarter have any impact on their success or failure.	

### Purpose
-The goal is to measure the impact of Launch Date (specifically, month) and 
the size (amount being sought) on the success or failure of campaigns to see if there is a way
to maximize the possibility of success of any future campaigns.


## Analysis and Challenges

### Analysis of Outcomes Based on Launch Date
-The first step was to isolate theater-related campaigns from the data set and categorize 
them by launch date (month) and outcome (successful, canceled, failed.)  The next step was to graph
the outcomes across the months to see if there was an optimal time to launch a campaign.  

See Below:

![Theater_Outcomes_vs_Launch](https://user-images.githubusercontent.com/68127033/88493144-9374fa00-cf7d-11ea-800c-52bfbae7bff7.png)


### Analysis of Outcomes Based on Goals
 - I took the subset of the theater data related to plays and broke it into $5k increments
(with the exception of campaigns with goals of less than $1k or greater than $50k, which got their own categories) to see if the size of the goal of an individual campaign had any impact of the outcome.  I then calculated the percentage of successful, canceled, and failed campaigns for each of the aforementioned categories.  

See below:

![Outcomes_vs_Goals](https://user-images.githubusercontent.com/68127033/88493240-0ed6ab80-cf7e-11ea-913f-9ad7ebf18e28.png)






### Challenges and Difficulties Encountered
	
- Launch Date Data:  One challenge I encountered in calculating the data was that the months that had the 
highest number of successful campaigns also had the most failed and overall campaigns.  It wasn't clear if the 
number of successful campaigns in any given month was being driven by the timing of the launch or by the sheer 
volume of campaigns being launched that month.  To help understand this, I calculated the percentage of successful campaigns within each month to see if there was any differentiation.  I also calculated the percentage of total campaigns per month over the course of the year to ensure that there weren't a disproportionate number of campaigns being launched in any given month. 

See below:

![success_rate_month](https://user-images.githubusercontent.com/68127033/88493660-4cd4cf00-cf80-11ea-9461-7afe90f37449.png)



- Goal Data: The biggest challenge in evaluating the outcomes by goals is that the outcome percentages derived
give no weight to the sheer number of campaigns in each category.  To mitigate this, I calculated the percentage of total campaigns in each goal category as a percentage of the total to give context to the percentages in each category. 

See below:

![goal_project%_total](https://user-images.githubusercontent.com/68127033/88493552-b6a0a900-cf7f-11ea-9c10-52dffc087279.png)



## Results

- What are two conclusions you can draw about the Theater Outcomes based on Launch Date?
	1. May is the single most popular month to launch a theater-based Kickstarter campaign, and it has the highest number of successful campaigns.  June and July are also very popular, and have a high number of launched and successful campaigns.
	2. While May has the highest percentage of successful campaigns at 67%, the average for the all the campaigns throughout the year is 61%, with only 4 months having successful percentages of under 60%.  Month may play a role in the decision to launch campaigns, but it is unclear if they play a big part in determining whether or not a campaign will be successful.

- What can you conclude about the Outcomes based on Goals?
	1. Kickstarter campaigns for plays with a fundraising goal of $5k or less have a good probability of success. They are successful 73.5% of the time
- What are some limitations of this dataset?
	1.  In the goals data set, 85% of the campaigns have fundraising goals of less than $10k.  Depending on the Louise's fundraising goal, predicting the success of a campaign with a higher target may prove difficult.  

- What are some other possible tables and/or graphs that we could create?
	1. Including pledged amounts relative to goals might give some insight into the characteristics of the most successful campaigns.  If we created a field called "surplus to goal" (=(pledged-goal)/goal) and created a benchmark (>10%?) for the most successful campaigns and then studied the patterns in that subset, it might tell us more.
