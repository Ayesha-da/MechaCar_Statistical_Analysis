# MechaCar_Statistical_Analysis
## Overview
To review the production data for insights that may help the manufacturing team overcome production troubles that are blocking the manufacturing team’s progress.
## Linear Regression to Predict MPG
![lm](https://user-images.githubusercontent.com/84524153/133928297-a261dd4c-f24d-4d2c-be1b-00c8d9771064.png)
![lm-summary](https://user-images.githubusercontent.com/84524153/133928314-8aa404ab-5aff-4eb5-9de4-abc7217b5f08.png)

- Which variables/coefficients provided a non-random amount of variance to the mpg values in the dataset?
 
  The **vehicle length**, and **vehicle ground clearance** provided a non-random amount of variance to the mpg values in the dataset.T values are relatively far away from zero       which indicate a relationship exists and these two variables have significant impact on mpg.
  
- Is the slope of the linear model considered to be zero? Why or why not?
 
  The **p-value: 5.35e-11** is much smaller han the assumed significance level of 0.05%.This indicates there is sufficient evidence to reject null hypothesis and the slope of     the linear model is not zero.

- Does this linear model predict mpg of MechaCar prototypes effectively? Why or why not?

  This linear model has **R-squared:  0.7149**, which means that approximately 71% of all mpg predictions will be determined by this model. This model  predict mpg of              MechaCar prototypes effectively.
 

## Summary Statistics on Suspension Coils
##### Total manufacturing lot
![total-summary](https://user-images.githubusercontent.com/84524153/133928986-9ec9b213-a84b-45c7-92ac-0d247c4921a1.png)
##### Individual manufacturing lot
![lot-summary](https://user-images.githubusercontent.com/84524153/133928995-ce3d2959-cfe4-4e45-b16e-50c39bf97268.png)

- The design specifications for the MechaCar suspension coils dictate that the variance of the suspension coils must not exceed 100 pounds per square inch. Does the current manufacturing data meet this design specification for all manufacturing lots in total and each lot individually? Why or why not?

The Variance for entire manufacturing lot is 62.293 which meets the current manufacturing design specification. The Variance for Lot1 is 0.9795 and Lot2 is 7.4693 and these two lots also meet the design specification. However Variance for Lot3 is 170.286 which exceeds the limit of 100 pounds per square inch and therefore Lot3 of suspension coils may not be accepted.


## T-Tests on Suspension Coils

![t-test](https://user-images.githubusercontent.com/84524153/133929002-00ec904b-4391-45cc-b08c-6247859e12b8.png)

#### Individual lots
![t-test-per-lot](https://user-images.githubusercontent.com/84524153/133929007-3436b462-4b69-4c09-9bef-09bc670be13e.png)

A T-test can be used to compare the mean of a sample to the population or the difference between population means.The null hypothesis assumes that there is no meaningful difference between the two means.Therefore the goal of the T-test is to reject the null hypothesis.

Here we can see  mean of the sample is 1498.78 with a p-Value of 0.06, which is higher than the common significance level of 0.05, there is NOT enough evidence to  reject
the null hypothesis. That is to say, the mean of all three of these manufacturing lots is statistically similar to the presumed population mean of 1500.

#### Individual lots
- Lot 1 has sample mean of 1500,with a p-Value of 1 and so we don't have enough evidence to reject the null hypothesis and so there is no statistical difference between the observed sample mean and the presumed population mean (1500).
Lot 2 has  sample mean of 1500.02, with a p-Value of 0.61 and so the null hypothesis cannot be rejected, and the sample mean and the population mean of 1500 are statistically similar.
Lot 3 however has the sample mean of 1496.14 and the p-Value is 0.04, which is lower than the common significance level of 0.05 indicating to reject the null hypothesis and so there is a statistical difference between the sample mean and the population mean.The suspension coils from this lot need to be inspected to remove those not meeting quality criteria.

## Study Design: MechaCar vs Competition
