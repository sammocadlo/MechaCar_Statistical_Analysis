# MechaCar_Statistical_Analysis

## Linear Regression to Predict MPG

R Script was used to perform a linear regression model on several coefficients of the data - the result of this is shown below.

![image](https://user-images.githubusercontent.com/105682444/195220073-53833b98-7dd8-4848-9ac5-1be80208e0cd.png)

1. Which variables/coefficients provided a non-random amount of variance to the mpg values in the dataset?
  Coefficients:
  mpg: 0 < .05, statistically significant, non-random amount of variance
  vehicle length: 0 < .05, statistically significant, non-random amount of variance
  vehicle weight: .08 > .05 not statistically significant, random amount of variance
  spoiler angle: .31 > .05 not statistically significant, random amount of variance
  ground clearance: 0 > .05 statistically significant, non-random amount of variance
  AWD: .19>=.05 not statistically significant, random amount of variance
  
2. Is the slope of the linear model considered to be zero? Why or why not?
  Converting from scientific notation, all of the slopes of the variables are shown to be non-zero even though some are close to zero.

3. Does this linear model predict mpg of MechaCar prototypes effectively? Why or why not?
  R-squared is .7149, which shows a strong correlation for the dataset and shows this is an effective dataset to help predict the mpg of the MechaCar         prototypes.
  
## Summary Statistics on Suspension Coils

Below is the summary statistics of all the manufacturing lots -

![image](https://user-images.githubusercontent.com/105682444/195220844-bb7303b8-e9d5-4aea-8423-2557a7690a00.png)

And an image showing the results by lot -

![image](https://user-images.githubusercontent.com/105682444/195221018-0e741535-3c97-4bb6-a412-2b169b71258f.png)

1. The design specifications for the MechaCar suspension coils dictate that the variance of the suspension coils must not exceed 100 pounds per square inch. Does the current manufacturing data meet this design specification for all manufacturing lots in total and each lot individually? Why or why not?
  The variance for the total manufacturing lot is 62 < 100, which is within the expected design specifications of staying under 100 PSI. However, when reviewing the data by Lot number, Lot 3 is a large contributing factor to the variance being high.
  
## T-Tests on Suspension Coils

Lot Tests for all 3 lots are shown below -

![image](https://user-images.githubusercontent.com/105682444/195221132-0daa15d7-f0b2-42db-9ab2-ecead3b8a831.png)

The overall manufacturing, Lot 1, and Lot 2 show a normal distribution. Therefore, there is not sufficient evidence to reject the null hypothesis, which shows the two means are statistically similar.

## Study Design: MechaCar vs Competition

When comparing MechaCar to its competitor’s other metrics that could be of interest to a consumer could include cost, fuel efficiency, horsepower, or safety rating.

 1. What metric or metrics are you going to test?
    The next metrics to test should be the safety rating, horsepower, and fuel efficiency, which address some safety concerns of consumers.

 2. What is the null hypothesis or alternative hypothesis?
    The null hypothesis is that the mean of the safety rating is zero. The alternative hypothesis is that the mean of the safety rating is not zero.

 3. What statistical test would you use to test the hypothesis? And why?
    Using a multiple linear regression statistical summary would show how the variables impact the safety ratings for MechaCar and their competitors.

 4. What data is needed to run the statistical test?
    A random sample of n > 30 for MechaCar and their competitor, would need to be collected including the safety ratings,fuel efficiency, and  horsepower plus running the data through RStudio.
