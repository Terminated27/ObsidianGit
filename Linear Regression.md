#prog 
Linear regression is a supervised [[machine learning]] algorithm used to predict a continuous target variable based on one or more independent variables. It assumes a linear relationship between the input variables (independent variables) and the output variable (dependent variable).

## Key Concepts and Keywords

- **[[Supervised Learning]]**: Linear regression is a [[supervised learning]] algorithm as it requires labeled training [[data]] with both input and output values.
- **Continuous Target Variable**: Linear regression predicts a continuous target variable, which means the output can take any numerical value within a given range.
- **Independent Variables**: Also known as features or predictors, these are the input variables used to predict the target variable.
- **Dependent Variable**: The target variable that we want to predict using linear regression.
- **Linear Relationship**: Linear regression assumes that there is a linear relationship between the independent variables and the dependent variable.

## Example

Let's consider an example where we want to predict housing prices based on the size of houses. We have collected [[data]] for various houses, including their sizes (in square feet) and corresponding prices (in dollars). Our goal is to build a linear regression model that can predict house prices based on their sizes.

```python
import numpy as np
from sklearn.linear_model import LinearRegression

# Input features (house sizes in square feet)
X = np.array([[1000], [1500], [2000], [2500], [3000]])

# Target variable (house prices in dollars)
y = np.array([50000, 75000, 100000, 125000, 150000])

# Create an instance of Linear Regression model
model = LinearRegression()

# Fit the model to our training data
model.fit(X, y)

# Predict house price for a new house with size 1800 square feet
new_house_size = np.array([[1800]])
predicted_price = model.predict(new_house_size)

print(f"Predicted price for a house with size 1800 square feet: ${predicted_price[0]}")
```

Output:
```
Predicted price for a house with size 1800 square feet: $90000.0
```

In this example, we first import the necessary libraries, including `numpy` for numerical operations and `LinearRegression` from `sklearn.linear_model` module. We then define our input features (`X`) and target variable (`y`) as numpy arrays.

Next, we create an instance of the Linear Regression model using `LinearRegression()` and fit it to our training [[data]] using the `fit()` method. This step involves finding the best-fit line that minimizes the sum of squared errors between predicted and actual values.

Finally, we can use the trained model to predict the price of a new house with a size of 1800 square feet by calling the `predict()` method on our model object. The predicted price is then printed to the console.

## Conclusion

Linear regression is a powerful algorithm for predicting continuous target variables based on one or more independent variables. It assumes a linear relationship between the input variables and the output variable. [[Python]] provides various libraries, such as scikit-learn, that make it easy to implement linear regression models efficiently.