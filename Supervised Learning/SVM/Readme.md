# Support Vector machine
Support Vector Machine (SVM) is a machine learning algorithm that is primarily used for classification problems. SVM works by finding the best possible decision boundary that separates the data points into different classes.

What is Support Vector Machine?

Support Vector Machine is a machine learning algorithm that works on the principle of finding the best possible decision boundary that separates the data points into different classes. SVM can be used for both classification and regression problems.

![image](https://miro.medium.com/v2/resize:fit:600/format:webp/0*9jEWNXTAao7phK-5.png) ![image](https://miro.medium.com/v2/resize:fit:600/format:webp/0*0o8xIA4k3gXUDCFU.png)


# Hyperplanes and Support Vectors:

The decision boundary that separates the data points is known as the hyperplane. In SVM, we find the hyperplane that maximizes the margin, i.e., the distance between the hyperplane and the closest data points from both the classes. The closest data points are known as the support vectors.

![image](https://miro.medium.com/v2/resize:fit:1400/format:webp/1*ZpkLQf2FNfzfH4HXeMw4MQ.png)



# Large Margin Intuition:

The idea behind SVM is to find a hyperplane that maximizes the margin between the closest data points from both the classes. This is because a larger margin leads to better generalization, and the model is less likely to overfit the training data.

# Cost Function and Gradient Updates:

In SVM, we use a cost function to penalize the misclassification of the data points. The cost function is optimized using gradient descent, and the hyperplane is updated iteratively.

![image](https://miro.medium.com/v2/resize:fit:886/format:webp/1*3xErahGeTFnbDiRuNXjAuA.png)


![image](https://miro.medium.com/v2/resize:fit:1400/format:webp/1*GQAd28bK8LKOL2kOOFY-tg.png)

SVM Implementation in Python:

SVM can be implemented in Python using various machine learning libraries, such as Scikit-Learn, Keras, TensorFlow, and PyTorch. Scikit-Learn provides an SVM implementation that is easy to use and is widely used in the industry. The implementation involves selecting the kernel function, tuning the hyperparameters, and fitting the SVM model to the training data.

There are several evaluation metrics that can be used to measure the performance of an SVM model:

1. Accuracy: This is the most commonly used metric for evaluating the performance of classification models. It is the ratio of correctly classified instances to the total number of instances.

2. Precision and Recall: Precision is the ratio of true positives to the total number of predicted positives, while recall is the ratio of true positives to the total number of actual positives. These metrics are useful when the classes are imbalanced.

3. F1 Score: This is the harmonic mean of precision and recall. It provides a single score that balances both precision and recall.

![image](https://datascience103579984.files.wordpress.com/2019/04/capture3-24.png)

4. Confusion Matrix: This is a table that summarizes the performance of a classification model. It shows the number of true positives, false positives, true negatives, and false negatives.

5. ROC Curve: Receiver Operating Characteristic (ROC) curve is a plot of the true positive rate against the false positive rate. It is used to evaluate the performance of binary classifiers.

![image](https://scikit-learn.org/0.15/_images/plot_roc_0012.png)

6. AUC Score: Area Under the ROC Curve (AUC) is a measure of the performance of a binary classifier. It represents the probability that a positive instance is ranked higher than a negative instance.

These metrics can be calculated using various libraries in Python, such as Scikit-learn.







#Acknowledgements

[SVM](https://towardsdatascience.com/support-vector-machine-introduction-to-machine-learning-algorithms-934a444fca47)

[article](https://datascience103579984.wordpress.com/2019/04/30/balanced-accuracy-and-f1-score/)
