## Data Leakage And Its Effect On The Performance of An ML Model

![image](https://miro.medium.com/v2/resize:fit:750/1*TSX7fu85EwGEdnhA-Sv4cA.jpeg)

 # what is Data Leakage?

Let’s start our discussion by imagine a scenario where you have tested your machine learning model well, and you get absolutely perfect accuracy. After getting the accuracy, you are happy with your work and say well done to yourself, and then decide to deploy your project. However, when the actual data is applied to this model in the production, you get poor results , The possible reason for this occurrence is **Data Leakage**

mean **Data Leakage** in machine learning happens when the data that we are used to training a machine learning algorithm is having the information which the model is trying to predict, this results in unreliable and bad prediction outcomes after model deployment.


# How does it exactly happen?

In simple terms, Data Leakage occurs when the data used in the training process contains information about what the model is trying to predict. It appears like “cheating” but since we are not aware of it so, it is better to call it “leakage” instead of cheating , Therefore, Data leakage is a serious and widespread problem in data mining and machine learning which needs to be handled well to obtain a robust and generalized predictive model.


 # What is the result of model on Train , Test , Production if there are Data Leakage Problem ?

 both training and testing accuracy should be high, but got poor result on Production data

# General Examples of Data Leakage ?

**Example 1-**

The most obvious and easy-to-understand cause of data leakage is to include the target variable as a feature. What happens is that after including the target variable as a feature, our purpose of prediction got destroyed. This is likely to be done by mistake but while modelling any ML model, you have to make sure that the target variable is differentiated from the set of features.

**Example 2 –**
To properly evaluate a particular machine learning model, we split our available data into training and test subsets. Invariably, what happens is that some of the information from the test set is shared with the train set, and vice-versa. So, another common cause of data leakage is to include test data with training data. Therefore, It becomes necessary to test the models with new and previously unseen data. If we include the test data in the training, then the process would defeat this purpose.


# How to detect Data Leakage?

**Case-1:**
In general, if we see that the model which we build **is too good to be true** ( gives predicted and actual output the same), then we should get suspicious and data leakage cannot be ruled out. At that time, the model might be somehow memorizing the relations between feature and target instead of learning and generalizing it for the unseen data



**Case-2: **

While doing the Exploratory Data Analysis (EDA), we may detect features that are very highly correlated with the target variable. Of course, some features are more correlated than others but a surprisingly high correlation needs to be checked and handled carefully. We should pay close attention to those features. So, with the help of EDA, we can examine the raw data through statistical and visualization tools.


# How to fix the problem of Data Leakage?

**Idea-1 (Extracting the appropriate set of Features)**

the first method we can try is to extract the appropriate set of features for a machine learning model. While choosing features, we should make sure that the given features are not correlated with the given target variable, as well as that they do not contain information about the target variable, which is not naturally available at the time of prediction.

# Idea-3 (Apply Data preprocessing Separately to both Train and Test subsets)
While dealing with neural networks, it is a common practice that we normalize our input data firstly before feeding it into the model. Generally, data normalization is done by dividing the data by its mean value. More often than not, this normalization is applied to the overall data set, which influences the training set from the information of the test set and eventually it results in data leakage. Hence, to avoid data leakage, we have to apply any normalization technique separately to both training and test subsets.



















