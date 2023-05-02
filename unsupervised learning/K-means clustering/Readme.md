# K-Means Clusturing

K-means clustering is a type of unsupervised machine learning algorithm that is used to group similar data points into K clusters. The "K" in K-means clustering represents the number of clusters that the algorithm should create. 

The algorithm works by randomly selecting K data points from the dataset to serve as the initial centroids of the clusters. Each data point is then assigned to the nearest centroid based on its distance to that centroid. The centroids are then recalculated as the mean of the data points assigned to each cluster. This process is repeated until the centroids no longer move or a maximum number of iterations is reached.

K-means clustering is commonly used in data mining, computer vision, and market segmentation. It is a simple and fast algorithm that can handle large datasets, but it has some limitations, such as sensitivity to the initial centroids and difficulty in handling non-linear data.


![Logo](https://i.imgur.com/S65Sk9c.jpg)


## Algorithm
1. Choose the number of clusters (k) that you want to create.

2. Initialize k centroids randomly. Each centroid represents the center point of a cluster.

3. Assign each data point to the nearest centroid. This is done by calculating the distance between each data point and each centroid and assigning the data point to the centroid with the shortest distance.

4. Recalculate the centroid of each cluster. This is done by taking the mean of all the data points in each cluster.

5. Repeat steps 3 and 4 until the centroids no longer move or a maximum number of iterations is reached.

![Logo](https://i.imgur.com/k4XcapI.gif)

The final result is k clusters, each with its own centroid and a set of data points assigned to it.


The results of a k-means clustering algorithm include the following:

1. Cluster assignments: Each data point is assigned to one of the k clusters based on its distance to the centroid. The cluster assignments can be used to understand which data points are similar to each other and which are dissimilar.

2. Centroids: The final centroids of each cluster represent the center point of that cluster. These centroids can be used to understand the characteristics of each cluster and to make predictions for new data points.

3. Within-cluster sum of squares (WSS): This measures the sum of the squared distances of each data point to its assigned centroid within each cluster. A lower WSS indicates that the data points within each cluster are closer to their respective centroids and that the clustering is more effective.

4. Between-cluster sum of squares (BSS): This measures the sum of the squared distances between the centroids of each cluster. A higher BSS indicates that the clusters are well-separated and that the clustering is effective.

5. Elbow plot: This is a visual representation of the WSS for different values of k. The plot shows the relationship between the number of clusters and the WSS. The "elbow" point on the plot indicates the optimal number of clusters, where adding more clusters does not significantly improve the clustering results.

## Acknowledgements

 - [K-Means Theory ](https://www.analyticsvidhya.com/blog/2019/08/comprehensive-guide-k-means-clustering/)
 - [K-Means algorithm](https://mubaris.com/posts/kmeans-clustering/)
