# data-visualization-and-mining

Since we all know, the used data in data analysis should be in clean form. As garbage data is provided as input, garbage data will be returned as output. As a result, we'll need to identify and erase any dirty data.
In advanced, we have discovered a limited number of duplicate records in the data set (only 286 in total), as well as some outliers data.   However, we could work with data even if there were a few minor outliers, and the analysis would be unaffected. For outliers' findings, we also built code in Jupyter notebook.
According to the analysis on notebook, there are 4538 outliers across all columns. Even with this small number of outliers, we can do our study.
Duplicate data is 256 records, which is a minor number when compared to the 52966 records, and it is a traffic offense that is easily reproduced.
we don't consider all of the 134544 null values to be dirty data:

We discovered that null data mostly in these two columns, and the note column isn't very important to us because the country name column has 52966 missing values, which isn't important in our analysis, and we can remove the entire column. We also found missing values in the search type column, which isn't important to us. The other null values in each column are almost 3000, which is not a large quantity given the dataset's 52966 rows.





•	Contents of the data

Essentially, we were only given one dataset to choose from and analyze. Approximately 65k+ traffic violation records are contained in the Traffic Violations Dataset. In relation of this dataset, it's a round 65k+ traffic-related violation that has been recorded that contained in this collection. Further details and their attributes are shown below:

1.      stop_date - the driver's violation date 
2.	stop_time - the driver's violation time
3.	driver_gender - the driver's violation gender (Female F, Male M)
4.	driver_age - the driver's violation age
5.	driver_race - the driver's violation race 
6.	violation - the driver's violation type














The quality of the data

-	 Velocity (also known as speeding) Violation
-	the Violation Movement (the driving is reckless, the driver hits others and run away, the driver assaults others, violation of pedestrian, improper turns and lane changes, etc)
-	 Vehicle (infractions such as window tinting, taillight or headlight loss, noisy exhaust, cracked front window, and so on.)
-	Registration/Plates 
-	driver's Registration or plates 
-	The belt of the seats
-	A variety of violations (the Service's call, a city's or town's ordinance violation, an individual's suspicion, aiding the driver /courtesy of the driver, etc.)



7. search_conducted - Whether or not the search is carried out in True or False manner.
8. stop_outcome - Violation outcome
9. is_arrested - Determines whether or not a person has been arrested in True or False manner.
10. stop_duration - Approximate detention time for offenders (in minutes)
11. drugsrelatedstop - Determine whether or if a person was caught in a drug charge (True, False)




•	Estimate of how clean the data is
Category 	Evaluating and ensuring 
Validity	Validity is not fully applied in the data, as two
attributes within the driver_age_raw are not totally valid year. Hence, we applied some data cleaning using python to display these data.
Accuracy	Some of the columns contained upper and lower bound. 
Hence, we have applied some Python coding to display these
 outliers' data 
Completeness	Some values where missing or null. We have counted them, and it turned out to be 134544 as total
Hence, we applied some python coding to display these data.
Consistency	Consistency means how consistence the data is.	
Since there is minor duplicated value that won't impact our analysis. Hence, we have used some python coding to find out totals of consistency in the data. 
Uniformity	After examining the data, we have seen that the Data seemed to be uniformed.










Summery
A New York City taxi driver was allegedly handed the first traffic violation in the United States around May 20, 1899, while driving at a speed of more than 12 miles per hour. Since then, various fines for traffic violations have been imposed across the country, and states have collected unfathomable billions of moneys from taxi driver violators.
There are 2 kinds of traffic violations: big and small violation. The most common violations are parking violations, which are not recorded on a driver's record but can lead to arrest if not paid.
The most frequent type of traffic violation is exceeding the posted speed limit. The speed limits are determined by the state. People in penal institutions and detention centers were also given health and demographic information as part of the Times' data collection project. 
2.	 Aims & Objective 
This project has several aims, one of which is to learn how to use data sets, combine them, and analyze them through practice, as well as how to use Jupyter notebook for analyzing and working with csv files in analysis using the libraries of NumPy and pandas.  Another aim is to practice selecting relevant aspects to locate a problem and then solve them. We also aim to improve our knowledge of plotting and other enhanced features that are used in practice, as well as our visualization skills using matplotlib. We also aim to learn certain data analysis methods in each data set through this practice.




One of our objectives is to develop a research question and explore it, after which we will create a report on what we have learned in order to answer the question. We also want to import the necessary libraries into Jupyter notebook or (ANACONDA). Following that, we'll look at the relationships between the independent and dependent variables that we've chosen. We plan to use the SQL language and the Pandas data frame Python library to do this. To do so, we'll need to employ a correct correlation measurement to show the correlations between our chosen variables, as well as appropriate visualizations created with various libraries.
3.	The Research Question
i.	By determining the independent variables, compared to the dependent variable, we are willing to examine them, and their presentation in the datasets, and their relationship, and their nature whither they are dependent or independent based on their properties for the purpose of examining datasets. We are presenting the datasets that are dependent or independent based on the nature of their properties for the purpose of examining datasets.
 
ii.	 we will list our dependent variables that we are willing to examine, followed by the table bellow
Question 	independent variable	dependent variable
What's the relationship between driver_race and is_arrested? 	driver_race	is_arrested
What's the relationship between driver_gender and is_arrested	driver_gender	is_arrested



Our Research Question is: What is the relationship between driver race and the arrested? We will manage to do that, by investigating the independent variable driver_race, and driver_gender, compared to the dependent variable is_arrested. 

 
Analysis & findings 

convincing correlations
We are aiming to investigate the relationship between gender, and race of the driver, and being arrested. 
We manage to do that using the tools provided by Jupyter notebook, using python, to determine the correlations between dependent and independent variables. We have found a correlation between: 

-	Race of the driver and number of being arrested
-	Gender of the driver, and times being arrested 

critical interpretation and conclusions 
The Data shows a relationship between race and being arrested. Hence, for Black and Hispanic people arrested is much more than white and Asian people. So, we would consider this in our analysis even we have more variables to consider but we have noticed that this is a big important variables and differences. We have also found a relationship between gender and being arrested. (SUMBRIA, 2022)



![image](https://user-images.githubusercontent.com/63984422/171057194-b92f1599-4a40-4855-b99d-323b1451dd9c.png)









tabular summaries


 
In this table we have found that Black, and Hispanic individuals are getting arrested more than white and Asian, this could be due many reasons, including the cultural background, and level of income. (SUMBRIA, 2022)






![image](https://user-images.githubusercontent.com/63984422/171057242-4a819fb1-692e-41f7-a49b-3b7e5aa86150.png)





![image](https://user-images.githubusercontent.com/63984422/171057176-29a3f11a-a2ef-4765-b2c6-c95cc2a81244.png)



Visualization with their interpretations

 

Figure indicates a statistically significant association between race and being arrested, since Pearson Chi-Square had p <0.01. The highest percent of total arrested drivers were Black, followed by Hispanic. The more the person identified with the Black race or Hispanic race, the more likely they are being arrested. On the other hand, the lowest percent of total arrested drivers were among Asian, followed by White. The more the person identified with the Asian or White race, the more likely they are not being arrested.





