 # what is KMeans Model ?
 
 machine learning algorithm used for clustering or grouping data points into K distinct and non-overlapping clusters. It's a popular unsupervised learning algorithm and is often used for tasks such as customer segmentation, image compression, and anomaly detection. The main idea behind K-Means is to find groups in the data, with the number of groups represented by the variable "K."
![Image](https://geomodeling.njnu.edu.cn/static/modelItem/c777f4e3-533d-480c-809d-f10757a5d5a5.jpg)

# what are the main steps in KMeans Model ?

1- **Initialization:** The algorithm starts by randomly selecting K data points from the dataset as initial cluster centroids .

2- **Assignment":** For each data point in the dataset, the algorithm calculates the distance between the point and each of the K centroids. The data point is assigned to the cluster whose centroid is closest to it .

3- **Update Centroid:** : After assigning all data points to clusters, the algorithm updates the cluster centroids by computing the mean (average) of all data points assigned to each cluster. These new centroids represent the updated cluster centers .

4- Calculate Errror **(WCSS)** within class sum of square .
'''
WCSS=∑ 
i=1
K
​
 ∑ 
j=1
n 
i

 ∣∣x 
ij
​
 −c 
i
​
 ∣∣ 
2
'''



5- **Repeat:** Steps 2 and 3 are repeated iteratively until a stopping criterion is met. The most common stopping criterion is when the centroids no longer change significantly or when a maximum number of iterations is reached
