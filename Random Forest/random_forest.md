# What is Random forest ?
Random forest is a Supervised Machine Learning Algorithm that is used widely in Classification and Regression problems. It builds decision trees on different samples and takes their majority vote for classification and average in case of regression.

# What ensemble learning technique ?
Ensemble simplymeans combining multiple models. Thus a collection of models is used to make predictions rather than an individual model.

# what are types of Ensemble ?

1. Bagging– It creates a different training subset from sample training data with replacement & the final output is based on majority voting. For example,  Random Forest.


2. Boosting– It combines weak learners into strong learners by creating sequential models such that the final model has the highest accuracy. For example,  ADA BOOST, XG BOOST.

 ![image](https://av-eks-blogoptimized.s3.amazonaws.com/4661536426211ba43ea612c8e1a6a1ed4550721164.png)

# what is Bagging technique ?

is the ensemble technique used by random forest.Bagging chooses a random sample/random subset from the entire data set. Hence each model is generated from the samples (Bootstrap Samples) provided by the Original Data with replacement known as row sampling. This step of row sampling with replacement is called **bootstrap**. Now each model is trained independently, which generates results. The final output is based on majority voting after combining the results of all models. This step which involves combining all the results and generating output based on majority voting, is known as **aggregation**.
![image](https://www.simplilearn.com/ice9/free_resources_article_thumb/Bagging.PNG)
