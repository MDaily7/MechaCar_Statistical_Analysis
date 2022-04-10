# MechaCar Statistical Analysis
## Overview
## Results
### Linear Regression to Predict MPG
[Multiple Linear Regression Results](https://github.com/MDaily7/MechaCar_Statistical_Analysis/blob/main/Images/MechaCar_multiplelinear.png)
### Summary Statistics on Suspension Coils 
* [PSI Total Summary](https://github.com/MDaily7/MechaCar_Statistical_Analysis/blob/main/Images/PSI_Total_Summary.PNG) displays the mean, median, variance, and standard deviation of suspension coil PSI across all lots
* [PSI Lot Summary](https://github.com/MDaily7/MechaCar_Statistical_Analysis/blob/main/Images/PSI_lot_summary.PNG) displays the mean, median, variance, and standard deviation of suspension coil PSI by lot
### T-Tests on Suspension Coils
* [Total Mean T-Test](https://github.com/MDaily7/MechaCar_Statistical_Analysis/blob/main/Images/All_Lots_T-test.png)
* [Lot Mean T-Tests](https://github.com/MDaily7/MechaCar_Statistical_Analysis/blob/main/Images/Lot_T-tests.png)
## Summaries
### Linear Regression to Predict MPG
A multiple linear regression was performed to determine if mpg can be predicted by vehicle length, weight, spoiler angle, ground clearance, and all wheel drive capability. 
As can be seen in the results section, the intercept term explains a significant amount of variability in miles per gallon. Additonally, vehicle length and ground clearance
also provide non-random variance to mpg values in the dataset (p-values all significantly lower than 0.05). Surprisingly, vehicle weight does not seem to provide non-random 
variance to mpg with an approximate p-value of 0.08. The p-value of the multiple linear regression model is 5.35e-11 indicating that the slope of the linear model is not
considered to be zero. The r-squared value of the model is 0.7149 indicating that the model can predict mpg about 70% of the time; with this in mind, it seems that the model
does not predict mpg of MechaCar prototypes all that effectively especially considering that only two of the five variables provided significant effects to the variability in
mpg. The lack of significant variables may also indicate that that the model is overfitted which could potentially be artificially raising the r-squared value and mean that
model would not do well at predicting future data. 
### Summary Statistics on Suspension Coils 
According to the design specifications for MechaCar suspension coils, the variance of the coils must not exceed 100 pounds per square inch. In the Total Summary, it can be seen
that the standard deviation of all lots combined is 7.89 pounds per square inch which meets the specification. The Lot Summary shows that the standard deviation in pounds per square
inch is less than 100 for each of the lots individually as well. As a note, standard deviation is used here becuase it keeps the units pounds per square inch whereas variance
would be pounds per square inch squared. 
### T-Tests on Suspension Coils
Total Mean T-Test shows the results of the t-test comparing the mean PSI of all lots compared to a population mean of 1500psi. The p-value is 0.06 indicating that there is
not enough evidence to reject the null meaning the two means are not statistically different. Lot Mean T-Tests displays the results of the t-tests comparing the mean psi for
each lot to a population mean of 1500psi. Lot 3 is the only lot to have a p-value less than 0.05 (Lot3 p-value = 0.04) indicating that it is the only lot with a mean psi that
is statistically different from the population mean of 1500.
## Study Design: MechaCar vs Competition
For this study, the cost of MechaCar vehicles will be compared to the aggregated cost of competitor vehicles (competitors will not be divided by individual competitor). A 
two-sample t-test will be used to determine if the mean cost of MechaCar vehicles is significantly different than the mean cost of competitor vehicles. The two-sample t-test
is used becuase two samples with continuous data are being compared. The null hypothesis is that there is no difference in the means costs, and the alternative hypothesis is
that the mean cost of MechaCar vehicles is statistically different than the mean cost of competitor vehicles. To run the test, MechaCar vehicle costs and the costs of competitor
vehicles will need to be acquired. To make this study more informative, it may be beneficial to perform this test by vehicle type. For example, MechaCar suburban vehicle costs
compared to competitor suburban vehicle costs. 
## Resources
* R 4.1.3
* [Images](https://github.com/MDaily7/MechaCar_Statistical_Analysis/tree/main/Images)
* [RScript](https://github.com/MDaily7/MechaCar_Statistical_Analysis/blob/main/RScripts/MechaCarChallenge.R)
