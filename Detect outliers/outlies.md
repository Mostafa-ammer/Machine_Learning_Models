![image](https://cdn.analyticsvidhya.com/wp-content/uploads/2019/02/Outliers.jpeg)
# How can outlier affect on central tendency such as Mean, Median, and Mode ?

if there an outlier on data the most central tendency affected by outliers is " Mean" then "Median" and " mode "

**Example : **

Consider a small dataset, sample= [15, 101, 18, 7, 13, 16, 11, 21, 5, 15, 10, 9]. By looking at it, one can quickly say ‘101’ is an outlier that is much larger than the other values.

![image](https://editor.analyticsvidhya.com/uploads/88471with_without_outliers.PNG)

# How can we detect outliers ?
If our dataset is small, we can detect the outlier by just looking at the dataset. But what if we have a huge dataset, how do we identify the outliers then? We need to use visualization and mathematical techniques.
**Below are some of the techniques of detecting outliers**

1- Boxplots

![image](https://www.statology.org/wp-content/uploads/2022/09/outlierbox2.jpg)


2- Z-score

Criteria: any data point whose Z-score falls out of 3rd standard deviation is an outlier.

![image](https://cdn.analyticsvidhya.com/wp-content/uploads/2023/09/image-76.png)

3- Inter Quantile Range(IQR)
Criteria: data points that lie 1.5 times of IQR above Q3 and below Q1 are outliers. This shows in detail about outlier treatment in Python.

![image](https://editor.analyticsvidhya.com/uploads/12311IQR.png)

**Main steps**
1- Sort the dataset in ascending order

2- calculate the 1st and 3rd quartiles(Q1, Q3)

3- compute IQR=Q3-Q1

4- compute lower bound = (Q1–1.5*IQR), upper bound = (Q3+1.5*IQR)

5- loop through the values of the dataset and check for those who fall below the lower bound and above the upper bound and mark them as outliers



