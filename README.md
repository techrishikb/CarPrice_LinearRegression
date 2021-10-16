# CarPrice_LinearRegression
# Simple Linear Regression
Simple Linear Regression is a model where we predict the value of an independent variable using the values of a dependent variable. Linear regression model is best describd using the linear equation of a line Y= mX+c."Y" is the dependent variable, "X" is the independent variable, "c" signifies the value of the dependent variable when the independent variable is equal to zero. "m" is the slope of the line describing, how much strong is the relation between "X" and "Y". That is what is the iuncrease in "Y"(dependent variable) with the increase in "X"(independent variable).

Among the multiple lines passing through the scattered data, we need to find the best fit line. The best-fit line is obtained by minimising a quantity called Residual Sum of Squares (RSS).

The strength of a linear regression model is mainly explained by R²,  where R² = 1 - (RSS / TSS)
RSS: Residual Sum of Squares
TSS: Total Sum of Squares. R-squared value tells us exactly how much variance in the data has been explained by the model. Suppose, the R-squared is about 0.816 which means that the model is able to explain 81.6% of the variance which is pretty good.

The new aspects to consider when moving from simple to multiple linear regression are:
# Overfitting:
As you keep adding the variables, the model may become far too complex
It may end up memorising the training data and will fail to generalise
A model is generally said to overfit when the training accuracy is high while the test accuracy is very low
# Multicollinearity
Multicollinearity refers to the phenomenon of having related predictor variables in the input dataset. In simple terms, in a model which has been built using several independent variables, some of these variables might be interrelated, due to which the presence of that variable in the model is redundant. You drop some of these related independent variables as a way of dealing with multicollinearity.

Two basic ways of dealing with multicollinearity
Looking at pairwise correlations
Looking at the correlation between different pairs of independent variables
Checking the Variance Inflation Factor (VIF)
Sometimes pairwise correlations aren't enough
Instead of just one variable, the independent variable might depend upon a combination of other variables
VIF calculates how well one independent variable is explained by all the other independent variables combined
The common heuristic we follow for the VIF values is:
> 10:  Definitely high VIF value and the variable should be eliminated.
> 5:  Can be okay, but it is worth inspecting.
< 5: Good VIF value. No need to eliminate this variable.
# Feature selection
Selecting the optimal set from a pool of given features, many of which might be redundant becomes an important task.


# Optimal Model Selection
To get the optimal model, you can always try all the possible combinations of independent variables and see which model fits the best. But this method is obviously, time-consuming and infeasible. Hence, you need some other method to get a decent model. This is where manual feature elimination comes in, where you:

Build the model with all the features
Drop the features that are least helpful in prediction (high p-value)
Drop the features that are redundant (using correlations and VIF)
Rebuild model and repeat

# MULTIPLE LINEAR REGRESSION


