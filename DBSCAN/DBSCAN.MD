# What is DBSCAN Algorithm ?
is a popular density-based clustering algorithm used in machine learning and data analysis. It is designed to discover clusters of data points in a dataset based on their spatial density distribution


# What is The two parameters present in a DBSCAN algorithm  ?

1- MinPoints (MinPts) : the minimum number of points inside hypersphere(circle)

2- Epsilon (Eps) :  the  radius of hypersphere

DBSCAN requires only two parameters: epsilon and minPoints. Epsilon is the radius of the circle to be created around each data point to check the density and minPoints is the minimum number of data points required inside that circle for that data point to be classified as a Core point.


DBSCAN creates a circle of epsilon radius around every data point and classifies them into Core point, Border point, and Noise. A data point is a Core point if the circle around it contains at least ‘minPoints’ number of points. If the number of points is less than minPoints, then it is classified as Border Point, and if there are no other data points around any data point within epsilon radius, then it treated as Noise

![image](https://cdn.analyticsvidhya.com/wp-content/uploads/2020/03/db26.png)

#  What are the types of data points in DBSCAN alogorithm ?

1- Core Points
      Core Point (P): The point P is said to be the core point if P has greater than MinPts in an Eps radius around it.
      These points always belong to the dense region and are at the interior of a cluster.

2-Border Points
   Border Point (P): The point P is said to be the border point if
   “P” is not the core point, it means that “P” has less than Minpts in an Eps radius around it.

3- Noise Points
      Any point which is neither a core point nor a border point is called a noise point.

![image](https://miro.medium.com/v2/resize:fit:1400/format:webp/1*XS889sctfs87fgLSELxPRA.png)

Now in this image my MinPts is 4 and Eps is 1, so when we draw a circle around it we have 5 points inside that which is greater than the MinPts so this point is Core Point. Now on the left side when we draw a circle around it we just have 3 points which are less than the number of MinPts so that point is not a core point and the distance between these two points is less than the Eps. Hence, that point becomes a Border Point. Now if you look at the Noise point so the points inside that circle are less than the MinPts and the distance from the core point is also greater than the Eps that is why it becomes a Noise Point.


# What are the main steps in  DBSCAN algorithm ?


1. For each point in my dataset, label each point as a core point or border point, or noise point.

2. Now, remove all the noise points from data because noise points belong to the sparse region it means they don’t belong to any clusters.

3. For each core point ‘p’ that is not assigned to a cluster.

· Create a new cluster with ‘p’.

· Add all points that are density connected to ‘p’ into this new cluster.

4. Take each border point and assign it to the nearest core point’s cluster.



# What are the Limitations of DBSCAN Algorithm ?

1. If we have a dataset of different densities, the algorithm fails to give an accurate result.

2. It is very sensitive to hyperparameters.

3. If you are having high-dimensional data and you are using metrics like Euclidean distance you easily kick into the problem of Curse of Dimensionality.




# Parameter Selection in DBSCAN Clustering ?


DBSCAN is very sensitive to the values of epsilon and minPoints. Therefore, it is very important to understand how to select the values of epsilon and minPoints. A slight variation in these values can significantly change the results produced by the DBSCAN algorithm.

The value of minPoints should be at least one greater than the number of dimensions of the dataset, i.e., 

minPoints>=Dimensions+1.

It does not make sense to take minPoints as 1 because it will result in each point being a separate cluster. Therefore, it must be at least 3. Generally, it is twice the dimensions. But domain knowledge also decides its value.

The value of epsilon can be decided from the K-distance graph. The point of maximum curvature (elbow) in this graph tells us about the value of epsilon. If the value of epsilon chosen is too small then a higher number of clusters will be created, and more data points will be taken as noise. Whereas, if chosen too big then various small clusters will merge into a big cluster, and we will lose details.












