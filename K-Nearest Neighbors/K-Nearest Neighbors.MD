# what is K-nearest Neighbors (KNN) algorithm ?

supervised machine learning algorithm used for classification, regression as well as outlier detection. It is extremely easy to implement in its most basic form but can perform fairly complex tasks. 
It is a lazy learning algorithm since it doesn't have a specialized training phase


# How KNN works ?

1- it uses all of the data for training while classifying (or regressing) a new data point or instance.

2- get the distance between new point and all points 

3-  Based on the values of "k" , model  can determine the closest points to new point 

4- if Task regression use Mean to predict the output , if Task Classiffication use Majority Voting 


# Why KNN is a non-parametric learning algorithm ?

KNN does not make any assumptions about the functional form of the relationship. It does not fit a predetermined mathematical model to the data.

# what the difference between non-parametric and parametric  ?

1- Parametric models : like linear regression or logistic regression, assume a fixed mathematical function (e.g., linear, logistic) to describe the relationship between variables

2- non-parametric models  : does not make any assumptions about the functional form of the relationship


# why KNN is lazy learning algorithm ?

Beacuse no training happen in KNN


# Example about regression tasks in KNN ?

KNN selects a number of nearest data points - 2, 3, 10, or really, any integer. This number of points (2, 3, 10, etc.) is the K in K-Nearest Neighbors!

In the final step, if it is a regression task, KNN will calculate the average weighted sum of the K-nearest points for the prediction. If it is a classification task, the new data point will be assigned to the class to which the majority of the selected K-nearest points belong.

Let's visualize the algorithm in action with the help of a simple example. Consider a dataset with two variables and a K of 3.

When performing regression, the task is to find the value of a new data point, based on the average weighted sum of the 3 nearest points.

KNN with K = 3, when used for regression:


![image](https://s3.stackabuse.com/media/articles/k-nearest-neighbors-algorithm-python-scikit-learn-1.png)
![image](https://s3.stackabuse.com/media/articles/k-nearest-neighbors-algorithm-python-scikit-learn-2.png)


# Example of Classification Task in KNN ?


calculating the distance of the new point from all the points. It then finds the 3 points with the least distance to the new point. This is shown in the second figure above, in which the three nearest points, 47, 58, and 79 have been encircled. After that, 
it calculates the weighted sum of 47, 58 and 79 - in this case the weights are equal to 1 - we are considering all points as equals, but we could also assign different weights based on distance. After calculating the weighted sum, the new point value is 61,33.
And when performing a classification, the KNN task is to classify a new data point, into the "Purple" or "Red" class. (image)


# why in KNN , feature scaling happen after spliting not before splitting ?

it is generally recommended to perform feature scaling after splitting the dataset into training and testing sets, rather than before splitting. This is done for avoiding Data Leakage:
Data Leakage Prevention: If you scale the entire dataset (including both training and testing data) before splitting, information from the testing set can potentially leak into the training set. 
Scaling involves calculating statistics like the mean and standard deviation of the data, and these statistics should be computed solely on the training data to avoid any data leakage.
 If you scale before splitting, the testing data might influence the scaling process, leading to overly optimistic performance estimates.


# what is the Disadvantages of KNN ?

1- Don't work with Large Dataset.

2- Don't work well with High Dimension .

3- Sensitive to outlier .

4- Need to make feature scaling .

5- Non-parametric model , No Training happen .


# what happen if the value of k is very small or very large in Knn ?

- When you choose a very small value of "k" , the model becomes highly sensitive to noise in the training data. It may result in overfitting
- When you choose a very large value of "k," the model may underfit the data

