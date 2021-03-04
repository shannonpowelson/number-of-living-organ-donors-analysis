# Analyzing the Number of Living Organ Donors with Respect to Donor Age and Gender
## Background
For this anlaysis, the number of living organ donors is being examined.  [Living organ donors](https://www.kidney.org/transplantation/livingdonors/general-information-living-donation#:~:text=Living%20donation%20takes%20place%20when,sister%20(living%20related%20donation).) are people who donate an organ or part of an organ while they are alive.  Living donors can donate an entire kidney or parts of their lung, liver, or pancreas to family members, friends, or strangers in need.  I became interested in organ transplants since I want to pursue a career in tissue engineering and artificial organ engineering.  Despite many advancements in 3D bioprinting organs, these artificial organs are not yet approved to be implanted into humans in need.  According to the [Health Resources and Services Administration](https://www.organdonor.gov/statistics-stories/statistics.html), "17 people die each day waiting for an organ transplant".  Therefore, organ donation is extremely important and more research needs to be conducted to find ways to recruit more organ donors.  In these analyses, we use data from the [Organ Procurement and Transplantation Network](https://optn.transplant.hrsa.gov/data/) to investigate the affect that age and gender has on the number of living donors.  The goal is to see if we can predict how many living donors there most likely could be in a group of people given the ages and genders of people in this group.  This could provide insight into age groups and genders that can be better marketed to to gain more donors.  

## Business Question
_Can we predict the number of living organ donors based on age and gender?_
## Data Sources
 

## Data Analysis


### _Simple Linear Regression_
I first conducted simple linear regressions for each of the indepdent variables in order to explore the association between the independent variable and the total number of living donors (our dependent variable).  The following plots show the simple linear regression plots for the total number of living donors vs each independent variable.  The graph also contains the least squares line, the R-Squared value, and the linear trendline.   

![alt text](https://github.com/shannonpowelson/number-of-living-organ-donors-analysis/blob/main/SimpleLR-%3C1.png)
![alt text](https://github.com/shannonpowelson/number-of-living-organ-donors-analysis/blob/main/SimpleLR-1-5.png)
![alt text](https://github.com/shannonpowelson/number-of-living-organ-donors-analysis/blob/main/SimpleLR-6-10.png)
![alt text](https://github.com/shannonpowelson/number-of-living-organ-donors-analysis/blob/main/SimpleLR-11-17.png)
![alt text](https://github.com/shannonpowelson/number-of-living-organ-donors-analysis/blob/main/SimpleLR-18-34.png)
![alt text](https://github.com/shannonpowelson/number-of-living-organ-donors-analysis/blob/main/SimpleLR-35-49.png)
![alt text](https://github.com/shannonpowelson/number-of-living-organ-donors-analysis/blob/main/SimpleLR-50-64.png)
![alt text](https://github.com/shannonpowelson/number-of-living-organ-donors-analysis/blob/main/SimpleLR-65.png)
![alt text](https://github.com/shannonpowelson/number-of-living-organ-donors-analysis/blob/main/SimpleLR-male.png)
![alt text](https://github.com/shannonpowelson/number-of-living-organ-donors-analysis/blob/main/SimpleLR-Female.png)

In the above graphs, it is clear that some independent variables have a stronger linear association with the number of living donors than others.  This is evident by how closely the data points follow the linear trendline.  In the table below, there is a list of the R-Squared value for the simple linear regression of each of the independent variables.  The R-Squared value tells us the proportion of the variance in the number of living donors that be explained by the independent variable.  It ultimately tells us how well the data fits the linear regression line and thus how certain we are of the association between the number of living donors and the independent variable.  

![alt text](https://github.com/shannonpowelson/number-of-living-organ-donors-analysis/blob/main/R-Squared.png)

In the simple linear regression for the number of living donors less than 1 years old and the number of living donors 1-5 years old, 1.29% and 0.06% of the data fits the linear regression models.  Therefore, we are almost uncertain of an association between these age groups and the total number of living donors.  For 11-17 year olds, 16.82% of the data fits the linear regression model.  This certainty level rises dramatically for the 18-34 year olds group since 77.85% of the data fits the linear regression model.  Out of all of the age group independent variables, we are most certain of an association between the 35-49 year old age group and the total number of living donors since 78.87% of the data fits the linear regression model.  For age groups after this, the R-Squared values go back down and thus we become less certain of the association.  For 50-64 year olds, 50.38% of the data fits the linear regression model and for people older than 65, 3.88% of the data fits the linear regression model.  The 35-49 year old age group data therefore fits the linear regression model the best and we are most certain of the association between this age group and the number of living donors than we are for the other age groups. This would be interesting to investigate in future research.  For gender groups, 98.77% of the data for females fits the linear regression model, while 96.66% of the data for males fits the linear regression model.  

### _Multiple Linear Regression_



These are some key results from out multiple linear regression.
![alt text](https://github.com/shannonpowelson/number-of-living-organ-donors-analysis/blob/main/MultipleLR-ResultsTable.png)




## Summary
This is important for marketing 
