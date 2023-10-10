# What Is a Confusion Matrix?
is a performance evaluation tool in machine learning, representing the accuracy of a classification model. It displays the number of true positives, true negatives, false positives, and false negatives. This matrix aids in analyzing model performance, identifying mis-classifications, and improving predictive accuracy.

A Confusion matrix is an N x N matrix used for evaluating the performance of a classification model, where N is the total number of target classes. The matrix compares the actual target values with those predicted by the machine learning model. This gives us a holistic view of how well our classification model is performing and what kinds of errors it is making.
![image](https://av-eks-blogoptimized.s3.amazonaws.com/Basic-Confusion-matrix.png)

-  The target variable has two values: Positive or Negative

-  The columns represent the actual values of the target variable

-  The rows represent the predicted values of the target variable


# what are the important Terms in a Confusion Matrix ?

**True Positive (TP)** :  The actual value was positive, and the model predicted a positive value.
**True Negative (TN) **:  The actual value was negative, and the model predicted a negative value.
**False Positive (FP) – Type I Error**:  The actual value was negative, but the model predicted a positive value.
**False Negative (FN) – Type II Error**:  The actual value was positive, but the model predicted a negative value.


**Example : **
Suppose we had a classification dataset with 1000 data points. We fit a classifier (say logistic regression or decision tree) on it and get the below confusion matrix:
![image](https://av-eks-blogoptimized.s3.amazonaws.com/Confusionmatrix-example.png)

- True Positive (TP) = 560, meaning the model correctly classified 560 positive class data points.

- True Negative (TN) = 330, meaning the model correctly classified 330 negative class data points.

- False Positive (FP) = 60, meaning the model incorrectly classified 60 negative class data points as belonging to the positive class.

- False Negative (FN) = 50, meaning the model incorrectly classified 50 positive class data points as belonging to the negative class.



What is the differnce between Precision vs. Recall ?

- Precision :  Precision tells us how many of the correctly predicted cases actually turned out to be positive.
![image](https://av-eks-blogoptimized.s3.amazonaws.com/Confusion-matrix_Precision.png)
- Recall : Recall tells us how many of the actual positive cases we were able to predict correctly with our model.
![image](https://av-eks-blogoptimized.s3.amazonaws.com/Confusion-matrix_Recall.png)

![image](https://av-eks-blogoptimized.s3.amazonaws.com/Example-Confusion-matrix.png)


# What Is F1-Score?

F1-score is a harmonic mean of Precision and Recall, and so it gives a combined idea about these two metrics. It is maximum when Precision is equal to Recall.

![image](https://av-eks-blogoptimized.s3.amazonaws.com/Confusion-Matrix-F1-score.png)


























