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

## How does K-Means Clustering work?
1. Input a dataset and choose the number of clusters, k
  There are two primary ways of selecting the number of clusters:
    - **Elbow criterion**
      Run k-means clustering on the dataset for a range of values of k and calculate the sum of squared errors (SSE) for each k, then calculate the mean distance between data points and their cluster's centroid. As the number of clusters increeases, the number of datapoints per cluster will decrease and will decrease the SSE until the SSE equals zero when k equals the number of datapoints. The goal is to select a small value of k with a low SSE.
    
      In short: run the algorithm for different values of k and plot the k values against SSE, then select the value of k for the "elbow point" where the graph dips.
    - **Silhouette coefficient:**
      The silhouette coefficient is about finding a model with well-defined clusters. This value is calculated by taking the mean distance between a sample and all other points in the same cluster as well as its distance from all other points in the nearest cluster. The equation for a single sample is below:
    
      ![image](https://user-images.githubusercontent.com/89811204/146045653-2898b2fa-6f54-4a50-a617-f8efb3f07ef5.png)

        Using the equation above, calculate the silhouette coefficient for all the clusters. A higher value indicates the sample is well matched to its own cluster and poorly matched to neighboring clusters. 
    - Other ways to choose k: cross-validation, information criteria, information theoretic jump method, G-means algorithm
3. Select k random points from the data as centroids. 
4. Calculate the Eucledean Distance from each feature vector to each centroid and assign each datapoint to the closest cluster centroid.

![image](https://user-images.githubusercontent.com/89811204/132998845-37a6f436-47b4-4337-a030-72bd9212d59f.png)

   The algorithm in the attached notebook uses the Euclidean Distance, but there are two other ways of calculating diatance that are used in machine learning algorithms: 
     
   - **Cosine distance:** determines the cosine of the angle between the point vectors of two points in n dimensional space. The closer the point vectors are by angle, the higher the Cosine Similarity. The equation is below:
    
   ![image](https://user-images.githubusercontent.com/89811204/146046597-0f8d9449-30d1-4bc7-9560-1b271cff737b.png)

   - **Manhattan distance** total sum of the difference between the x-coordinates and the y-coordinates. The equation is below: 
    
      ![image](https://user-images.githubusercontent.com/89811204/146046963-1f7a89a4-2a11-4466-b756-5bb1960d4c44.png)

   The Manhattan distance is so-called because it measures the distance between two points in a city if you could only travel along orthogonal city blocks.
   
4. Update the centroid for each cluster by taking the mean of all the datapoints assigned to that centroid's cluster.

5. Report previous steps 3-4 until the centroids converge (no change in cetnroids), datapoints stop moving between clusters, or the algorithm reaches the maximum number of iterations. Note that the algorithm may converge on a _local_ optimum, so it is important to run the algorithm several times. 

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
