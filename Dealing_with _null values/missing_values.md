# Why Fill in the Missing Data?

It it necessary to fill in missing data values in data sets as most of the machine learning models that you want to use will provide an error if you pass NaN values into it. The easiest way is to just fill them up with 0, but this can reduce your model accuracy significantly.


# How to Know If the Data Has Missing Values?

1-  df.info() The function can be used to give information about the dataset. This function is one of the most used functions for data analysis.
This will provide you with the column names and the number of non–null values in each column. It will also display the data types of each column.
Thus we can find out which number columns are where null values are present, and by looking at the data types, we can have an understanding of which value to replace nulls with.

2-  The second way of finding whether we have null values in the data is by using the isnull() function.

#What happen if  try fitting the data contain null values using logistic regression ?

**This error happen :**  ValueError: Input contains NaN, infinity or a value too large for dtype('float64').

# What are different Methods of Dealing With Missing Data ?

1. Deleting the column with missing data
![image](https://av-eks-blogoptimized.s3.amazonaws.com/546762.png)

2. Deleting the row with missing data

- axis=1 is used to drop the column with NaN values.

- axis=0 is used to drop the row with NaN values.


3. Filling the Missing Values – Imputation
![image](https://av-eks-blogoptimized.s3.amazonaws.com/240564.png)

**The possible ways to do this are:**

1- Filling the missing data with the mean or median value if it’s a numerical variable.
2- Filling the missing data with mode if it’s a categorical value.
3- Filling the numerical value with 0 or -999, or some other number that will not occur in the data. This can be done so that the machine can recognize that the data is not real or is different.
4- Filling the categorical value with a new type for the missing values.


4. Filling with a Regression Model
In this case, the null values in one column are filled by fitting a regression model using other columns in the dataset
I.e. in this case the regression model will contain all the columns except Age in X and Age in Y.
Then after filling the values in the Age column, then we will use logistic regression to calculate accuracy.
















