# what is the Gradient boosting ?

 is one of the ensemble machine learning techniques. It uses weak learners like the others in a sequence to produce a robust model
It is a flexible and powerful technique that can be used for both regression and classification problems. Good results can be achieved
even with a very little tuning. It can handle a large number of features and is not biased towards any particular feature type.


# What are the main steps in Gradient boosting ?


1- start with a single leaf means that we will initialize the model with a constant.

Imagine that we have a dummy dataset and target feature as above. In this case, our initial prediction will be the average = 75.

  ![image](https://miro.medium.com/v2/resize:fit:720/format:webp/1*Nr7azub07vhCrf7enCOIuQ.png)


2- compute the residual error (Actual value - Predicted Value )

 ![image](https://miro.medium.com/v2/resize:fit:750/format:webp/1*hczu0UgP2TQEfPF_-1oeiA.png)

In this step, we will build a base learner (decision tree in our case). Our target feature will not be the target column, instead, it will be the residuals.


3-  calculate the gamma value for each leaf separately and whatever observations are on the leaf in question will be included in the calculation

4- Update the predictions

the output table after two prediction : 

![image](https://miro.medium.com/v2/resize:fit:1100/format:webp/1*YxsvdIywm-WeIjuvEZB98g.png)



# what are the Hyperparameter in Gradient Boosting ?


1-  Number of Trees (n_estimators): The number of decision trees to be built. A higher value often leads to better performance, but it can increase training time.

2- Learning Rate (learning_rate): Also known as the shrinkage parameter, it controls the contribution of each tree to the final prediction. Lower values require more trees for the same performance but may generalize better. Typical values are in the range of 0.01 to 0.3.

3- Tree Depth (max_depth): The maximum depth of each decision tree in the ensemble. A deeper tree can capture complex patterns in the data but is prone to overfitting. It should be tuned carefully.

4- Minimum Samples per Leaf (min_samples_leaf): The minimum number of samples required to be in a leaf node. It helps control overfitting.

5- Minimum Samples per Split (min_samples_split): The minimum number of samples required to split an internal node. It also helps control overfitting.

6- Subsampling (subsample): The fraction of samples used for fitting the trees. It's also known as Stochastic Gradient Boosting and can help reduce overfitting. Typical values are between 0.5 and 1.0.

7- Maximum Features (max_features): The number of features considered for splitting at each node. It helps reduce the risk of overfitting. "auto" means all features, "sqrt" means the square root of the number of features, and "log2" means the base-2 logarithm of the number of features.

8- Loss Function (loss): The loss function to optimize during training. Common options include "deviance" for classification problems (logistic regression) and "ls" for regression problems (least squares).

9- Random State (random_state): A random seed used to ensure reproducibility. Setting this value ensures that the results are consistent across runs.
