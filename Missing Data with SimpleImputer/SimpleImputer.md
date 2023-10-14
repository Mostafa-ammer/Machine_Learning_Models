# How to dealing with Missing values 

# How can we used "scikit learn"  ?

 By using scikit learn library named SimpleImputer

# What the  values of Missing Values ?

the values of missing values is “None” or “NaN” type 

#  How can SimpleImputer  solve the problem of missing values ?

it replaces the missing data with another value based on a given strategy(parameter).

#  What are Parameters of the SimpleImputer ?

1- **Missing_values :** indicates the missing values in the dataset. By default np.nan is set in the missing_values, which means all the values containing np.nan will be considered as missing values.

2-  **strategy:**  it is the method by using which we want to fill in the missing values.the value of the strategy could be “mean”, “median”, “most_frequent”, or “constant”.

3- **fill_values:**  It is a parameter only used when the strategy is set to be constant. When the strategy is constant, the Nan values will be replaced by the value passes in fill_value.

4- **copy:**  If this parameter is set to be True, then the copy of the dataset will be created, else imputation will be done without copying.

 # How can use " SimpleImputer " library in python ?

1- install sklearn library 

       - import sklearn

2- importing simpleimputer from sklearn 

      -  from sklearn.impute import SimpleImputer



#  what happen if the data contains Outliers ?

 we must avoid using "Mean" as SimpleImputer because mean affected by " outlier" 


# When using "Mean Imputer , Median Imputer , Mode Imputer , constant imputer ?


-  We can use Mean Imputer , Median Imputer with **Numerical data**

-  We can use  Mode Imputer with **Categorical data** 

- we can use Constant imputer with   **Numerical data - Categorical data**
 
