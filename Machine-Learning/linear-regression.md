## Linear Regression

Linear regression is one of many regression models that originated in the field of statistics and now has applications in machine learning. It's a supervised learning technique to predict a real-value, such as income level, prices, or demand. The goal is to create a model from a training set of data that can accurately predict the value of the target variable when it's given a new, unseen data point.

The model that a regression algorithm tries to create is really a continuous function $f$ that maps the input variables ($X$) to an output (or target) variable ($Y$). Recall that with supervised learning techniques, the training set includes the "answer" for the target variable's value. This allows the algorithm to find the mathematical relationship ($f$) between the input variables and the target variable. That way, for future input variables $X$, you can apply $Y = f(X)$ to get a predictions for the value of $Y$.

There are many different techniques of regression analysis. Generally, they'll differ in their assumptions around parameters or how input variables relate to one another or the target variable. These different assumptions impact the format that the function $f$ can take. Linear regression assumes there's a linear relationship between the independent input variables and the target variable.

The simplest form of a linear regression model is when there's only one independent variable used to predict the target variable. This is called **linear regression with one variable** or **simple linear regression**. When there is more than one independent variable, it's called **linear regression with multiple variables** or **multiple linear regression**.

### Notation and Model Representation for Simple Linear Regression
As noted above, linear regression assumes a linear relationship between the independent input variables and the target variable, which restricts the form that the function \(f\) can take.

With simple linear regression, the form of the function is:

\\[
f(x_i) = \beta_0 + \beta_1x_i
\\]

Where:
- $(x_i, y_i)$ for $i=1 \ldots n$ is a training set of data with $n$ observations
- $x$ is the input variable (or independent variable, or feature), and $x_i$ is the input variable for the $i^{th}$ observation
- $X$ is the space of input values
- \\(y\\) is the target variable (or output variable, or label), and \(y_i\) is the target variable for the \(i^{th}\) observation
- \(Y\) is the space of output values

The Greek letter beta (\(\beta\)) is used for the parameters (also called weights or coefficients) for each input value. In the case where there's only one input variable, the equation forms a line with a y-intercept of \(\beta_0\) and slope of \(\beta_1\).

\(\beta_0\) is also called a bias coefficient. It's like the starting point for the value the model is predicting. If you're trying to predict the price of a car (\(y\)) based on its engine size (\(x\)), the value for \(\beta_0\) may be $2,000, since cars typically don't start with $0 value. This is the value the model assigns to a car before the engine size of that car is taken into consideration.

Here's an image of an example linear regression function. For certain values of \(\beta_0\) and \(\beta_1\), this function would create the red line based on the training set (blue points):

![Example of simple linear regression with one independent variable. A line approximately estimates the trend in the data set of points](https://en.wikipedia.org/wiki/File:Linear_regression.svg)

A change to \(\beta_0\) in this example would push the line up or down. A change to \(\beta_1\) would adjust the slope of the line.

### Model Representation for Linear Regression with Multiple Variables
When there's more than one input variable (you have multiple features as represented by columns in the training set), the linear regression function can be generalized. The formula below has observations \(i = 1 \ldots n\) in the training set and \(p\) input variables for each observation:

\[
f(x_i) = \beta_0 + \beta_{1}x_{i1} + \beta_{2}x_{i2} + \ldots + \beta_{p}x_{ip}
\]

### Linear Regression Cost Function
A **cost function** (also known as a loss function) calculates the degree of fit of a model against the given training set data. It's a quantitative way to measure the accuracy of the predictions made by the machine learning model compared to the actual values. In other words, the cost function defines what it means for a model to be a "good fit" to the data, and gives you a way to measure that fit.

There are different types of cost functions, but the most common one to use for linear regression problems is the **squared error function**, also called **mean squared error**. This function averages the sum of the squared differences between each prediction \(f(x_i)\) and the actual value \(y_i\). This difference is also called a **residual**. The general form is:

\[
\frac{1}{n} \displaystyle\sum_{i=1}^{n} (f(x_i) - y_i)^2
\]

Recall that for simple linear regression, the function \(f(x_i) = \beta_0 + \beta_1x_i \). You want \(\beta_0, \beta_1\) parameter values in your model so \(f(x_i)\) is close to \(y_i\) for all points in the training set \((x, y)\). The linear regression machine learning algorithm will try to find values for \(\beta_0, \beta_1\) in order to minimize the cost function.

### Minimizing the Cost Function Using Gradient Descent
**Gradient descent** is an iterative algorithm that finds the optima (minima or maxima) of a function. You can use it in linear regression to find the parameters \(\beta_0, \beta_1\) that minimize the cost function.

### Evaluating Linear Regression Models
[TO DO]

### Regularization
[TO DO]

### Other Considerations
Note that in machine learning, the term "regression" can refer to both a type of problem or to specific algorithms. Generally, regression problems predict real-valued output, like the price of a car based on its engine size and horsepower. But confusingly, some specific algorithms with "regression" in their name aren't always used for regression problems. For example, you typically use [logistic regression](../logistic-regression/index.md) for classification problems.

### Other Resources
- [Supervised learning](../supervised-learning/index.md)


