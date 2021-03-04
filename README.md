# Comparing Individual Income in Baltimore City, MD and Hunterdon County, NJ using The Opportunity Atlas
## Background
For this comparison, Baltimore City, MD and Hunterdon County, NJ are being examined.  I grew up in Hunterdon County and came to Baltimore City for college.  The second I arrived in Baltimore, I noticed differences.  Instead of farms and horses on every street, there were skyscrapers, apartments, restaurants, and lots of people.  These differences are obvious and surface level.  For this analysis, I dig beneath the surface and study the individual income in each of these locations.  I am interested in the individual income metric on [The Opportunity Atlas](https://www.opportunityatlas.org/) because income can tell us a lot about the structure of a town or city.  I am interested to see how the income distribution compares for city neighborhoods and rural towns.  I was also curious about how population density and job density impacts individual income.  Baltimore has much higher population and job densities than Hunterdon County, so I wanted to see if that had an impact on individual income.  
## Business Question
_How is income distributed in city neighborhoods versus rural towns?_
## Data Sources
1. Baltimore City - Individual Income Data
https://github.com/shannonpowelson/comparing-baltimore-hunterdon-county-individual-income/blob/main/Baltimore%20City%20-%20Individual%20Income%20Data.xlsm
This data from The Opportunity Atlas contains the average annual income for children from neighborhoods in Baltimore City, MD.  It is the individual income so a spouse's income is not included.  This data was collected in 2014-2015. 

2. Baltimore City - Job Density Data
https://github.com/shannonpowelson/comparing-baltimore-hunterdon-county-individual-income/blob/main/Baltimore%20City%20-%20Job%20density%20Data.xlsm
This data from The Opportunity Atlas contains the number of jobs per square mile in each neighborhood in Baltimore City, MD.  This data was collected in 2013.  

3. Baltimore City - Population Density Data
https://github.com/shannonpowelson/comparing-baltimore-hunterdon-county-individual-income/blob/main/Baltimore%20City%20-%20Population%20Density%20Data.xlsm
This data from The Opportunity Atlas contains the number of residents per square mile in each neighborhood in Baltimore City, MD.  This data was collected in 2010. 

4. Hunterdon County - Individual Income Data
https://github.com/shannonpowelson/comparing-baltimore-hunterdon-county-individual-income/blob/main/Hunterdon%20County%20-%20Individual%20Income.xlsm
This data from The Opportunity Atlas contains the average annual income for children from towns in Hunterdon County, NJ.  It is the individual income so a spouse's income is not included.  This data was collected in 2014-2015. 

5. Hunterdon County - Job Density Data
https://github.com/shannonpowelson/comparing-baltimore-hunterdon-county-individual-income/blob/main/Hunterdon%20County%20-%20Job%20Density%20Data.xlsm
This data from The Opportunity Atlas contains the number of jobs per square mile in each town in Hunterdon County, NJ.  This data was collected in 2013.

6. Hunterdon County - Population Density Data
https://github.com/shannonpowelson/comparing-baltimore-hunterdon-county-individual-income/blob/main/Hunterdon%20County%20-%20Population%20Density%20Data.xlsm
This data from The Opportunity Atlas contains the number of residents per square mile in each town in Hunterdon County, NJ.  This data was collected in 2010.

7. Analyzed Excel Data
https://github.com/shannonpowelson/comparing-baltimore-hunterdon-county-individual-income/blob/main/Analyzed%20Excel%20Data.xlsm
This file contains the condensed data from each of the raw data files described above.  It also contains the excel spreedsheets used to create each graph used in the Data Analysis section.  


## Data Analysis
To start this analysis, we will look at two bar graphs showing the distribution of individual income in Baltimore City, MD and the distribution of income in Hunterdon County, NJ.  
![alt text](https://github.com/shannonpowelson/comparing-baltimore-hunterdon-county-individual-income/blob/main/individualincomebaltimore.png)
![alt text](https://github.com/shannonpowelson/comparing-baltimore-hunterdon-county-individual-income/blob/main/individualincomehunterdoncounty.png)
The above graphs show that individual income is distributed differently in Baltimore City and Hunterdon County.  In Baltimore City, there is a large range of incomes.  There are very high incomes and very low incomes.  However, in Hunterdon County, the incomes are very similar and consistent.  There are no extreme values like in the incomes for Baltimore City.  

__Why are incomes distributed differently in Baltimore City and Hunterdon County?__

For the next part of the analysis, I tested my hypothesis on why I thought that this difference in income distrbution occurs.  I thought that job density and population density might have an impact on income distribution.  Areas with more available jobs might have higher incomes and areas with higher populations might have lower incomes because of more competition for jobs.  

First, I investigated the impact of job density on income distribution in the following combination charts.  
![alt text](https://github.com/shannonpowelson/comparing-baltimore-hunterdon-county-individual-income/blob/main/jobdensitybaltimore.png)
![alt text](https://github.com/shannonpowelson/comparing-baltimore-hunterdon-county-individual-income/blob/main/jobdensityhunterdoncounty.png)
The above graphs show that there is no clear association between job density and individual income distribution in Baltimore City and Hunterdon County.  This shows that the amount of jobs in a certain area is not impacting the income.  

Since job density is not playing a role in income distribution differences, I investigated the impact of population density on income distribution in the following combination charts. 
![alt text](https://github.com/shannonpowelson/comparing-baltimore-hunterdon-county-individual-income/blob/main/populationdensitybaltimore.png)
![alt text](https://github.com/shannonpowelson/comparing-baltimore-hunterdon-county-individual-income/blob/main/populationdensityhunterdoncounty.png)
The above graphs show that there is no clear association between individual income distribution and population density in Baltimore City and Hunterdon County.  This shows that the population in a certain area is not impacting the income.  


## Summary
Overall, this data analysis revealed that the income distribution of neighborhoods in Baltimore City is very diverse and contains both high and low income extremes.  In contrast, the data analysis revealed that the income distribution of towns in Hunterdon County is relatively uniform.  There are no extreme values.  More research is needed to extend these findings to city neighborhoods and rural towns in general, but for this specific case, the data shows that city neighborhoods experience income diversity while rural towns have uniform incomes.  When searching for a reason for these differences in income distribution, the data analysis revealed that population and job density do not have a clear impact on income distributions in either location.  More data analysis using sociodemographic metrics would be helpful to determine the reason for the difference in these income distributions.  For example, instead of the impact of the job density, the impact of the types of jobs should be studied.  Also, instead of the impact of population density, the impact of the opportunities, education, and resources available to the people in certain areas should be studied.  The outcomes of this analysis are important for me.  I grew up in a place where income disparities were not common and therefore when encountered with income disparities I assume that it must be attributed to economic factors like job density or competition for jobs due to population density.  However, this data analysis showed me that income disparities are actually most likely impacted by social factors like education levels, opportunities, available resources, and more.  Therefore, when approaching Baltimore-centric solutions, I will be sure to keep these disparities and social factors in mind. 
