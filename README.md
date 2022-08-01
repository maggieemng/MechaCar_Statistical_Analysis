# MechaCar_Statistical_Analysis
## Project Overview

The purpose of the project is analyze metrics (such as: vehicle length, weight, spoiler angle, ground clearance, AWD capabilities, MPG, and PSI) that could  affect the manufacturing a new car prototype. And then later on compare vehicle performance across different manufacturer lots. 

## Linear Regression to Predict MPG

Q: Which variables/coefficients provided a non-random amount of variance to the mpg values in the dataset? 
- The 4 variables are: vehicle length, vehicle weight, spoiler angle, and ground clearance. The data was continuous. AWD data was excluded as it is either true or false and categorical, which means that it is not suited for linear regression analysis.

Q: Is the slope of the linear model considered to be zero? Why or why not? 
- The slop of the linear model is not zero because the p-value is 2.277x10-11. This value is much smaller than a typical assumed significance level of 0.05%. Because of this, we reject the null hypothesis and conclude that the slope of the model is not zero. 

Q: Does this linear model predict mpg of MechaCar prototypes effectively? Why or why not? 
- The model is somewhat accurate with a R value or confidence level of 70% accuracy. This means in the future prediction, there's about a 70% chance that our prediction will be correct. We can say that factors in length, and ground clearance for MechaCar prototype models have a greater impact to MPG. MechaCar Vehicles' spoiler angle and weight in our prototype data reveals these 2 factors do not correlate to MPG.

## Summary Statistics on Suspension Coils

Manufacturing lot 1 has a much more uniform production result compared to lot 3, which has the highest range of variance and standard deviation. MechaCar's spec dictates that the variance can not exceed 100 PSI, so lot 3 having a 220 PSI variance fails the test. While Lot 1 and lot 2 are within acceptable ranges, (1.15 and 10.1 PSI). Overall, Lot 1 and Lot 2 are both within design specifications and have hnearly the same exact mean and median; while Lot 3 shows the most variance and exceeds the manufacturers specs.

## T-Test on Suspension Coils
<img src="https://github.com/maggieemng/MechaCar_Statistical_Analysis/blob/main/Resources/t-test.PNG">
</p>
The above screenshot shows the t-test done on the entire lot. After generating a t-test on suspension coils, we can see that the sample data has a high p value much higher than the commonly accepted .05. We fail to reject the null hypothesis since the p-value equals 0.06.

### T-Test on Three Smaller Lots
<img src="https://github.com/maggieemng/MechaCar_Statistical_Analysis/blob/main/Resources/lots_t_test.PNG">
</p>
I've also done a t-test on the 3 lots separately. 

## Study Design: MechaCar vs. Competition

We can also perform a linear regression on city and highway fuel efficiency to analyze MechaCar's standing against its competition. As gas prices rise, it is a growing factor in the car purchasing process. The metrics that can be included in this analysis are:
- City and highway fuel efficiency: dependent variable
- Horse power: independent variable
- MPG: independent variable In addition to the MPG, AWD, and vehicle weight data that we already have, we would have to collect fuel efficiency and horse power data for the sample data set at hand.
