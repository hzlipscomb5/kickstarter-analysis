# Kickstarting with Excel

## Overview of Project

### Purpose
The purpose of the analysis was to gain insights on common characteristics for succesful kickstarter campaigns for plays. Louise has the beginnings of a succesful play on her hands 
and requested more information on the best practices to follow through with her launch. She requested research on two specific variables, one was how different projects fared relative to 
their launch date and the other was how goal amounts affected the success of the projects. 
## Analysis and Challenges
### Analysis of Outcomes Based on Launch Date
The proccess of analyzing based on launch date was a fairly simple. The first step was creating a pivot table that collected that data for "Succesful", "Failed", and "Canceled" 
kickstarter campaigns and then sorted them by the months they were launched. The pivot table had filters for both the year of launch and the subcategory of the project. After filtering
the table to "plays", we could study the benefits and drawbacks for the respective months of launch. To make the information easier to consume, it was also converted into a line chart.
The line chart made it even more clear that certain months had a substantial advantage or disadvantage. 
### Analysis of Outcomes Based on Goals
For the analysis of outcomes based on their goals, we used a "COUNTIFS" formula in Excel to gather the neccesary data into a table. An example of one line of this formula reads
`=COUNTIFS(Kickstarter!$F:$F, "successful", Kickstarter!$D:$D, ">=1000", Kickstarter!$D:$D, "<=4999",  Kickstarter!$R:$R, "plays")`. This would give you the count of successful plays that
had a goal between $1000 and $4999. Using variations of this formula, the results were broken down by differing ranges of goal amounts. The table that was created organized the raw counts, 
which were then converted into percentages. 
### Challenges and Difficulties Encountered
Overall, this was a simple analysis, and minimal difficulties were experienced. One minor difficulty arose with "COUNTIFS", this a novel formula which caused a few headaches at the onset,
but was quite simple once the protocol was established. One potential difficulty that could be imagined, would be if the analyst has previously filtered the dataset and forgotten to reset
this. Also the creation of the "Outcomes Based on Goals" table required careful proofreading, which could has caused issues if it was not diligently created.
## Results
- What are two conclusions you can draw about the Outcomes based on Launch Date?
One takeaway that leapt from the data, was that a May launch delivered a distinct advantage for the plays' kickstarter campaigns. The May release advantage was visualized by a clear spike in
the line chart. May was one of few points in the year when the ratio of successes and failures were not relatively constant. While the May surge came quickly, June and July saw an 
advantage as well, but this slowly decreased through these months and had entirely dissipated by August. While late Spring through Early summer was the prime spot for success, there was 
a clear disadvantage for launches in December. December was the only point in the year where the number of failed attempts and succesful plays nearly converged.
- What can you conclude about the Outcomes based on Goals?
The results of outcomes based on goals was not quite as clear as the other analysis, but some insights could be gleaned from the data. The highest success rate came from the two smallest
goal ranges, which were "Less than $1000 and $1000 to $4999". Following the success of the lower ranges, we found some parity. The ranges from $5,000 and $24,999 had quite even success rates. 
The larger the goal amounts grew, the sample sizes became smaller, which appeared to lead to some inconsistency towards the bottom of the table. The last clear result was that for goals
over $50,000, success rates took a nosedive.
- What are some limitations of this dataset?
The most apparent limitation of the dataset, for our research goals, was the small sample size for larger goal amounts. This weakness in sample size caused some inconsistencies in the larger 
goal groups, but that seemed to be remedied by in the $50,000 and above category. While it was not in the purview of our analysis, effects of the city of release might be a variable 
worthy of consideration for plays specifically. The marketing and promtion schemes utilized by the various kickstarters would also be a nice dataset to consider for someone like Louise. 
Another weakness in the dataset, was that the dollar amounts were listed in the same column with various other currencies, it might have been better to have a column the values 
converted to a standard currency. 
- What are some other possible tables and/or graphs that we could create?
It would be interesting to have a table that compiled information on average donations and the average number of backers for each outcome. The table with average donations and number of 
backers could split amongst different goal or pledged amounts as well. A table and chart for success rate by year would have less obvious actionable insights. Although, if certain 
years stood out as unusual we could check for factors such as the economy that year, for example a recession might cause a spike in failures. 


