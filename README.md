# Analyzing_Factors_That_Impact_Snapchat_Election_Ad_Impressions
## Background
What factors affect the number of impressions an advertisement receives? Looking at the 2020 election advertisements in the US regardless of political platform from [Snapchat](https://www.snap.com/en-US/political-ads/), we can predict this using regression analysis. Specifically, I looked at these factors:
1. Duration 
2. Targeted Gender (if a specific gender was targeted)
3. Targeted Age (if a specific age group was targeted)
4. Amount Spent 

## Multiple Regression
To find the relationship between these variables and impression, I conducted a multiple regression analysis.

![alt_text](https://github.com/AndrealZhang/Analyzing_Factors_That_Impact_Snapchat_Election_Ad_Impressions/blob/master/Multi_regression_model1.png)

The R squared value means that around 60% of the data can be displayed using this model. The significance F, the probability that none of the variables matter, is very small, meaning that the model is pretty accurate. However, the p-values for targeted age group, duration, and targeted gender are greater than 0.05, making these variables statistically insignificant. This means that we must run this model again with only the amount spent variable to get a more accurate model. 

## Linear Regression
