# Food-Insecurity-MySQL-Project
A MySQL Query To Organize food insecurity rankings from 2017-2022

The data took the national (all 50 states) health measures from America's Health Ranking and specifically focused on 'Food Insecurity' for the 2017 - 2022 years to examine the top 4 most populated states have a higher prevalence of food insecurity as compared to the least 4 populated states. 

Excel was used to remove the unwanted variables from the analysis, of which the blanks were replaced with NULL. 

The data was then imported to MySQL and a database was created. 
The following code was written:

SELECT *
	FROM 2017_annual
    WHERE Measure_Name = 'Food Insecurity'
    
UNION

SELECT *
	FROM 2018_annual
    WHERE Measure_Name = 'Food Insecurity'
    
UNION

SELECT *
	FROM 2019_annual
    WHERE Measure_Name = 'Food Insecurity'
    
UNION

SELECT *
	FROM 2020_annual
    WHERE Measure_Name = 'Food Insecurity'
    
UNION

SELECT *
	FROM 2021_annual
    WHERE Measure_Name = 'Food Insecurity'

The data was then exported back to Excel to be organized and processed further. 'District of Columbia' and 'United States' were removed and the data was organized to create a timeline chart. 

The data was color-coded after for visualization purposes. 
