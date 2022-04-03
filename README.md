# Kickstarting with Excel

## Overview of Project
In this written report and analysis will attempt to describe Kickstarter campaign outcomes both based on their launch dates and on their funding goals. Included is the dataset, the relevant and analyzed data from that dataset (both in the Excel doc) along with some charts generated from them and my analysis in this README. 

### Purpose
The purpose of this analysis is to visualize Kickstarter campaign outcomes in relation to two factors: launch dates and funding goals. 

## Analysis and Challenges
The analysis itself was fairly straight forward with little difficulties, the data had few outliers and most of the data could be used as it was and didn't need much cleaning. One exception to that was splitting categories into subcategories by their delimiters. It was also a challenge for me to come to terms with the conclusions of this analysis because I can't help but wonder how reliable starting a kickstart based on these factors could be. Although I identify some correlations below I'm left wondering if there is not a better way to determine a Kickstart outcome.

### Analysis of Outcomes Based on Launch Date
In doing the analysis of Kickstarter outcomes based on launch dates I had to do a little data cleaning. I converted the Unix date to years, put the years column in my pivot table and from there filtered it down to month. This allowed me to look at all years as a data point on any given month. I went with a line chart as it's the best way to show this sort of data over time, with three lines one for canceled failed and successful kickstarters.
![Outcomes_vs_Launch Date](/resources/Theater_Outcomes_vs_Launch.png)

### Analysis of Outcomes Based on Goals
The analysis of the outcomes based on goals was fairly straight forward. I created a Goal column that splits the goal amounts in increments of 5000, giving us a decent spread of 12 rows. This allowed me to use a CountIf() function to populate a table to chart. A line chart was appropriate here as well with percentages on the x-axis and goal ranges on the y.
![Outcomes_vs_Goals](/resources/Outcomes_vs_Goals.png)

### Challenges and Difficulties Encountered
As I mentioned above there were few challenges or difficulties to be encountered, other than perhaps me learning the technology and methodologies involved. Creating the second line chart took me a while to format and display the correct data. Also this written analysis has proven to be a difficulty as I felt this template wants me to repeat myself over and over again on what is really a small starter analysis.


## Results

- What are two conclusions you can draw about the Outcomes based on Launch Date?

The first conclusion one may reach is that **The best month to start a kickstarter is May**. I suspect this is the case as summer is starting and consumers have less holidays and other obligations to spend their money on. The numbers stay high throughout the summer but never rise up to May levels again. The second conclusion we can reach is **The worst month to start a kickstarter is December**. This makes sense if we use the same logic as the first conclusion. Consumers are spending money on holiday shopping and traveling and are not looking to invest on a long term reward like a kickstarter. One thing to note is there were less successful kickstarters in the winter months but also less kickstarters in general, the failed kickstarters remain fairly consistent throughout the year

- What can you conclude about the Outcomes based on Goals?

One can conclude by looking at the Outcomes vs Goals chart above that **The lower the goal, the more likely you'll have a successful kickstarter**. It may appear that there is another point at the $35,000 Goal range where kickstarters are more successful, but if we look at the total numbers and not just the percentages we can see there is probably not enough data to come to that conclusion

![Outcomes_vs_Goals_Table](/resources/Outcomes_vs_Goals_table.PNG)

It makes sense that having a lower goal would make a successful kickstarter easier, but with this data we can see that the cut off point for previous kickstarters appears to be around the $10,000 - $15,000 mark.

In conclusion I would recommend one start a Kickstarter with a goal less than $15,000 (maybe even $10,000) and launch in May for the best chance at a successful kickstarter

- What are some limitations of this dataset?

The dataset feels very robust with a lot of information for further analysis, but of course there are some limitations. One big limitation is simply missing more modern data. The latest year in the dataset was 2017, which at the time of writing means there is 5 years of missing data. This is made even more important by the fact that the years missing are the most recent years and trends may have changed. I would also be interested to see how the pledges for any given Kickstart were made over time, perhaps kickstarters that reach a certain amount of their goal are more likely to complete the goal as people are convinced into it upon seeing early success, of course with this dataset this is not possible

- What are some other possible tables and/or graphs that we could create?

I would be curious to see charts using their 'spotlight' status as a filter and how that influenced the outcomes of kickstarters that launched at any time and at any goal. I would be interested in seeing how 'staff picks' influences outcomes in the same way. Another graph we could create is one that shows goal/launch date outcomes with years on the y axis, perhaps showing changes in trends of how and when people decide to back. Finally, one could also create a chart that shows how different types of kickstarts compare on their best goals and launch dates, perhaps there are trends we can apply to theater outcome that are hard to see using only the theater data
