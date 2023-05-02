# K-Means Clusturing

K-means clustering is a type of unsupervised machine learning algorithm that is used to group similar data points into K clusters. The "K" in K-means clustering represents the number of clusters that the algorithm should create. 

The algorithm works by randomly selecting K data points from the dataset to serve as the initial centroids of the clusters. Each data point is then assigned to the nearest centroid based on its distance to that centroid. The centroids are then recalculated as the mean of the data points assigned to each cluster. This process is repeated until the centroids no longer move or a maximum number of iterations is reached.

K-means clustering is commonly used in data mining, computer vision, and market segmentation. It is a simple and fast algorithm that can handle large datasets, but it has some limitations, such as sensitivity to the initial centroids and difficulty in handling non-linear data.


![Logo](https://i.imgur.com/S65Sk9c.jpg)


## Algorithm
The algorithm works as follows:

1. First, a dataset is input and the number of clusters, k, is chosen. There are various methods for selecting the optimal k value, including the elbow criterion and the silhouette coefficient.

2. Next, k random points from the dataset are chosen as the initial centroids.

3.Calculate the Eucledean Distance from each feature vector to each centroid and assign each datapoint to the closest cluster centroid.

![image](https://user-images.githubusercontent.com/89811204/132998845-37a6f436-47b4-4337-a030-72bd9212d59f.png)

   The algorithm in the attached notebook uses the Euclidean Distance, but there are two other ways of calculating diatance that are used in machine learning algorithms: 

  
   
4. The centroids are then updated by taking the mean of all the data points assigned to each centroid's cluster.

5. Steps 3-4 are repeated until the centroids converge, the data points stop moving between clusters, or the algorithm reaches its maximum number of iterations. It's important to note that the algorithm may converge on a local optimum, so it should be run multiple times.

There are other ways to calculate distance besides the Euclidean Distance used in this algorithm, including the Cosine distance and the Manhattan distance. 

     
   - **Cosine distance:** determines the cosine of the angle between the point vectors of two points in n dimensional space. The closer the point vectors are by angle, the higher the Cosine Similarity. The equation is below:
    
   ![image](https://user-images.githubusercontent.com/89811204/146046597-0f8d9449-30d1-4bc7-9560-1b271cff737b.png)


The Cosine distance calculates the cosine of the angle between two point vectors, while 

 - **Manhattan distance** total sum of the difference between the x-coordinates and the y-coordinates. The equation is below: 
    
      ![image](https://user-images.githubusercontent.com/89811204/146046963-1f7a89a4-2a11-4466-b756-5bb1960d4c44.png)

   The Manhattan distance is so-called because it measures the distance between two points in a city if you could only travel along orthogonal city blocks.

the Manhattan distance calculates the total sum of the differences between the x-coordinates and the y-coordinates.

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

