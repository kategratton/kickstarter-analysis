# Kickstarting with Excel

## Overview of Project

### The purpose of this project was to gauge Play campaign outcomes (either Successful, Failed or Canceled) based upon their launch dates, and their funding goals.

## Analysis and Challenges

### Analysis of Outcomes Based on Launch Date

Gathering this particular outcome was a simple process using a PivotTable.  Placing the outcomes in the Columns field, Date Created Conversion in the Row Field, and Count of Outcomes in the Value Field, I was able to calculate the total amount of Successful, Failed, and Canceled campaigns based on the months the campaign was launched. I also applied a Parent Category - theater filter, and an All Years filter to the date to focus on the overall theater based campaign data. Once completed, I graphed this analysis in a line chart seen below. 
![image of Theater Outcomes Chart](https://github.com/kategratton/kickstarter-analysis/blob/8d6783378573e251bc786c662eb6dcf44fb1a388/Resources/Theater_Outcomes_vs_Launch.png)    
    
   
    
### Analysis of Outcomes Based on Goals
Creating this analysis was more of an manual task. I created a datasheet with the Headers including Number of Successful, Failed, and Canceled Projects; as well as the Total amount of Projects, and the correlating successful, failed and canceled percentage rates. I broke up the data in Goal increments of $4999, starting at Goals less than 1000, and finishing with goals over $50,000. 

Using the `COUNTIFS()` function, I calculated the total amount of successful, failed and canceled campaigns in the "Plays" subcategory. I then used the `SUM()` function to calculate the total plays, and completed the Percentage columns of each outcome by dividing the number of projects in said outcome by the total number of projects overall. Once I had a decimal number in place, I used the `Percent Style` option in Excel to create my percentages. All of this data was caterogized by the Goal column, with my Goal funding intervals. 

Once all the data was organized, I created a Line graph showcasing the "Outcomes Based on Goal", with my Goal intervals on the X axis, and the percentage rates as the y axis. As we see below, no projects in the "Plays" subcategory were canceled, however the Goal amount with the highest success rate was for projects with less than $1000 Goal amounts. 

![image of Outcomes based on goals chart](https://github.com/kategratton/kickstarter-analysis/blob/8d6783378573e251bc786c662eb6dcf44fb1a388/Resources/Outcomes_vs_Goals.png)
     
### Challenges and Difficulties Encountered
Challenges encountered appeared espeically in the "Outcomes Based on Goals" worksheet. Using the `COUNTIFS()` function, but having to edit it per row leaves alot of room for user error, therefore causing incorrect data reporting. A few times the function/formula was repeating the formula entered in the cell above, and would also provide warning errors until the full column was complete. Editing and reviewing the formaulas for all cells constantly was key to make sure accurate data was being reported. 
    
## Results

### What are two conclusions you can draw about the Outcomes based on Launch Date?
I have determined that the month of May had the highest amount of successful play campaigns, this would be the first conclusion. However, the lowest month for failed campaigns was November, which would be the second conclusion. With this data, I would recommend launching your campaign in the month of May, with an end campaign date of November.
     
### What can you conclude about the Outcomes based on Goals?
I can conclude that the best Goal amounts to insure a successful campaign outcome would be in the lower tiers - meaning Less than $1000; with $1000-$4999 being the next best Goal amount. However, my findings did show that the next highest percentage of Successful campaigns appeared in the $35,000-$44,999 Goal amounts. Therefore, if a higher goal amount is needed, I would recommend applying a goal between $35,000-$44,999.
    
### What are some limitations of this dataset?
Unfortuantely, this dataset only covers years 2009-2017, which means the data is at least 5 years old. To start a campaign in 2022/2023. I would recommend having data from the last 5 years to have more modern and relevant data. As well, this dataset is limited in the "Outcome Based on Goals" worksheet in that any outcomes with goal amounts above $50,000 are blended into one row of data - and are no longer well defined. Because of this, there is the potential to identify any outliers, or in the least other successful goal outcomes for this dataset. 
      
### What are some other possible tables and/or graphs that we could create?
The Following are other possible tables and/or graphs that could be created:
- A Clustered Column Chart for the "Outcomes Based on Goal" Table
- A Line with Markers Chart for the "Outcomes Based on Goal" Table
- A Pivot Table for the "Outcomes Based on Goal" Table, with Goal totals, and number of successful, failed and canceled outcomes, filtered by year if needed. 
- A Clustered Column Chart for the "Theater Outcomes by Launch Date" PivotTable
- A Pie Chart for the "Theater Outcomes by Launch Date" PivotTable, with each outcome (successful,failed, canceled) having it's own Pie Chart.
- A Box and Whisker Chart for the "Theater Outcomes by Launch Date" PivotTable, showcasing each outcome and it's potential outliers.
