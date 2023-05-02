# Random Forest

![image](https://1.bp.blogspot.com/-cq_HrPq0qeg/XtZYm_rlUpI/AAAAAAAAEkE/z1dL1TKk0cUJy6ympLUX1fM2t0XRnkJuQCNcBGAsYHQ/s1600/decisiontree_and_randomforest.png)

What is Random Forest?

Random Forest is an ensemble learning algorithm that combines multiple decision trees to improve the accuracy of predictions. Each tree in the forest is built using a random subset of features and a random subset of data samples, and the final prediction is made by averaging the predictions of all trees.

![image](https://cdn.analyticsvidhya.com/wp-content/uploads/2020/02/rfc_vs_dt1.png)

Algorithm for Random Forest:

- Choose the number of trees to include in the forest.
For each tree:
- a. Randomly select a subset of features to use for building the tree.
- b. Randomly select a subset of data samples to use for building the tree.
- c. Build the decision tree using the selected features and samples.
- To make a prediction for a new input, pass the input through each tree in the forest and average the predictions.

# Advantages:

- Random Forest is highly accurate and can work well with both numerical and categorical data.
- It can handle missing data and maintain accuracy with a large number of input variables.
- It can handle large datasets with high dimensionality and is not easily overfitting.
- It can be used for classification and regression tasks.

# Disadvantages:

- Random Forest models can be slow to train and evaluate, especially with large datasets and many trees.
- They can be difficult to interpret, as the output is a combination of many individual trees.
- Random Forest models can be sensitive to noise in the data.

# Limitations:

- Random Forest can sometimes produce biased results if the dataset is imbalanced.
- It may not be as effective as other algorithms for identifying complex relationships between variables.
- Random Forest may not work well with very high-dimensional data.

# Performance analysis parameters and formulas:

- The accuracy of Random Forest can be measured using metrics such as classification accuracy, precision, recall, F1 score, and ROC AUC.

![image](https://scikit-learn.org/stable/_images/sphx_glr_plot_roc_curve_visualization_api_002.png)


- The performance of Random Forest can be improved by adjusting hyperparameters such as the number of trees, the maximum depth of each tree, and the number of features to consider at each split.
- The complexity of Random Forest can be analyzed using the number of trees, the number of nodes in each tree, and the number of features used.










