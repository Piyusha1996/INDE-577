# Principle Component Analysis (PCA)

Principle Component Analysis (PCA) is a widely used technique in data analysis and machine learning. It is a dimensionality reduction technique that can be used to reduce the number of variables in a dataset while retaining as much information as possible.

PCA works by finding the principal components of the dataset, which are linear combinations of the original variables that capture the most variance in the data. These components are ordered in terms of the amount of variance they capture, with the first component capturing the most variance and so on.

PCA can be used for a variety of tasks, including data visualization, feature extraction, and data compression. It is particularly useful when dealing with high-dimensional datasets where the number of variables is much larger than the number of observations.



![Logo](https://miro.medium.com/v2/resize:fit:1192/format:webp/1*QinDfRawRskupf4mU5bYSA.png)

Principal Component Analysis (PCA) is a popular unsupervised machine learning technique used for dimensionality reduction. The goal of PCA is to identify the most important features or components in a dataset and transform the data into a new coordinate system where these components can be visualized and analyzed easily.

The algorithm for PCA can be summarized in the following steps:

1. Standardize the data: PCA requires the data to be standardized, meaning that each feature should have zero mean and unit variance.

2. Compute the covariance matrix: Calculate the covariance matrix of the standardized data, which represents the relationships between the different features.

3. Compute the eigenvectors and eigenvalues: Find the eigenvectors and eigenvalues of the covariance matrix. Eigenvectors represent the directions in which the data varies the most, and eigenvalues represent the magnitude of this variance.

4. Select the principal components: Select the top k eigenvectors with the highest eigenvalues to form the principal components.

5. Transform the data: Project the original data onto the new coordinate system formed by the principal components to obtain the transformed data.

PCA can be used for a variety of applications such as data visualization, feature extraction, and noise reduction. It is widely used in fields such as image processing, finance, and natural language processing.

![Logo](https://devopedia.org/images/article/139/4543.1548137789.jpg)

The math underlying PCA is quite complicated, but at a high level:
Consider an n x p data matrix X, where each of the rows represents a different repetition of the experiment and each of the columns gives a particular kind of feature. the k-th component can be found by subtracting the first k principal components from X as shown below:

![image](https://user-images.githubusercontent.com/89811204/146064331-67d84e5c-b938-40f7-9fc1-716577c032cb.png)

then finding a new weight vector which extracts the maximum variance from this new data matrix, as detailed below:

![image](https://user-images.githubusercontent.com/89811204/146064425-486393f3-b30f-4de9-abb8-2db1c72dc636.png)

i.e. the weight vectors are the eigenvectors of X^TX. The full principal components of X can therefore be given as T = XW, where W is a p by p matrix of weights whos colums are the eigenvectors fo X^TX.

Principal Component Analysis (PCA) is a widely used technique in data analysis that offers several benefits, including:

1. Dimensionality reduction: PCA helps to reduce the number of variables in a dataset while retaining the maximum amount of information. This is particularly useful when working with large datasets that have many variables, making it easier to analyze the data and visualize patterns.


![Logo](https://www.researchgate.net/profile/Nico-Migenda/publication/350507718/figure/fig1/AS:1010319459643392@1617890338021/Dimensionality-reduction-process-performed-with-a-PCA-a-Data-distribution-in-a.png)

2. Identifying important variables: PCA can help identify the variables that contribute most to the variation in the data, allowing researchers to focus on the most important variables in their analysis.


3. Improved data visualization: PCA can help to visualize high-dimensional data in two or three dimensions, making it easier to identify patterns and relationships in the data.

4. Data pre-processing: PCA can be used as a pre-processing step before applying other machine learning algorithms. It can help to remove redundant information from the data, reduce noise, and improve the performance of other algorithms.

5. Better understanding of data: PCA can provide insights into the underlying structure of the data by identifying hidden patterns and relationships between variables. This can help researchers to better understand the data and formulate hypotheses for further analysis.

![Logo](https://online.stat.psu.edu/onlinecourses/sites/stat508/files/lesson05/image_05.gif)
## Acknowledgements

 - [PCA Theory ](https://towardsdatascience.com/a-one-stop-shop-for-principal-component-analysis-5582fb7e0a9c)
 - [PCA - Interactive analysis](https://setosa.io/ev/principal-component-analysis/)

