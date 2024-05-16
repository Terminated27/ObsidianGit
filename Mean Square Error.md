#stats #prog #info 

Mean Square Error (MSE) is a commonly used metric to measure the average squared difference between the predicted values and the actual values in regression analysis. It provides a quantitative measure of how well the model fits the [[data]].

## Definition

The Mean Square Error is defined as the average of the squared differences between the predicted values $\hat{y}_i$ and the actual values $y_i$:

$$
MSE = \frac{1}{n} \sum_{i=1}^{n} (\hat{y}_i - y_i)^2
$$

where $n$ is the number of [[data]] points.

## Theorem 1: Bias-Variance Decomposition

The expected value of MSE can be decomposed into three components: bias, variance, and irreducible error. This decomposition helps us understand different sources of error in a model.

$$
E[MSE] = \text{Bias}^2 + \text{Variance} + \text{Irreducible error}
$$

- **Bias** measures how far off, on average, are our predictions from the true values. A high bias indicates an underfitting model that oversimplifies the [[data]].
- **Variance** measures how much our predictions vary for different training sets. A high variance indicates an [[overfitting]] model that is too sensitive to noise in the [[training data]].
- **Irreducible error** represents the inherent noise or randomness in the [[data]] that cannot be reduced by any model.

## Theorem 2: Relationship with Variance

The MSE can be decomposed into two components related to variance:

$$
MSE = \text{Var}(\hat{y}) + \text{Bias}^2(\hat{y}, y)
$$

where $\hat{y}$ represents the predicted values and $y$ represents the true values.

This theorem shows that the MSE is the sum of the variance of the predicted values and the squared bias between the predicted values and the true values.

## Example

Consider a simple [[linear regression]] model with one independent variable $x$ and a target variable $y$. We want to estimate the relationship between $x$ and $y$ using a [[linear]] function $\hat{y} = \beta_0 + \beta_1 x$, where $\beta_0$ and $\beta_1$ are the intercept and slope coefficients, respectively.

Suppose we have a dataset with $n$ observations $(x_i, y_i)$. The objective is to find the optimal values of $\beta_0$ and $\beta_1$ that minimize the MSE.

The steps to compute MSE in this example are as follows:

1. Fit the [[linear regression]] model by estimating $\hat{y}_i = \hat{\beta}_0 + \hat{\beta}_1 x_i$.
2. Calculate the residuals for each observation: $e_i = y_i - \hat{y}_i$.
3. Compute the Mean Square Error using:

$$
MSE = \frac{1}{n} \sum_{i=1}^{n} e_i^2
$$

4. Interpret and analyze the MSE value obtained.

By minimizing MSE, we can obtain optimal estimates for $\beta_0$ and $\beta_1$, leading to a better fit of our model to the [[data]].

## Conclusion

Mean Square Error is a valuable metric in regression analysis that quantifies how well a model fits observed [[data]]. It provides insights into bias, variance, and irreducible error components, allowing us to understand different sources of error in our models. By minimizing MSE, we can improve our models' [[performance]] and make more accurate predictions.