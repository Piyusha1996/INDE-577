
# Logistic Regression

Logistic regression is a statistical method for analyzing a dataset in which there are one or more independent variables that determine an outcome. It is a type of regression analysis used for predicting the outcome of a categorical dependent variable based on one or more predictor variables. The output is a probability value between 0 and 1, indicating the likelihood of the outcome being a particular category.

There are two main types of logistic regression: binary logistic regression and multinomial logistic regression. Binary logistic regression is used when the dependent variable has only two categories, while multinomial logistic regression is used when there are more than two categories.


![image](https://www.saedsayad.com/images/LogReg_1.png)


## Advantages & Disadvantages
Advantages of logistic regression include:

1. It is a simple and easy-to-understand method.
2. It can handle non-linear relationships between the independent and dependent variables.
3. It can handle both continuous and categorical independent variables.
4. It provides the probability of the outcome, rather than just a binary classification.

Disadvantages of logistic regression include:

1. It assumes that the independent variables are not highly correlated with each other.
2. It can be sensitive to outliers in the dataset.
3. It is not suitable for complex relationships between the independent and dependent variables.
4. It assumes that the relationship between the independent and dependent variables is linear.


##The functions used in logistic regression include:

1. Sigmoid function: This is the activation function used in logistic regression. It converts any input value into a probability value between 0 and 1.

![image](https://studymachinelearning.com/wp-content/uploads/2019/09/sigmoid_graph.png)



2. Cost function: This function is used to calculate the error between the predicted output and the actual output. The most commonly used cost function is the binary cross-entropy function.

![image](https://miro.medium.com/v2/resize:fit:783/1*6oBgYMy4wOls9zGC-frSQg.png)

3. Gradient descent: This is the optimization algorithm used to minimize the cost function. It iteratively adjusts the weights of the model to find the minimum value of the cost function.

![image](https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcSMvTLPtKbOf4W-Biynhps4L41qHRUuFefhtQ&usqp=CAU)

The error function
The error function in logistic regression is the cost function, which measures the difference between the predicted output and the actual output. The binary cross-entropy function is commonly used as the cost function in binary logistic regression. It penalizes the model more heavily for making incorrect predictions, and less heavily for making correct predictions.

The accuracy function
The accuracy function measures the overall performance of the model in predicting the correct outcome. It is calculated as the percentage of correct predictions over the total number of predictions made. In binary logistic regression, the accuracy function is commonly used to evaluate the performance of the model. However, it is important to also consider other metrics such as precision, recall, and F1 score, especially in imbalanced datasets.
## Acknowledgements

 - https://medium.com/analytics-vidhya/derivative-of-log-loss-function-for-logistic-regression-9b832f025c2d
