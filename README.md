# An Analysis on the Outcomes of Kickstarter Theater Campaigns
## Overview of Project
The purpose of this analysis is to reveal the potential relationship between the outcomes of Kickstarter campaigns of the theater category and their corresponding launch date and funding goals. 
## Analysis and Challenges
### Outcome with Respect to Launch Date
For the relationship between outcomes and corresponding launch dates of the campaign, a pivot table is created from the original data. The launch dates are categorized by month, and the occurrence of different outcomes, namely “successful”, “failed”, and “canceled”, are aggregated for each calendar month. A chart is then created based on the table.
### Outcome with Respect to Funding Goals
In order to demonstrate the relationship between outcomes and the funding goals, a table is created with the rows being different level ranges of funding goals and the columns being the numbers of corresponding outcomes, and the percentages of the outcomes in the subtotal. In this case the value in each entry is the count of the outcomes calculated with the COUNTIFS() function, or the percentage derived from the counts. A chart is also created with the data from the table.
## Results
### Theater Outcomes by Launch Date
![alt text](https://github.com/gabac1/kickstarter-analysis/blob/main/Theater_Outcomes_vs_Launch.png)
Two conclusions can be drawn from the above analysis. First, neither the total number nor the subsequent outcomes are evenly distributed throughout the calendar months, and there is strong seasonality. Second, specifically, May has both the highest number of campaigns and the highest ratio of successful ones, both followed by the subsequent month June. On the contrary, December has the least number of campaigns and the lowest success ratio.
### Outcomes based on Goals
![alt text](https://github.com/gabac1/kickstarter-analysis/blob/main/Outcomes_vs_Goals.png)
The outcomes with respect to funding goals graph demonstrates a general trend, which is that the higher the goal is, the lower possibility it has to success. There is however, exceptions occurring on the 35000-39999 and 40000-44999 categories, where the success rate is relatively higher comparing to the categories below and above. 
### Limitations of the Dataset
One limitation of this dataset is that it doesn’t contain information related to the cause of cancellation of the canceled campaign, or information which could help to infer the cause. It highly likely that a lot of the campaigns are canceled due to the lack of interest from the public and thus a low pledge relative to their goals, yet we cannot be absolutely sure about it. To make distinctions between the campaigns canceled due to lack of money, just like the failed ones, and the campaigns canceled due to other reasons may help us draw a clearer picture of the situation. But luckily, due to the relatively small number of canceled campaigns, the analysis is not likely to be vitally affected by the missing information.
Further statistical significance tests on the difference between the monthly success ratios may also be helpful. 
