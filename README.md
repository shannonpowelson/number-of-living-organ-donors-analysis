# Analyzing the Number of Living Organ Donors with Respect to Donor Age and Gender
## Background
For this anlaysis, the number of living organ donors is being examined.  [Living organ donors](https://www.kidney.org/transplantation/livingdonors/general-information-living-donation#:~:text=Living%20donation%20takes%20place%20when,sister%20(living%20related%20donation).) are people who donate an organ or part of an organ while they are alive.  Living donors can donate an entire kidney or parts of their lung, liver, or pancreas to family members, friends, or strangers in need.  I became interested in organ transplants since I want to pursue a career in tissue engineering and artificial organ engineering.  Despite many advancements in 3D bioprinting organs, these artificial organs are not yet approved to be implanted into humans in need.  According to the [Health Resources and Services Administration](https://www.organdonor.gov/statistics-stories/statistics.html), "17 people die each day waiting for an organ transplant".  Therefore, organ donation is extremely important and more research needs to be conducted to find ways to recruit more organ donors.  In these analyses, we use data from the [Organ Procurement and Transplantation Network](https://optn.transplant.hrsa.gov/data/) to investigate the affect that age and gender has on the number of living donors.  The goal is to see if we can predict how many living donors there most likely could be in a group of people given the ages and genders of people in this group.  This could provide insight into age groups and genders that can be better marketed to to gain more donors.  

## Business Question
_Can we predict the number of living organ donors based on age and gender?_
## Data Sources
1. Living Donors in the US by Donor Age

https://github.com/shannonpowelson/number-of-living-organ-donors-analysis/blob/main/Living_Donors_Recovered_in_the_U.S._by_Donor_Age.xlsm

This data set contains the number of living donors in each age group for each year.  It also contains the total number of living donors for each year.  This data was downloaded from the Organ Procurement and Transplantation Network.    

2. Living Donors in the US by Donor Gender

https://github.com/shannonpowelson/number-of-living-organ-donors-analysis/blob/main/Living_Donors_Recovered_in_the_U.S._by_Donor_Gender.xlsm

This data set contains the number of living donors for each gender for each year.  It also contains the total number of living donors for each year.  This data was downloaded from the Organ Procurement and Transplantation Network.   

3. Living Donor Data

https://github.com/shannonpowelson/number-of-living-organ-donors-analysis/blob/main/Living%20Donor%20Data.xlsm

This file contains the compiled living donor age and gender data.  It also contains the simple linear regression graphs, the multiple linear regression data, and two tables that were made for visualization purposes.  

## Data Analysis

For this analysis, our dependent variable will be the total number of living donors and the dependent variables will be each age group (<1, 1-5, 6-10, 11-17, 18-34, 35-49, 50-64, and 65+) and gender (male and female).  

### _Simple Linear Regression_
I first conducted simple linear regressions for each of the indepdent variables in order to explore the association between the independent variable and the total number of living donors (our dependent variable).  The following plots show the simple linear regression plots for the total number of living donors vs each independent variable.  The graph also contains the least squares line, the R-Squared value, and the linear trendline.   

![alt text](https://github.com/shannonpowelson/number-of-living-organ-donors-analysis/blob/main/SimpleLR-%3C1.png)

The least squares line shown in this graph is y = 667.56x + 4979.9.  The interpretation of this line is that an increase of 1 in the number of living donors aged less than one is associated with an increase of 667.56 total living donors.  This interpretation format can be referenced for the least squares lines for the following graphs. 

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

In the simple linear regression for the number of living donors less than 1 years old and the number of living donors 1-5 years old, 1.29% and 0.06% of the data fits the linear regression models.  Therefore, we are almost uncertain of an association between these age groups and the total number of living donors.  For 11-17 year olds, 16.82% of the data fits the linear regression model.  This certainty level rises dramatically for the 18-34 year olds group since 77.85% of the data fits the linear regression model.  Out of all of the age group independent variables, we are most certain of an association between the 35-49 year old age group and the total number of living donors since 78.87% of the data fits the linear regression model.  For age groups after this, the R-Squared values go back down and thus we become less certain of the association.  For 50-64 year olds, 50.38% of the data fits the linear regression model and for people older than 65, 7.55% of the data fits the linear regression model.  The 35-49 year old age group data therefore fits the linear regression model the best and we are most certain of the association between this age group and the number of living donors than we are for the other age groups. This would be interesting to investigate in future research.  For gender groups, 98.77% of the data for females fits the linear regression model, while 96.66% of the data for males fits the linear regression model.  Therefore, we have a high level of certainty of the association between these two variables the the number of living donors.   

### _Multiple Linear Regression_

I then conducted a multiple linear regression to see the combined association of each of these independent variables with the total number of living donors.  This was the overall equation:

Total number of living donors = 0.127 - 0.047(age < 1 year) - 0.04(age 1-5 years) - 0.024(age 6-10 years) - 0.058(age 11-17 years) - 0.028(age 18-34 years) - 0.028(age 35-49 years) - 0.028(age 58-64 years) - 0.028(age 65+ years) + 1.028(male) + 1.028(female)

These are some more key results from our multiple linear regression.
![alt text](https://github.com/shannonpowelson/number-of-living-organ-donors-analysis/blob/main/MultipleLR-ResultsTable.png)

The coefficients tell us how an independent variables is associated with the total number of living donors and the p-value tells us the probability that the association is not by chance.  If the p-value is less than 0.05, then it is statistically significant and we have evidence to suggest that the association exists.  As shown in the table above, the only associations that are statistically significant are for the female and male independent variables.  We can therefore say, when we control for the number of female living donors and the number of living donors in each age group, a 1 person difference in the number of male living donors is associated with a 1.0278 difference in the total number of living donors.  However, this association is nearly the same for females, so it appears that males and females have the same association with the total number of living donors.  For the gender groups that are not statistically significant (for example, the 35-49 year old age group), we can say that when we control for the gender and other age groups, the total number of living donors with people in this age group have on average a difference of 0.028 in the number of living donors.  The F-significance is not picture above, but it is the probability that none of the parameters that we used are significant.  The F-significance value for this multiple linear regression is 2.70974796960042E-91 which shows that our parameters are likely to be significant. The coefficients ultimately show that each age indpendant variable is associated with having a similar average difference in the number of living donors.  Our simple linear regression was able to reveal more important information.     

## Summary

Overall, these linear regression analyses showed that we cannot confidently predict the total number of living donors from age and gender.  The multiple linear regression showed that the coefficients of association for most of our independent variables are not statistically significant.  Therefore, we do not have enough evidence to suggest that these associations actually exist.  However, the linear regression analyses revealed two important findings.  From the simple linear regressions, it was evident that we are more certain of an association between some age groups than others.  We are more certain that the middle age groups, like the 35-49 year old age group is associated with the total number of living donors than the younger and older age groups.  Only 1.29% of the less than 1 age group data fits the linear regression model and only 7.55% of the 65+ age group data fits the linear regression model.  Meanwhile, 78.87% of the 35-49 year old age group data fits the linear regression model.  This is important for capturing new markets for organ donation.  The younger and older age groups are not closely associated with the total number of living donors and therefore marketing campaigns can target these markets in order to get more donors.  However, more research needs to be conducted to determine why these age groups have less donors.  Health status or organ development might be confounding variables.  Another important finding was from the multiple linear regression.  The coefficients from the multiple linear regression showed that females and males have almost the same association with the toal number of living donors.  This is important because it shows that marketing campaigns do not need to target one gender more than another since their contributions are very similar.  Thus, these findings are important because many people are in need of organ transplants, so any information that could enhance marketing campaigns and increase the number of living donors is vital. 
