# MechaCar_Statistical_Analysis

## Deliverable 1: Linear Regression to Predict MPG

![Deliverable1_1](https://user-images.githubusercontent.com/99096376/172055862-9d27d0be-bd28-4c0c-b09d-5b1f079c2ca1.png)
![Deliverable1_2](https://user-images.githubusercontent.com/99096376/172055869-00f291f9-000b-4349-b85c-e18bb614f44b.png)

After running each test we can see that:
- The vehicle length, and vehicle ground clearance are statistically likely to provide non-random amounts of variance to the model. That is to say, the vehicle length and vehicle ground clearance have a significant impact on miles per gallon on the MechaCar prototype. Conversely, the vehicle weight, spoiler angle, and All Wheel Drive (AWD) have p-Values that indicate a random amount of variance with the dataset.
- The p-Value for this model, 5.35e-11, is much smaller than the assumed significance level of 0.05%. This indicates there is sufficient evidence to reject our null hypothesis, which further indcates that the slope of this linear model is not zero.
- This linear model has an r-squared value of 0.7149, which means that approximately 71% of all mpg predictions will be determined by this model. Relatively speaking, his multiple regression model does predict mpg of MechaCar prototypes effectively.

## Deliverable 2:Summary Statistics on Suspension Coils

Total Summary

![Deliverable 2_Total_Summary](https://user-images.githubusercontent.com/99096376/172056057-c4133008-109c-42c0-88f9-54a73f079875.png)

Lot Summary

![Deliverable 2_Lot_Summary](https://user-images.githubusercontent.com/99096376/172056070-1de5b769-ea2e-49b5-aba5-5214afd431c6.png)

While the overall variance, as shown in the Total Summary data above, is under 100 psi and meets specifications, there is a problem with one of the individual lots. As shown in the Lot Summary stats, the variance for Lot 3 is well over the acceptable threshold, at 170.28.

## T-Tests on Suspension Coils

### Summary T-Test

![Deliverable 3_TTest_Total](https://user-images.githubusercontent.com/99096376/172056466-588e26ea-7458-46a0-896b-23604c0138df.png)

From here we can see the true mean of the sample is 1498.78, which we also saw in the summary statistics above. With a p-Value of 0.06, which is higher than the common significance level of 0.05, there is NOT enough evidence to support rejecting the null hypothesis. That is to say, the mean of all three of these manufacturing lots is statistically similar to the presumed population mean of 1500.


### Individual Lots

![Deliverable 3_TTest_All](https://user-images.githubusercontent.com/99096376/172056704-cae42407-e59e-4a4c-a032-7e1e82bd5395.png)

Lot 1 sample actually has the true sample mean of 1500, again as we saw in the summary statistics above. With a p-Value of 1, clearly we cannot reject (i.e. accept) the null hypothesis that there is no statistical difference between the observed sample mean and the presumed population mean (1500).

Lot 2 has essentially the same outcome with a sample mean of 1500.02, a p-Value of 0.61; the null hypothesis cannot be rejected, and the sample mean and the population mean of 1500 are statistically similar.

However, Lot 3, not surprisingly is a different scenario. Here the sample mean is 1496.14 and the p-Value is 0.04, which is lower than the common significance level of 0.05. All indicating to reject the null hypothesis that this sample mean and the presumed population mean are not statistically different

## Study Design: MechaCar vs Competition

The plan is to design the MechaCar vehicle to perform better than the general marketplace vehicles. To accomplish this goal atttention is best served improving the fuel efficiency of the MechaCar. Data needs to be gathered for all MechaCar manufacturing designs, in addition to the current six variables from this analysis. Additional data could include weather conditions, i.e. wind sheer, rain, heat, etc. Varying distances of short trips and long trips are also needed to determine fuel efficiency, as well as fuel efficiency over time. The dataset must include general marketplace competitor's data for comparison

What is the null hypothesis or alternative hypothesis?
HO: There is no statistical difference between the competition's mpg dataset and MechaCar's mpg dataset.

Ha: The true mean of MechaCar's mpg is greater than the mean of the competitor's mpg.

What statistical test would you use to test the hypothesis? And why?
I reccomend using the t-test to compare our dataset with the competitors. The t-test has already been used for this current analysis and provided the predictions needed to take the next steps for improvement.

What data is needed to run the statistical test?
The p-value would be set at 0.05. Data that results in a prediction of a p-value smaller than 0.05 would provide predictive evidence that the null hypothesis could be rejected and state that the Ha is true. Providing evidence that the Ha is true would also predict that the MechaCar provides consistently better fuel efficiency than the competitors mpg. There is always room for error and better fuel efficiency may not happen all of the time, but at least 95% of the time.
