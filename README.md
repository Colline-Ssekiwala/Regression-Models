# Regression-Models
## <a href="https://github.com/Colline-Ssekiwala/Regression-Models/blob/main/simple_linear_regression.ipynb">Simple Linear Regression</a>
<p>A simple linear regression in machine learning is a supervised learning algorithm that uses a single feature $(x)$ to predict a continuous target variable $(y)$ using a linear function.</p>
<p>A linear function is a function that can be written in the form:

$$y = ax + b$$

<p>where $a$ and $b$ are $constants$</p>
<p>$x$ is the $independent$ $feature$</p>
<p>$y$ is the $dependent$ $variable$</p>

<p>A linear function has a constant rate of change, meaning that the difference between any two output values is proportional to the difference between the corresponding input values. A linear function can be represented by a straight line on a graph, where the slope of the line $(Coefficient)$ is equal to $a$, and the $y-intercept$ is equal to $b$. A linear function can be used to model situations that have a constant rate of change, such as speed, distance, or cost.</p>

## <a href="https://github.com/Colline-Ssekiwala/Regression-Models/blob/main/Cmultiple_linear_regression.ipynb">Multiple Linear Regression</a>
<p>Multiple linear regression is a statistical technique that allows you to model the relationship between one continuous dependent variable and two or more continuous or categorical independent variables.</p>
<p>The formula for multiple linear regression is:</p>
<p>$$y = β0 ​+ β1​x1 ​+ β2​x2 ​+...+ βk​xk​$$
where:</p>

<p>$y$ is the $dependent variable$</p>
<p>$β0$​ is the $intercept$</p>
<p>$β1​,β2​,...,βk$​ are the $coefficients$ of the $independent variables$</p>
<p>$x1​,x2​,...,xk$​ are the $independent variables$</p>
<p>The coefficients $β0​,β1​,...,βk​$ are estimated using a method called ordinary least squares (OLS), which minimizes the sum of squared errors (SSE) between the observed and predicted values of $y$</p>
<code>print(regressor.predict([[1, 0, 0, 160000, 130000, 300000]]))</code>
**Important note 1:** Notice that the values of the features were all input in a double pair of square brackets. That's because the "predict" method always expects a 2D array as the format of its inputs. And putting our values into a double pair of square brackets makes the input exactly a 2D array. Simply put:

$1, 0, 0, 160000, 130000, 300000 \rightarrow \textrm{scalars}$

$[1, 0, 0, 160000, 130000, 300000] \rightarrow \textrm{1D array}$

$[[1, 0, 0, 160000, 130000, 300000]] \rightarrow \textrm{2D array}$

**Important note 2:** Notice also that the "California" state was not input as a string in the last column but as "1, 0, 0" in the first three columns. That's because of course the predict method expects the one-hot-encoded values of the state, and as we see in the second row of the matrix of features X, "California" was encoded as "1, 0, 0". And be careful to include these values in the first three columns, not the last three ones, because the dummy variables are always created in the first columns.

