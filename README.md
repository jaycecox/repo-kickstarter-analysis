# Analysis of Outcome Based on Goal and Launch Date
---
Purpose:
---
The purpose of the analysis is to compare how the theater campaigns fared in relation to their launch dates and how play campaigns fared based on their funding goals.
---
Analysis:
---
*	Theater Outcome By Launch Date:
---
I collected the amount of times a theater campaign was labeled as successful, failed, and canceled for each month.  A pivot sheet was created to disseminate this information where all the data can be filtered by year in addition to campaign category. A corresponding line graph was created to illustrate the differences between outcomes of successful, failed, and canceled campaigns. 
---
![Outcome by Launch Date](https://user-images.githubusercontent.com/92542382/139611483-e599c273-1c2a-42fa-a0cb-053d22bb11c9.png)
---
* Outcomes Based on Goals
---
I established 12 different ranges for goal amounts and tallied how many times a project was labeled successful, failed, or canceled for each range. I filtered the projects to show only plays for each outcome. I did this utilizing the COUNTIFS() function, which you can find an example below:
---
(=COUNTIFS(Kickstarter!$D:$D,"<1000",Kickstarter!$F:$F,"failed",Kickstarter!$R:$R,"plays").
---
Using the SUM() function, I was able to calculate the total amount of plays for each goal range. I also calculated the percentage of successful, failed, and canceled plays  for each goal range. I did this  by dividing the number of each outcome by the total number of plays for each goal range.  A line graph was created to illustrate the percentage of how each outcome performed over each range. 
---
![Outcome Goal Percentage2](https://user-images.githubusercontent.com/92542382/139612817-e0e63829-d5d2-4cc4-af0a-13335f2d7788.png)
---
Challenges:
---
It was difficult to write the COUNTIFS() function, when trying to find the number of each outcome for each range. To find success, I watched the video in the module with an example of the COUNTIFS() function and performed the example activity in a separate workbook. For the project, I replaced the criteria of the example function with what outcome and subcategory I was using as a filter.  
---
Results:
---
* Theater Outcome By Launch Date:
---
I can  state that there were much more successful theater outcomes in the month of May than any other month.  There were also much less canceled theater outcomes when compared to the successful and failed outcomes, no matter the month of the launch date. 
---
![Theater_Outcomes_ vs_ Launch](https://user-images.githubusercontent.com/92542382/139610982-7efcfa46-70d5-4b7f-be9b-44e9ede3119b.png)
----
* Outcomes Based on Goals
---
Approximately 85% of total plays had a goal of up $9,999 with an average success rate of 68%. 
---
![Percentage of Success](https://user-images.githubusercontent.com/92542382/139615577-6f388dc7-5604-49f2-8d70-cb978819ce18.png)
---
![Outcomes_vs_Goals](https://user-images.githubusercontent.com/92542382/139610975-1a216819-cf3d-4be7-91b5-3bad26987789.png)
---
Limitations:
---
Some limitations presented was the lack of descriptive statistics, such as the mean or median goal amounts for each outcome. Perhaps a box and whisker plot would show this information in addition to any outliers. Be having this data presented in this way, we would be able to see the average or median goal amount for successful play campaigns. By knowing this we can set our own goal for future campaigns and compare our goals for past campaigns.  A box-and-whisker plot of for each outcome with its goal, would also show any potential outliers that may help us better understand the skew of the data.  This would allow us to help determine if the mean or median would be better to use. Through quartiles, a box-and-whisker plot would also show where the majority of the each outcome lies, giving us an idea of a range of goal amounts to choose from.   Overall, the dataset is limited based on what variables are used to determine success or failure.   Depending on how success or failure is measured, the same project might be considered either.
---
