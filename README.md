# Challenge1
# Kickstarting with Excel

## Overview of Project
Louise's play "Fever" came close to it's fundraising goal in a short amount of time.The objective of the project is to analyze the given dataset to show Louise how different campaign fared in relation their launch dates and their funding goals.

Using Kickstarter dataset,the project will visualize campaign outcomes based on their launch dates and their funding goals.

### Purpose
Using the Kickstarter data set visualize campaign outcomes based on it's launch dates and funding goals.


## Analyze and Challenges

### Analysis of Outcomes Based on Launch Date
- In the Kickstarter_Challenge.xlsx workbook , I created a new column labeled "Years".In the "Years" column, use the YEAR() function to extract the year from the "Date Created Conversion" column.
- Create a pivot table from the Kickstarter worksheet,and place the pivot table in a new sheet. 
- Labaled the sheet "Theater Outcomes by Launch Date"
- Filter the pivot table based on "Parent Catogery","theotor" and "Years".
- Sort the "otcomes" field in decending order.
- used group by option to get the month value from launch date field
- Use values to count outcome, "successful","failed" and "canceled".
- then filter the column labels to show only "successful","failed" and "canceled"

![](images/dil1pivot.PNG)
-Finally created a line chart from the pivot table to visualize the relationship between outcomes and launch month.
![](images/Theoter_Outcomes_vs_Launch.png)

### Analysis of Outcomes Based on GOals
-In the Kickstarter workbook,I created a new sheet and lebel it "Outcomes Based on Goald."
In the new sheet,create the following columns to hold the data:
 - Goal
 - Number Successful
 - Number Failed
 - Number Canceled
 - Total Projects
 - Precentage Successful
 - Precentage Failed
 - Precentage Canceled
 
-In the "Goal" column,created amount ranges as per belpw
 - Less than 1000
 - 1000 to 4999
 - 5000 to 9999
 - 10000 to 14999
 - 15000 to 19999
 - 20000 to 24999
 - 25000 to 29999
 - 30000 to 34999
 - 35000 to 39999
 - 40000 to 44999
  - Greater than 50000
 -I used COUNTIFS() function to calaculate the "Number Successful","Number Failed" and "Number Canceled",on the "goal amount" column for the created ranges,and on the Subcatogery" column using "plays" as criteria.
 
 i.e: =COUNTIFS(kickstater!$D:$D,"<1000",kickstarter!$F:$F,"successfu[l",;kickstarter!$R:$R,"plays")
