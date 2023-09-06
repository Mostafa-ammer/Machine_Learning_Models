# Logistic Regression Model 

Logistic regression is a fundamental and widely used statistical technique in machine learning and statistics for binary and multi-class classification problems. Despite its name, it is a classification algorithm, not a regression algorithm. Logistic regression models the probability that a given input belongs to a particular category or class. It is particularly useful when you need to predict the probability of an event occurring, such as whether an email is spam or not, whether a customer will make a purchase, or whether a patient has a particular medical condition.

# How get sigmoid from Odds 

In logistic regression, we model the odds of an event occurring. The odds of an event happening is defined as the ratio of the probability of the event occurring to the probability of it not occurring. Mathematically, the odds (OR) can be expressed as:

                                                          Odds= P(event)/1−P(event)
                                                                        

To model the relationship between the input features and the log-odds, logistic regression applies a logit transformation. The logit transformation takes the natural logarithm (base e) of the odds
​      

                                                          logit(P(event))=ln( P(event) /1−P(event))



  # Sigmoid Function

  The sigmoid function, also known as the logistic function, is used to transform the logit (log-odds) into a probability between 0 and 1

                                                        P(event)= 1 / 1+e pow(- logit)


 The sigmoid function maps any real-valued number (the logit) to a value between 0 and 1, representing the probability of the event occurring. If the logit is very large (positive), the probability is close to 1, and if the logit is very small (negative), the probability is close to 0. When the logit is 0, the probability is 0.5.

​![Alt text](https://th.bing.com/th/id/R.1e57c046e521fa3dd1d93fdc28fcae09?rik=cKAknoKsD0tpDg&pid=ImgRaw&r=0)


# Cost function 

- MSE is typically used for regression problems where the goal is to predict a continuous target variable. Logistic regression, on the other hand, deals with binary or multi-class classification problems where the 
  output is a probability (between 0 and 1) of belonging to a particular class
- MSE is not suitable for modeling probabilities because it does not enforce the necessary constraints on predicted probabilities.
- The MSE loss function is non-convex and non-smooth when applied to logistic regression. This means that optimization algorithms may have difficulty finding the global minimum, leading to convergence issues and suboptimal results

​![Alt text](https://th.bing.com/th/id/OIP.Mcij1eXbWrxWe2IpBNNkrAAAAA?pid=ImgDet&rs=1)


## How solve Proplem 

the logistic loss (cross-entropy loss) is the preferred choice for logistic regression because it is specifically designed for binary and multi-class classification problems, encourages the model to output probabilities, is convex and smooth, and aligns with standard classification evaluation metrics

In logistic regression, the cost function, also known as the loss function or log-likelihood function, is used to quantify how well the model's predicted probabilities match the actual binary labels in the training data. The goal of logistic regression is to minimize this cost function during training. The specific cost function used in logistic regression is called the "logistic loss" or "cross-entropy loss."
## Cost Function in Logistic Regression

The cost function, also known as the loss function or log-likelihood function, in logistic regression is used to measure the discrepancy between the predicted probabilities and the actual binary labels. The logistic regression cost function, often referred to as the "logistic loss" or "cross-entropy loss," is defined as follows:

For binary classification with classes 0 and 1:

- If the actual label is 1:
  \[ \text{Cost}(y, \hat{y}) = -\log(\hat{y}) \]

- If the actual label is 0:
  \[ \text{Cost}(y, \hat{y}) = -\log(1 - \hat{y}) \]

Where:
- \( y \) is the true binary label (0 or 1).
- \( \hat{y} \) is the predicted probability that the example belongs to class 1.

The overall cost function for logistic regression is the average (or sum) of these individual costs across all training examples, and it is used as the basis for training the logistic regression model.

The goal during training is to find the set of model parameters that minimizes this cost function, typically accomplished using optimization algorithms like gradient descent.


The overall cost function for logistic regression is the average (or sum) of these individual costs across all training examples. If you have a training dataset with \( N \) examples, the cost function \( J(\theta) \) (where \( \theta \) represents the model parameters, including the coefficients) is typically defined as:

\[ J(\theta) = \frac{1}{N} \sum_{i=1}^{N} \left[ -y^{(i)} \log(\hat{y}^{(i)}) - (1 - y^{(i)}) \log(1 - \hat{y}^{(i)}) \right] \]

# Benfits of using Log Loss 

- Probabilistic Interpretation: Log loss provides a probabilistic interpretation of the model's predictions. Instead of just binary classifications (0 or 1), logistic regression outputs probabilities between 0 and 
  indicating the confidence or likelihood of an example belonging to a particular class. This is valuable for understanding the model's uncertainty and making informed decisions.

- Continuous and Smooth Loss Function: Log loss is continuous and smooth, which makes it suitable for optimization using gradient-based algorithms like gradient descent. Smoothness ensures that small changes in 
  model parameters result in continuous changes in the loss, aiding convergence during training.

- Well-Behaved Gradient: Log loss has a well-behaved gradient, which simplifies the optimization process. The derivative of the log loss with respect to the model parameters (coefficients) can be computed 
  efficiently, allowing for efficient gradient-based optimization techniques.

-  log loss in logistic regression indeed results in a convex cost function, which facilitates the training and optimization of the logistic regression model
​![Alt text](https://th.bing.com/th/id/OIP._G3J_3SSN3mmakDWOzwhcQAAAA?pid=ImgDet&rs=1) 
