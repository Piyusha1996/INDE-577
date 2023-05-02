# Decision Tree Regression 

Decision Tree Regression is a machine learning algorithm used for solving both regression and classification tasks. It is a tree-structured classifier with three types of nodes, including the Root Node, Interior Nodes, and Leaf Nodes. The Root Node represents the entire sample, which may be further split into more nodes based on features of the data set. The Interior Nodes represent the decision rules, while the Leaf Nodes represent the outcome or the predicted values.

![image](https://miro.medium.com/v2/resize:fit:1400/format:webp/0*IY07ftCHvVuuw35_.png)



In decision tree regression, the algorithm works by dividing the data set into subsets based on the values of a particular feature. The algorithm determines the feature that is most useful for splitting the data into subsets such that it minimizes the error between the predicted values and the actual values. This process is repeated recursively until the tree is fully built, and the outcome can be predicted for new data points.

![image](https://miro.medium.com/v2/resize:fit:1000/format:webp/0*YlmscpNST8MY7yzw.png)


Advantages of Decision Tree Regression:

1. Easy to Understand: Decision Tree Regression is simple and easy to understand, making it a popular choice for beginners.

2. Handles both numerical and categorical data: Decision trees can handle both numerical and categorical data without requiring much data pre-processing.

3. Less Data Cleaning Required: Decision trees do not require extensive data cleaning or normalization, unlike many other machine learning algorithms.

4. Non-linearity does not affect model performance: Decision tree regression can easily handle non-linear relationships between the input and output variables.

Disadvantages and Limitations of Decision Tree Regression:

1. Overfitting: Decision trees have a tendency to overfit the data, which can lead to poor performance on new, unseen data.

2. Instability: Small changes in the data can result in large changes in the final decision tree, leading to instability in the model.

3. Bias: Decision trees can be biased towards features with more levels, leading to an incorrect model.

![image](https://editor.analyticsvidhya.com/uploads/983161.png)

4. Complexity: Decision trees can become complex with many features, which can lead to longer training times and slower prediction times.

Algorithm for Decision Tree Regression:

![image](https://static.javatpoint.com/tutorial/machine-learning/images/decision-tree-classification-algorithm.png)

1. Load the data into the model.

2. Split the data into training and testing sets.

3. Build the decision tree using a suitable splitting criterion such as Gini index, entropy, or information gain.

4. Prune the tree to reduce overfitting.

5. Predict the output for the test data and calculate the accuracy.

6. Tune the hyperparameters such as the maximum depth of the tree, minimum number of samples per leaf, and minimum number of samples per split to improve the model's performance.

7. Evaluate the model using different metrics such as mean squared error (MSE), root mean squared error (RMSE), and R-squared value.


When implementing a decision tree, selecting the best attribute for the root node and sub-nodes can be challenging. This is where Attribute Selection Measures (ASM) come in handy. Two popular techniques for ASM are Information Gain and Gini Index.

Information Gain measures the changes in entropy after segmenting a dataset based on an attribute. It calculates how much information a feature provides about a class, and the algorithm always tries to maximize the value of information gain. Entropy is a metric used to measure the impurity in a given attribute and can be calculated using the formula: 
- Entropy(S) = -P(yes)log2P(yes) - P(no)log2P(no)

where S is the total number of samples, and P(yes) and P(no) represent the probabilities of "yes" and "no," respectively.

Gini Index is another measure of impurity used while creating a decision tree. An attribute with a low Gini index is preferred compared to one with a high Gini index. Gini index only creates binary splits, and the CART algorithm uses it to create binary splits. Gini Index can be calculated using the formula: 

- Gini Index = 1 - ∑jPj2.

![image](https://qph.cf2.quoracdn.net/main-qimg-690a5cee77c5927cade25f26d1e53e77)

Pruning is a process of deleting unnecessary nodes from a tree to obtain the optimal decision tree. A too-large tree increases the risk of overfitting, while a small tree may not capture all the essential features of the dataset. Two main tree pruning technologies used are Cost Complexity Pruning and Reduced Error Pruning. Pruning decreases the size of the learning tree without reducing accuracy.







#Acknowledgements

[decisionTreeRegressor](https://www.javatpoint.com/machine-learning-decision-tree-classification-algorithm)

[article](https://www.saedsayad.com/decision_tree_reg.htm#:~:text=Decision%20tree%20builds%20regression%20or,decision%20nodes%20and%20leaf%20nodes.)
