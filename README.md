# Linear Regression Model
Linear regression is a fundamental statistical and machine learning technique used for modeling the relationship between a dependent variable (target) and one or more independent variables (features or predictors). It is a supervised learning algorithm commonly employed for predictive analysis and understanding the linear relationship between variables.

# How Linear Regression Works
Linear regression aims to find a linear equation that best represents the relationship between the input features and the target variable

# Equation 
  Y = a + bX where : 
  - Y represents the predicted value of the target variable.
  - X represents the input feature(s).
  - a is the intercept (the value of Y when X is 0).
  - b is the slope (the change in Y for a unit change in X).


# Goal 
The goal of linear regression is to determine the optimal values of 'a' and 'b' such that the predicted values are as close as possible to the actual target values. This is typically done by minimizing the sum of squared differences between predicted and actual values

# Types of Linear Regression
There are several types of linear regression models, including:

Simple Linear Regression: Involves a single independent variable to predict a dependent variable.
Multiple Linear Regression: Utilizes multiple independent variables to predict a dependent variable.
Polynomial Regression: Extends linear regression to fit polynomial functions to the data, allowing for curved relationships.
Ridge Regression and Lasso Regression: Variations of linear regression that introduce regularization to prevent overfitting.

# Gradient Descent in Linear Regression
Gradient Descent is a fundamental optimization technique used to find the optimal parameters (coefficients) of a linear regression model

# How Gradient Descent Works
the cost function is typically defined as the Mean Squared Error (MSE), which is the average of the squared differences between predicted and actual values

                                                                 MSE = (1/n) * Σ(yᵢ - ŷᵢ)²
                                                                  
Gradient Descent works by iteratively adjusting the model's parameters (coefficients) to minimize this cost function. It calculates the gradient (slope) of the cost function with respect to each parameter and updates the parameters in the direction that decreases the cost

                                                                 θ = θ - α * ∂(MSE)/∂θ


                                                                
# Benefits of Gradient Descent
Gradient Descent offers several advantages in linear regression:

Efficiency: It is efficient for optimizing large datasets and high-dimensional feature spaces.
Flexibility: It can be used with various cost functions and is not limited to linear regression.
Convergence: With appropriate hyperparameter settings, it typically converges to a minimum point.

# Learning Rate
The learning rate is a crucial hyperparameter in the context of gradient-based optimization algorithms, such as Gradient Descent, used in linear regression and many other machine learning models. It significantly impacts the training process and the performance of your linear regression model

High Learning Rate lead to :
- Overshooting: When the learning rate is too high, the model may take excessively large steps during training. This can cause it to overshoot the optimal parameter values and result in instability.
- Divergence: In extreme cases, a very high learning rate can cause the training process to diverge completely. The loss may increase at each iteration instead of decreasing, leading to an unusable model.
![image](https://miro.medium.com/v2/resize:fit:552/1*69g-QzyJ_sRJ033Ydph9Ww.png)
Very Low Learning Rate:

- Slow Convergence: A very low learning rate will cause the model to update its parameters very slowly. This can result in extremely slow convergence, and the training process may require a large number of 
  epochs to reach a satisfactory solution, or it may get stuck in local minima.

- Getting Stuck: If the learning rate is too low, the model may get stuck in local minima or plateaus and struggle to escape from them.












