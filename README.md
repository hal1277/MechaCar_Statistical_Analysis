# AutosRU: MechaCar

## Overview

AutosRU is having some manufacturing problems with their newest prototype MechaCar.  A statistical analysis needs to be done to help identify the issue so it can be corrected.  

## Results

## Linear Regression to Predict MPG

![Customers vs Subscribers](https://public.tableau.com/views/Module14ChallengeAssignment_16436792672500/NYCCitibikes?:language=en-US&:display_count=n&:origin=viz_share_link)

The linear regression tested the variables of vehicle length, vehicle weight, spoiler angle, ground clearance, and AWD to see their affect on efficiency (MPG).  The slope of the linear model is not exactly zero but is very close to 0.  The slope has a slight inverse relationship with ground clearance and vehicle lenth meaning that as the clearance and length increase the MPG decreases slightly.  For both of these variables the P value is below 0.05 meaning a high degree of confidence that these variables are having a non-random effect on the MPG.

This linear model does predict the MPG of MechaCar prototypes effectively.  This conclusion is supported by the R-squared value of 0.7149 which means that these variables explain 71% of the correlation and the p-value is well below 0.05 giving a high level of confidence that these results are repeatable and non-random.  

## Summary Statistics on Suspension Coils

It's important that the variance of suspendsion coils not exceed 100 PSI.  When looking at the total summary statistics the samples are within the tolerance specified with a variance of 62.2.

![Number of Rides per Bike](https://public.tableau.com/shared/NZ4PTGNWQ?:display_count=n&:origin=viz_share_link)

However, when looking at the individual lots it can be seen that the variance in Lot 1 and Lot 2 is actually much lower than 62.2 but the variance in Lot 3 is out of tolerance at 170.2.  

![Duration of Rides](https://public.tableau.com/shared/724S699YJ?:display_count=n&:origin=viz_share_link)

## T-tests On Suspension Coils 

![Rentals by Gender](https://public.tableau.com/shared/BNCQDKDR8?:display_count=n&:origin=viz_share_link)

Performing a t-test on a sample of 50 data points across all lots the p-value is higher than 0.05 so it is appropriate to reject the null hypothesis that true mean is equal to 1498.78.    

![Rentals by Time of Day](https://public.tableau.com/shared/P7Y6SWRQT?:display_count=n&:origin=viz_share_link)

Performing the t-test on each individual lot shows for Lot 1 and Lot 2 the null hypotheses cannot be rejected since the p-values are much lower than 0.05 but on Lot 3 the null hypothesis can be rejected becuase the p-value is much higher than 0.05.  This is an expected result since we say from the summary statistics that Lot 3 has some values that are too low relative to the tolerance level.  

## Study Design: MechaCar vs. Competition 

AutosRU would like to compare their vehicles against those of their competitors.  It would be useful to know how certain vehicle characteristics affect consumer purchases and therefore vehichle sales.  I recommend a statistical study to test the effect that the metrics of cost, fuel efficiency, maintenance costs, and safety rating have on the number of vehicles sold.  

The null hypothesis for this statistical test will be: Car sales are not higher for lower cost, higher efficiency, lower maintenance costs, and better safety ratings.  

The alternative hypothesis is: Car sales are higher for lower cost, higher efficiency, lower maintenance costs, and better safety ratings.  

A linear regression test will be best suited for this analysis since it allows the testing of multiple variables and can distinguish the effect that each has, or does not have, on the dependant variable of number of vehicles sold.  This will allow us to see if cost, efficiency, maintenance costs and safety ratings have a non-random effect on the number of vehicles sold.   

In order to perform this statistical analysis the following data will be necessary to acquire:
-sales volume by car by manufacturer
-cost by car 
-efficiency by car
-average maintenance costs by car
-safety ratings by car

## Results 

The statistical analysis that was performed on the MechaCar data shows there is an issue with the suspension coils produced in Lot 3.  The manufacturing team will now be able to use this info to investigate what occured during that speciic manufacturing process to prevent the issue from occuring again.  
