# 	The purpose of the Analysis
The purpose of the analysis was to assist Louise launch her crowdfunding successfully.
She seemed to be more interested into the theatre categories, so we went ahead and filtered our categories based on the theater to have a better overview of the outcomes based on the launch dates using mainly the months as this will help with seeing the trends of successful, failed and cancelled outcomes over the past few years.
Using a chart, we also identified the goals that were reached failed or succeeded (sometimes by exceeding their goals) based on the outcomes of the campaign, to do so we divided the goal amount in different ranges to have a clear view based on the outcomes of the plays.
# 	Analysis and challenges
## 	Analysis 
For us to carry out this analysis the following steps were taken:

1.First as the data we were given for launch date (column I) and deadline (column J) was not in a readable format: it was in Unix timestamps ; we had to make it readable in dates in standard format using the formula : =(((J2/60)/60)/24)+DATE(1970,1,1) as well as: =(((I2/60)/60)/24)+DATE(1970,1,1) . By doing so we created column S and T for the date ended conversion and date started conversion. 

2. We then had to separate our category to obtain column Q and R for our parent category and subcategory as we were interested in pointing out theather and plays which were the focus of our analysis
3. After that we created a new column for years which will assist us during our analysis to establish the relationship between theater and outcomes based on the launch dates by using the formula : =YEAR(T2) 
4. The above steps allowed us to create a pivot table based on dates in standard format as we wanted to overview the outcomes of the project based on launch dates. We filtered our pivot tanle based on parent category and years and obtained the chart below

 ![image](https://user-images.githubusercontent.com/99924850/156952302-5bf8dd9b-a0f9-4eaf-9d9b-761649914054.png)



	5.Then we did a comparison of the theater’s outcomes by filtering the parent category to show us only the theater data and created a chart based on theater based and outcomes and obtain the following table and chart
  
![image](https://user-images.githubusercontent.com/99924850/156952902-a8454937-a5e3-4c77-a94c-6da300fa3d91.png)

 
6. We then created a new sheet to establish the relationship between the goals and outcomes by dividing the goal amount in different ranges and established the number of goals that were successful, failed or canceled using the COUNTIFS formula. For example we used this formula for the range of 0-1000 goal amount that were successful: =COUNTIFS(KickStarter!D2:D4115,"<1000",KickStarter!F2:F4115,"successful",KickStarter!R2:R4115,"plays")
.* We then created a line chart to visualize the relationship between the outcomes and goals which gave us the following table and line chart.
![image](https://user-images.githubusercontent.com/99924850/156953375-387e1c27-76e6-430a-b255-eb6c1174c688.png)




 


## Challenges
The challenges we encountered included the unreadable data were given which led us to create column I and J to obtain a more readable set of data. 
The second challenge was the COUNTIFS function as although the concept was understandable it took me a great amount of time to be able to come up with a formula that would work for each row and this was to be duplicated on every single column of the outcomes (failed, successful and canceled)
# Conclusion 
## Theater outcomes by Launch Date
By looking at our graph and table we can conclude that the launch was most successful in May and June. There is a high chance of a having a failed launch in November and December before.
## 	Outcomes based on goal
The conclusion I came up with was that the higher the goal the less chances it has to succeed.
By looking at my graph and table we can identify a trend of failed goals starting from a goal as big as $20 000 and higher whereas small goal of $15000 and less have seen a high rate of success.  
# 	Limitation and possible new analysis 
The first limitation was the fact that the data included currency which did not specify which dollar we were working with 
Also based on the quality of the data provided there was no clear mention on the reason why the goals failed, succeeded or were cancelled which leave us on guessing on the reason of trends being illustrated on our charts. 
The above limitation leaves a room on analysis based on the reason why the goals were not met if we were given more data. 
We can also create a line chart to understand the trends in theater crowdfunding
We can conduct an analysis between the pledgers and percentage funded as well as average donation.

