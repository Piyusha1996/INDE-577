# K-Nearest neighbours
K-nearest neighbors (KNN) is a machine learning algorithm used for both regression and classification tasks. The algorithm works by finding the K closest data points to a given test point, and then making a prediction based on the labels of those closest data points.

Birds of a feather flock together.

![image](https://miro.medium.com/v2/resize:fit:1222/format:webp/1*wW8O-0xVQUFhBGexx2B6hg.png)

# How it works

- The training data is first considered as vectors in multidimensional space (depending on features).

- There is a user-defined constant k, that’s why this algorithm is called K Nearest Neighbor or KNN.
- When a user passes an instance for classification, this algorithm first calculates the distance between the instance and all of the vector points given in the data. For this commonly euclidean distance is used, but other distance based methods can also be used, depending on the use case and performance.

![image](https://miro.medium.com/v2/resize:fit:538/format:webp/0*yPNLlZPav7W6xDxS.png)

![image](https://miro.medium.com/v2/resize:fit:1400/format:webp/1*zQucA3czF28kk5c10WukRg.png)


- After calculating the distance between instance and all points in training data, the algorithm calculates its k nearest neighbors through sorting usually or some other method to find k nearest neighbors
- Then it performs majority voting usually on its k nearest neighbor, and classifies the given instance accordingly.

![image](https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcSOqFhZ3V4nuwZ5hHacqTqcLmicGcOItWsxjg&usqp=CAU)

# Choosing K
The value of K is an important hyperparameter in KNN. Choosing the right value of K can greatly affect the performance of the algorithm. A larger value of K will result in a smoother decision boundary, while a smaller value of K will result in a more complex decision boundary. One common approach is to use cross-validation to find the optimal value of K.

![image](https://miro.medium.com/v2/resize:fit:1400/format:webp/1*WoL6cFcZZ2ZxVJ8k5iA7sw.png)

# Pros and Cons
- Pros

Simple and easy to understand
Can be used for both regression and classification tasks
No assumption about the underlying data distribution is needed
Non-parametric (i.e., no assumption about the shape of the underlying function)

- Cons
Can be slow and computationally expensive for large datasets
Requires careful selection of distance metric and value of K
Can be sensitive to outliers in the data
The algorithm doesn't provide a way to interpret the features that are important for the prediction.



Overall, KNN can be a powerful and useful algorithm for many machine learning tasks. However, it is important to carefully consider the choice of K and the distance metric used, and to be aware of its limitations when applying it to a particular problem.







#Acknowledgements

[K- nearest neighbours](https://medium.com/@muhammadammarabid01/k-nearest-neigbors-knn-basic-algorithm-from-scratch-in-python-8471b655a013)
[[classification](https://stackoverflow.com/questions/11568897/value-of-k-in-k-nearest-neighbor-algorithm)
