# What is Random forest ?
Random forest is a Supervised Machine Learning Algorithm that is used widely in Classification and Regression problems. It builds decision trees on different samples and takes their majority vote for classification and average in case of regression.

# What ensemble learning technique ?
Ensemble simplymeans combining multiple models. Thus a collection of models is used to make predictions rather than an individual model.

# what are types of Ensemble ?

1. Bagging– It creates a different training subset from sample training data with replacement & the final output is based on majority voting. For example,  Random Forest.


2. Boosting– It combines weak learners into strong learners by creating sequential models such that the final model has the highest accuracy. For example,  ADA BOOST, XG BOOST.


# what is Bagging technique ?

is the ensemble technique used by random forest.Bagging chooses a random sample/random subset from the entire data set. Hence each model is generated from the samples (Bootstrap Samples) provided by the Original Data with replacement known as row sampling. This step of row sampling with replacement is called **bootstrap**. Now each model is trained independently, which generates results. The final output is based on majority voting after combining the results of all models. This step which involves combining all the results and generating output based on majority voting, is known as **aggregation**.
![image](https://www.simplilearn.com/ice9/free_resources_article_thumb/Bagging.PNG)


# what are main steps in Random Forest ?
Step 1: In the Random forest model, a subset of data points and a subset of features is selected for constructing each decision tree. Simply put, n random records and m features are taken from the data set having k number of records.


Step 2: Individual decision trees are constructed for each sample.


Step 3: Each decision tree will generate an output.


Step 4: Final output is considered based on Majority Voting or Averaging for Classification and regression, respectively.





# what the important of using Random Forest ?

1- Reduced Overfitting: Random Forests reduce the risk of overfitting compared to individual decision trees. By aggregating predictions from multiple trees, they tend to generalize better to unseen data.

2- High Accuracy: Random Forests are known for their high accuracy in both classification and regression tasks. They work well with complex datasets and are capable of capturing intricate relationships between features and the target variable.

3- Feature Importance: Random Forests provide a measure of feature importance, which helps identify which features are contributing the most to the model's predictions

4- Parallel Processing: Random Forests can be trained in parallel, which speeds up training on multicore processors.



# what are Hyperparameters in Random Forest ?

n_estimators: Number of trees the algorithm builds before averaging the predictions.

max_features: Maximum number of features random forest considers splitting a node.

mini_sample_leaf: Determines the minimum number of leaves required to split an internal node.

criterion: How to split the node in each tree

max_leaf_nodes: Maximum leaf nodes in each tree

n_jobs: it tells the engine how many processors it is allowed to use. If the value is 1, it can use only one processor, but if the value is -1, there is no limit.

random_state: controls randomness of the sample. The model will always produce the same results if it has a definite value of random state and has been given the same hyperparameters and training data.



# what is out of bagging in Random Forest ?

OOB means out of the bag. It is a random forest cross-validation method. In this, one-third of the sample is not used to train the data; instead used to evaluate its performance. These samples are called out-of-bag samples.


# what are solution to solve overfitting decision tree ?

1-Limit Tree Depth (Pruning)

2-Using Ensemble Methods

3-Using Regularization Term 

4-Feature selection

4- Feature Selection

5- Collect more Data 

