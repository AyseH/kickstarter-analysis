
# Kickstarting with Excel

## Overview of Project

Louise is a play writer who is interested in learning how different theater campaigns performed in relation to their launch date and their funding goals.She nearly met her fundraising goal in her play ‘Fever’ and now she wants to get more in depth information about other campaigns.

### Purpose

The aim of this report is to uncover trends in the Kickstarter data and provide Louise with data analyses and visualizations to help her plan and set up her project.

## Analysis and Challenges

From the analysis of the Kickstarter Campaigns dataset we observe that there are over 4,000 campaigns in 9 different categories. Theater is the most successful category with 525 successful campaigns which is followed by the ‘music’(490 successful campaigns) and the ‘film & video’(261 successful campaigns) categories. 

### Analysis of Outcomes Based on Launch Date

When we look at the pivot table and graph for theater outcomes based on launch date, we can see that May is the ideal date to launch a campaign while December is the worst date. There are 111 successful plays in May (almost 67% of the theater campaigns were successful), while this number is only 37 in December which translates into a 49.3% success rate. June (65.36% success rate) and July (63% success rate) are also fairly good choices to launch a play. The graph also delineates that launch date does not affect its cancellation rate as the line is almost constant throughout the year.
![Theater_Outcomes_vs_ Launch](https://user-images.githubusercontent.com/81400525/115952944-8bb39900-a4ae-11eb-87bc-1ceab6bf0529.png)

### Analysis of Outcomes Based on Goals

The analysis of outcomes based on goals reveals that the success rate of the campaign decreases as the amount of goal increases. When goal is less than $1,000, 76% of the campaigns are successful, followed by 73% for the goal amount ranging between $1,000 and $5,000. The percentage of successful campaigns continue to be higher than the failed ones until the amount of goal reaches approximately $15,000. It picks up again around $37,000 until around $43,000. For the goal amount ranging between $45,000 and $49,999 all of the campaigns fail.Between goal amount $15,000 and $35,000 the percentage of failed campaigns are more than the percentage of successful campaigns.This is also true when the goal amount is over $45,000.
![Outcomes_vs_Goals](https://user-images.githubusercontent.com/81400525/115952969-a0902c80-a4ae-11eb-9dd4-805b85c3bb01.png)


### Challenges and Difficulties Encountered

The dates in the initial data set were not readable. They were entered in Unix time stamps, not standard format. First, we confirmed that these numbers in the date column were not just random numbers by using an online converter tool. After this step, we converted all the unix time stamps to standard format using a formula in Excel. Another problem we encountered was the errors in the ‘average donation’ column that we have created.We determined that some campaigns had no backers, therefore they received no funding. Hence, dividing 0/0 returned an error for these data. We fixed this by using the “IFERROR” formula in Excel.

## Results

The data on “Outcomes based on Launch Date’ reveals that theater is successful project throughout the year. The number of successful campaigns are always greater than the failed campaigns. Furthermore, in December failed campaigns (e.g. 35) are almost as much as the successful (e.g. 37) campaigns. In May, successful theater kick-starters (e.g. 111) are more than twice as much as the failed ones (e.g. 52). Based on the results of our analyses regarding “Outcomes Based on Launch Date” it might be better for Louise to consider launching her play in May. The line graph for “Outcomes based on Goals” shows that the success rate of the campaigns decreases as the funding goal increases.Campaigns with lower goals seem to be more successful than the campaigns with higher goals. If Louise wants to increase her chances of success to around 70% it would be wiser for her to keep her goal between $1,000 and $2,000. If she sets her goal between $5,000 and $10,000, there is approximately 50% chance that her campaign will succeed. The number of parent categories in the dataset is only nine which could be considered a limitation. The name and the blurb of the campaign could impact the amount of donations made. However, this requires qualitative analysis and we cannot perform that in Excel.This could be a potential limitation as well. In order to achieve a greater level of understanding of the dataset, it might be helpful to create a table to demonstrate the relationship between average donation and the month to uncover any potential trends between these variables. In addition,  creating a Box and Whisker plot for the plays to determine and visualize the outliers, the mean, the median and the upper and the lower quartiles might help Louise form more solid insights. Finally, it might be a good idea to check the relationship between the duration of the campaign and the success of the campaign.



