# What is Hierarchical Clustering?

Hierarchical clustering is a popular method for grouping objects. It creates groups so that objects within a group are similar to each other and different from objects in other groups. Clusters are visually represented in a hierarchical tree called a dendrogram.
![image](https://miro.medium.com/v2/resize:fit:720/0*afzanWwrDq9vd2g-)


# Hierarchical clustering types ?

There are two main types of hierarchical clustering:

**Agglomerative:** Initially, each object is considered to be its own cluster. According to a particular procedure, the clusters are then merged step by step until a single cluster remains. At the end of the cluster merging process, a cluster containing all the elements will be formed.

**Divisive:** The Divisive method is the opposite of the Agglomerative method. Initially, all objects are considered in a single cluster. Then the division process is performed step by step until each object forms a different cluster. The cluster division or splitting procedure is carried out according to some principles that maximum distance between neighboring objects in the cluster.


# How to compute Similarity between Clusters  ?


1- **Min (Single) Linkage :**

One way to measure the distance between clusters is to find the minimum distance between points in those clusters. That is, we can find the point in the first cluster nearest to a point in the other cluster and calculate the distance between those points. In Figure 2,
the closest points are in one cluster and in the other. The distance between those points, and hence the distance between clusters

![image](https://storage.googleapis.com/lds-media/images/Sample-data-min-distance-single-linkage.width-1200.jpg)


**disadvantages is :** it is sensitive to noise and outliers

2-  **Max (Complete) Linkage**

Another way to measure the distance is to find the maximum distance between points in two clusters. We can find the points in each cluster that are furthest away from each other and calculate the distance between those points.
In Next  Figure ,  Distance between those two points, and hence the distance between clusters

![image](https://storage.googleapis.com/lds-media/images/Sample-data-max-distance-complete-linkage.width-1200.jpg)


3- **Centroid Linkage:**

The Centroid method defines the distance between clusters as being the distance between their centers/centroids. After calculating the centroid for each cluster, the distance between those centroids is computed using a distance function.

![image](https://storage.googleapis.com/lds-media/images/Sample-data-centroid-distance-linkage.width-1200.jpg)


4- **Average Linkage :**

  The Average method defines the distance between clusters as the average pairwise distance among all pairs of points in the clusters. For simplicity, only some of the lines connecting pairs of points
![image](https://storage.googleapis.com/lds-media/images/Sample-data-average-distance-linkage.width-1200.jpg)


















