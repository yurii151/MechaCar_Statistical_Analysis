# MechaCar_Statistical_Analysis

## Linear Regression to Predict MPG

The liner regression I used to find what variables mattered is as followed:

<img width="606" alt="Screen Shot 2022-02-15 at 4 08 56 PM" src="https://user-images.githubusercontent.com/92888170/154387845-97e79052-5238-4c83-ba5c-2b5f6824c150.png">

As shown above, vehicle length and ground clearacne are both non random amount of variance to the mpg values in the data set. This is because they are both nearly zero. The p-value of this linear regressino is shown at the bottom of the screenshot is 5.35e-11. This is much smaller than .05. So, this is an sitaution where we can reject the null hypothesis. This proves that the slope of the linear model is not zero. The r-squared value of the regession is .7149, so I would say that the model is a good indicator of mpg. 

## Summary Statistics on Suspension Coils

The summary table of all of the suspension coils regardless of what Lot they were made in looks like this:

<img width="606" alt="Screen Shot 2022-02-17 at 3 24 01 PM" src="https://user-images.githubusercontent.com/92888170/154589948-8612d51f-29ca-4089-963a-a07e1a197835.png">

At first glance, it seems like everything is all good! The total variance of the group is 62.29356, which is less than the maximum variance of 100. While this is all well, we should dig deeper to see if there is any differences in the lots causing the over trends of the group. 

The summary break down of each lot is below:

<img width="606" alt="Screen Shot 2022-02-17 at 3 48 01 PM" src="https://user-images.githubusercontent.com/92888170/154590718-267a9ee3-448f-43cf-99c3-803ac663a3d2.png">

The mean of Lot1 is 1500, the median of Lot1 is 1500, the variance is 0.9795918 and the standard deviation is 0.9897433.
The mean of Lot2 is 1500.20, the median of Lot1 is 1500, the variance is 7.4693878 and the standard deviation is 2.7330181.
The mean of Lot3 is 1496.14, the median of Lot1 is 1498.5, the variance is 170.2861224 and the standard deviation is 13.04937253.

Lots 1 and 2 seem fine, as there is very little variance compared to the threshold of 100 that the manufactuarer requires. However, looking at lot 3, there is some cause for concern. The variance is around 170 which is way over the accepted amount of variance. Also, considering the high standared deviation, I would say that there is a huge differnce in the coils being produced in this lot so I would look into this if I were the manufacturer.

## T-Tests on Suspension Coils
T-testing over the entire population of suspension coils, the results are below:

<img width="606" alt="Screen Shot 2022-02-17 at 4 06 34 PM" src="https://user-images.githubusercontent.com/92888170/154592539-e3174a48-4740-4bff-ac8e-918f1500641a.png">

The results of the t-test show that mean of the sample is 1498.78, which is the same result as the summary table above. The p-value = 0.06028, which is above the threshold of 0.05, so that indicates that the mean of all three lots together is statisctially similar to the population mean (1500).


T-testing over the entire population of just lot1, the results are below:

<img width="606" alt="Screen Shot 2022-02-17 at 4 16 31 PM" src="https://user-images.githubusercontent.com/92888170/154593434-fe2c5487-0cb1-44c0-a42c-5c05041e56e8.png">

The results of the t-test show that mean of the sample is 1500, which is the sameple mean of Lot1. The p-value = 1, which is above the threshold of 0.05, so that indicates that the mean of Lot1 is statisctially similar to the population mean (1500).

T-testing over the entire population of just lot2, the results are below:

<img width="606" alt="Screen Shot 2022-02-17 at 4 20 47 PM" src="https://user-images.githubusercontent.com/92888170/154593807-ffa3a025-fdeb-4042-af63-ccf6e5bdac83.png">


The results of the t-test show that mean of the sample is 1500.02, which is the sameple mean of Lot2. The p-value = 0.6072, which is above the threshold of 0.05, so that indicates, much like Lot1, that the mean of Lot2 is statisctially similar to the population mean (1500).


T-testing over the entire population of just lot3, the results are below:

<img width="606" alt="Screen Shot 2022-02-17 at 4 26 57 PM" src="https://user-images.githubusercontent.com/92888170/154594299-cfa96e91-ee5b-4540-b060-5c6b79044caf.png">

The results of the t-test show that mean of the sample is 1496.14. The p-value = 0.04168, which is below the threshold of 0.05, so that indicates that the mean of Lot3 is NOT statisctially similar to the population mean (1500). Clearly, something has gone wrong in Lot3 and as stated before, will need to be investigated to see what went wrong.


