# what is the XGboost model ?
 stands for eXtreme Gradient Boosting, is a popular and powerful machine learning algorithm used for both classification and regression tasks. 
 It belongs to the class of ensemble learning methods, specifically gradient boosting, and is known for its speed and performance in various 
 machine learning competitions and real-world applications
![image](https://i0.wp.com/neptune.ai/wp-content/uploads/2022/10/Ensemble-algorithms-boosting.png?ssl=1)





 

# what is the Main Framework of XGboost ?

XGBoost is built on the gradient boosting framework, which involves creating an ensemble of weak learners

# How XGboost help to prevent overfitting ?

1- use multiple weak leaener models insted of one complex  and this help to reduce the complexity of mode 

2- XGBoost includes built-in L1 (Lasso) and L2 (Ridge) regularization terms, which can help prevent overfitting


# what are the advantages of using XGboost ?

1- Handling  the  problem of overfitting 

2- XGBoost is scalable and can handle large datasets.

3-  provides feature importance scores, which can help identify the most relevant features for making predictions

4-  it may not fully exploit the capabilities of modern hardware with multiple cores or distributed computing clusters (Sequntial Maodel) 

5- XGBoost can be configured to work in parallel mode to take advantage of multiple cores and distributed computing environments

# XGboost work Sequential or parallel ?

XGBoost operates in sequential mode, where the boosting process is performed sequentially, one tree at a time. In this mode, 
each decision tree is built using information from the previous tree.While this mode is straightforward and suitable for many use cases


# Based on what the model can prune tree in XGboost ?

based on the difference between the value of Gain and the value of Gamma 
- if(Gain-Gamma)<0 the model prune the branch
- if(Gain-Gamma)>0 the model not prune the branch

# What are tha Main HyperParameter in XGboost ?

1- alpha  : L1 and L2 regularization terms on weights. They help to control overfitting.

2- gamma  : Minimum loss reduction required to make a further partition

3-  n_estimators: The number of boosting rounds (trees)

4- Max_depth

5- Learning Rate 
