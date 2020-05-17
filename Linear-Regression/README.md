### Project Overview

 In simple linear regression, we establish a relationship between the target variable and input variables by fitting a line, known as the regression line.

In general, a line can be represented by linear equation y = mx + by=mx+b. Where y is the dependent variable, x is the independent variable, m is the slope, b is the intercept.

Further, the residual could be modeled as the sum of the individual residual errors. You can interpret these errors as the individual errors due to wrong parameter estimation or error in the measurement of features.

**Linear** **Relationship**
According to this assumption, the relationship between response (Dependent Variables) and feature variables (Independent Variables) should be linear.

Why it is important?

Linear regression only captures the linear relationship, as it is trying to fit a linear model to the data.
How to validate it?

The linearity assumption can be tested using scatter plots.

**Little or No Multicollinearity Assumption
**What is multicollinearity?

It is assumed that there is little or no multicollinearity in the data. But what do we mean by multicollinearity? Well, multicollinearity occurs when independent variables in a regression model are correlated. This correlation is a problem because independent variables should be independent. If the degree of correlation between variables is high enough, it can cause problems when you fit the model and interpret the results.

Why sweat over multicollinearity?

The interpretation of a regression coefficient is that it represents the mean change in the dependent variable for each unit change in an independent variable when you hold all of the other independent variables constant. However, when independent variables are correlated, changes in one variable, in turn, shifts another variable/variable. The stronger the correlation, the more difficult it is to change one variable without changing another. It becomes difficult for the model to estimate the relationship between each independent variable and the dependent variable independently because the independent variables tend to change in unison.

Effects of multicollinearity

It results in unstable parameter estimates which makes it very difficult to assess the effect of independent variables.
Weakens the statistical power of the regression model
How to validate it?

Multicollinearity occurs when the features (or independent variables) are not independent of each other. Pair plots of features help validate.
You can also calculate the correlation coefficient (Pearson or Spearman) to figure out which features are correlated.
Treating multicollinearity

Remove some of the highly correlated independent variables.
Linearly combine the independent variables, such as adding them together.

**Homoscedasticity Assumption
**Homoscedasticity describes a situation in which the error term (that is, the “noise” or random disturbance in the relationship between the independent variables and the dependent variable) is the same across all values of the independent variables.

Why it is important:

Generally, non-constant variance arises in the presence of outliers or extreme leverage values.
How to validate:

The plot between error (residuals) vs predicted/fitted values. If there is no fan-shaped pattern visible, then it satisfies this assumption.
In the image below, shown are three different plots for residuals (True value - Predicted value) and Predicted value. Let's discuss these plots in detail:

The left two plots are instances of heteroscedasticity where the variance either increases (left plot) or decreases (right plot). So, it violates the assumption of constant variance.

The rightmost plot is an instance that satisfies the assumption of constant variance among the residuals.

The residual plot i.e. Residuals vs Predicted value plot should aspire to achieve the third plot for linear regression.



**Little or No autocorrelation in residuals
**There should be little or no autocorrelation in the data. Autocorrelation occurs when the residual errors are not independent of each other.

Why it is important:

The presence of correlation in error terms drastically reduces the model's accuracy. This usually occurs in time series models. If the error terms are correlated, the estimated standard errors tend to underestimate the true standard error.
How to validate:

Residual vs Time plot: Look for the seasonal or correlated pattern in residual values.
In the plot, two plots are shown where the regression line (right plot) deviates from the true trend. Hence, it is necessary to take care of it.

Normal Distribution of error terms
A common misconception about linear regression is that it assumes that the outcome Y is normally distributed. Actually, linear regression assumes normality for the residual errors \varepsilonε, which represent variation in Y not explained by the predictors.

Why it is important:

Due to the Central Limit Theorem, we may assume that there are lots of underlying facts affecting the process and the sum of these individual errors will tend to behave like in a zero-mean normal distribution. In practice, it seems to be so.
How to validate:

You can look at the QQ plot of the residuals. QQ plot is a scatterplot created by plotting two sets of quantiles against one another. For our case, we plot the residual quantiles against the theoretical quantiles corresponding to a normal distribution. If the QQ plot is a straight line, then we can infer that the errors follow a normal distribution.
You should observe a normal curve on plotting a histogram of the residuals.

Why you should care about these assumptions?

In a nutshell, your linear model should produce residuals that have constant variance and are normally distributed, features are not correlated with themselves or other features, etc. If these assumptions hold true, the OLS procedure (discussed in the next chapter) creates the best possible estimates for the coefficients of linear regression.

Another benefit of satisfying these assumptions is that as the sample size increases to infinity, the coefficient estimates converge on the actual population parameters.

We have a regression problem at hand and the different types of error metrics that can be used are:

Mean Absolute Error (MAE)
 Mean absolute error is nothing but the average of absolute values of these residuals

Root Mean Squared Error (RMSE)
Root mean Square Error (RMSE) is nothing but the square root of the mean/average of the squares of all the errors.
RMSE is very commonly used and makes for an excellent general purpose error metric for numerical predictions.
Compared to the similar Mean Absolute Error, RMSE amplifies and severely punishes large errors.
Residuals can be positive or negative as the predicted value underestimates or overestimates the actual value
Thus to just focus on the magnitude of the error we take the square of the difference as it's always positive
So you may wonder what is the advantage of RMSE when we could just take the absolute difference instead of squaring
RMSE severely punishes large differences in prediction. This is the reason why RMSE is powerful as compared to Absolute Error.
Evaluating the RMSE and tuning our model to minimize its results in a more robust model.


R-Squared
R-squared is a statistical measure of how close the data are to the fitted regression line i.e. it measures the goodness of fit of a straight line. It is also known as the coefficient of determination, or the coefficient of multiple determination for multiple regression.
It is a measure of the proportion of variability in the response that is explained by the regression model. 

Adjusted R-squared

To counter the issue of adding more independent variables, you should consider using the metric Adjusted R-squared instead of R-squared. Simply put it penalizes the model for adding irrelevant explanatory variables. 
**R-squared tells you how well your model fits the data points whereas Adjusted R-squared tells you how important is a particular feature to your model.**


### Learnings from the project

 You are a die hard Lego enthusiast wishing to collect as many board sets as you can. But before that you wish to be able to predict the price of a new lego product before its price is revealed so that you can budget it from your revenue. Since (luckily!), you are a data scientist in the making, you wished to solve this problem yourself. This dataset contains information on lego sets scraped from lego.com. Each observation is a different lego set with various features like how many pieces in the set, rating for the set, number of reviews per set etc. Your aim is to build a linear regression model to predict the price of a set.

Why solve this project ?
After completing this project, you will have the better understanding of how to build a linear regression model. In this project, you will apply the following concepts.

Train-test split
Correlation between the features
Linear Regression
MSE andR^2
R 2
Evaluation Metrics



