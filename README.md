# Kickstarting with Excel

## Overview of Project
In this written report and analysis will attempt to describe Kickstarter campaign outcomes both based on their launch dates and on their funding goals. Included is the dataset, the relevant and analyzed data from that dataset (both in the Excel doc) along with some charts generated from them and my analysis in this README. 

### Purpose
The purpose of this analysis is to visualize Kickstarter campaign outcomes in relation to two factors: launch dates and funding goals. 

## Analysis and Challenges
The analysis itself was fairly straight forward with little difficulties, the data had few outliers and most of the data could be used as it was and didn't need much cleaning. One exception to that was slpitting categories into subcategories by thier delimiters. It was also a challenge for me to come to terms with the conclusions of this analysis because I can't help but wonder how reliable starting a kickstart based on these factors could be. Although I identify some correlations below I'm left wondering if there is not a better way to determine a Kickstart outcome.

### Analysis of Outcomes Based on Launch Date
In doing the analysis of Kickstarter outcomes based on launch dates I had to do a little data cleaning. I converted the Unix date to years, put the years columnn in my pivot table and from there filtered it down to month. This allowed me to look at all years as a data point on any given month. I went with a line chart as its the best way to show this sort of data over time, with three lines one for canceled failed and successful kickstarters.

### Analysis of Outcomes Based on Goals
The analysis of the outcomes based on goals was fairly straight forward. I created a Goal column that splits the goalk amounts in increments of 5000, giving us a decent spread of 12 rows. This allowed me to use a CountIf() function to populate a table to chart. A line chart was appropriate here as well with percentages on the x-axis and goal ranges on the y.


### Challenges and Difficulties Encountered
As I mentioned above there were few challenges or difficulaties to be encountered, other than perhaps me learning the technology and methodologies involved. Creating the second line chart took me a while to format and display the correct data. Also this written analysis has proven to be a difficulty as I fell this template wants me to repeat myself over and over again on what is really a small starter analysis.


## Results

- What are two conclusions you can draw about the Outcomes based on Launch Date?

![Outcomes_vs_Goals](/Resources/Outcomes_vs_Goals.png)

The first conclusion one may reach is that **The best month to start a kickstarter is May**. 

There were less successful kickstarters in the winter months but also less kickstarters in general, I suspect other factors might be better for determining a succesful kickstarter.

- What can you conclude about the Outcomes based on Goals?

- What are some limitations of this dataset?

- What are some other possible tables and/or graphs that we could create?
