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
![alt_text](https://github.com/AndrealZhang/Analyzing_Factors_That_Impact_Snapchat_Election_Ad_Impressions/blob/master/regression_model2.png)

The R squared value is still around 60% and the significant F value decreased, meaning that there is a very high probability that the amount spent impacts the number of impressions. We can better visualize this relationship with a scatter plot.

![alt_text](https://github.com/AndrealZhang/Analyzing_Factors_That_Impact_Snapchat_Election_Ad_Impressions/blob/master/spending_vs_impressions_scatterplot.png)

## Summary and Implications
1. Regardless of political campaign, 60% of the number of implications can be predicted using this formula: number of impressions = 348.84(amount spent) + 67694
2.
