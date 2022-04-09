# MechaCar Statistical Analysis
## Linear Regression to Predict MPG:  
### Linear Regression:
![](/Images/Linear_Regression_D1_5.png)
### Linear Regression Summary:
![](/Images/p-value_r-squaredValue_lm_D1_6.png)   
### Quesions:
1. Which variables/coefficients provided a non-random amount of variance to the mpg values in the dataset?
   - The vehicle_length and ground_clearance have p-values below the significance level of 0.05, indicating non-random variation in the data set.   
2. Is the slope of the linear model considered to be zero? Why or why not?
   - `p-value: 5.35e-11` is below the significance level of 0.05, indicating the slope is not zero.  
3. Does this linear model predict mpg of MechaCar prototypes effectively? Why or why not?
   - `R-squared:  0.7149` suggests 71% of the time the model will predict mpg, meaning a moderate to strong correlation.   

## Summary Statistics on Suspension Coils:   
### Total Summary:
![](/Images/Coil_Suspension_total_summary.png)
### Lot Summary:
![](/Images/Coil_Suspension_lot_summary.png) 

### Question:
1. The design specifications for the MechaCar suspension coils dictate that the variance of the suspension coils must not exceed 100 pounds per square inch. Does the current manufacturing data meet this design specification for all manufacturing lots in total and each lot individually? Why or why not?
   - Total Summary Variance is 62.3 and within design specs.
   - Lot Summary Variance for Lot 1 is .979 and within design specifications.
   - Lot Summary Variance for Lot 2 is 7.469 and within design specifications.
   - Lot Summary Variance for Lot 3 is 170.286 and **outside** design specifications.  

## T-Tests on Suspension Coils:
### All Lots and Lot1, Lot2, Lot3:
![](/Images/t_test_PSI_All_Lot1_Lot2_Lot3.png)

### Summary of T-Tests:
    - All Lots have a p-value = 0.060 and within the 95% confidence interval.
    - Lot1 has a p-value = 1 and within the 95% confidence interval.
    - Lot2 has a p-value = 0.607 and within the 95% confidence interval.
    - Lot3 has a p-value = 0.042 and **outside** the 95% confidence interval.  

## Study Design: MechaCar vs Competition:
### Plan a statistical study to compare performance of the MechaCar vehicles against performance of vehicles from other manufacturers:

1. What metric or metrics are you going to test?
   - A subset of consumers are interested in MSPR, City/Hwy MPG, and Safety Ratings.
2. What is the null hypothesis or alternative hypothesis?
   - Null hypothesis is that there is no difference between MechaCar vehicles and the Competition vehicles.  
   - Alternative hypothesis is that there is difference between MechaCar vehichles and the Competition vehicles.
3. What statistical test would you use to test the hypothesis? And why?
   - Linear regression model and p-test to compare MechaCar vehicles data to the competition vehicles data.
4. What data is needed to run the statistical test?
   - A statistically substantial data set for each the MechaCar vehichles and Competition vehicles.  
