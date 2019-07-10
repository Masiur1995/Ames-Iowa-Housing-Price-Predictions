## Problem Statement

For stakeholders that intend on buying or selling houses in Iowa, you've come to the right place! Here we have an analysis on homes in Iowa ready for you to understand which features and aspects to consider when buying/selling your house!


## Data Cleaning and Data Exploratory Analysis

Our initial step in data cleaning was to examine null values and understand what to do with them. For different kinds of datatypes, we imputed different kinds of values. For our numerical values, we imputed numerical zeroes. This was to avoid imputing outliers into our data if we had incorporated the mean or median. For our nominal categorical values, we assigned the entirety of its structure to a one hot encoded variable as dummy variables so that their input towards analyzing the data is numerical, rather than as objects. As for our ordinal categories, we assigned a ranking system with numbers so they could have an input when we analyze the dataset as a whole. 

During our data exploratory, we noticed that the distribution of the saleprice was not normal. For this matter we got rid of outliers. The two categories with outliers that we removed were from ground level area and lot area. Now our data doesn't look so skewed so we don't have to look at other variables to remove outliers or we can just deteriorate our data.

We established this as a problem requiring a regression model and therefore, we provided three regression models (Linear Regression, Ridge Regression, and Lasso Regression. Our target variable was saleprice and we were trying to understand the variance/bias for each model, as well as which model provided the best predictions.  For each model, we analyzed their mean-squared-error and their R-squared score. These are metrics that explained and concluded which model was the best fit for our analysis.

## Conclusion

Our Ridge Regression model produced a higher robust R-squared value than our Lasso Regression model and therefore, we will use the Ridge Regression model to help explain our data. The variance in our Ridge regression model is high however, it can be explained by our predictions.