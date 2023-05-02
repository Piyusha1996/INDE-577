
# Perceptron

Perceptron is a type of artificial neural network that is used for supervised learning of binary classifiers. It was introduced by Frank Rosenblatt in 1957 and is considered the simplest type of neural network.

The perceptron model consists of input values and their weights, the sum of all weighted input, and an activation function. The activation function applies a step rule to check whether the weighted sum of inputs is greater than zero or not. If the sum is greater than zero, the output is 1; otherwise, it is 0.

![image](https://static.javatpoint.com/tutorial/machine-learning/images/perceptron-in-machine-learning2.png)


There are two types of perceptron models based on the layers: single-layer perceptron and multi-layer perceptron. A single-layer perceptron model consists of a feed-forward network with a threshold transfer function, and it is used to analyze linearly separable objects with binary outcomes. It can only learn linearly separable patterns.

![image](https://miro.medium.com/v2/resize:fit:563/1*4_BDTvgB6WoYVXyxO8lDGA.png)

On the other hand, a multi-layer perceptron model has a greater number of hidden layers and is also known as the backpropagation algorithm. It has greater processing power and can process both linear and non-linear patterns. It can also implement logic gates such as AND, OR, XOR, NAND, NOT, XNOR, NOR. It is used to solve complex non-linear problems.

The perceptron function can be achieved as output by multiplying the input with the learned weight coefficient. The weight coefficient is automatically learned by the algorithm, and the linear decision boundary is drawn, enabling the distinction between the two linearly separable classes +1 and -1.

Perceptron has certain limitations, such as it can only classify linearly separable sets of input vectors, and the output can only be a binary number due to the hard limit transfer function.

Perceptrons are trained in three phases:

**1. Data Processing**

  As a binary classifier, perceptrons are meant to classify input into two groups: yes/no, black/white, up/down, etc, corresponding to 1/0 or 1/-1 outputs (depending on the selected activation function). To prepare data, we must first determine the two output groups and classify data in numerical terms, at which point the data will be in a format that will allow the perceptron to be trained. 
  
**2. Predict Results**

![image](https://cdn.analyticsvidhya.com/wp-content/uploads/2020/02/13UpdymQx-C1tBKRnfD7eOg.gif)

The perceptron learning rule states that the algorithm would automatically learn the optimal weight coefficients. The input features are then multiplied with these weights in a weighted sum to determine if the neuron "fires" or not (returns 1 if positive, 0 otherwise, or 1 and -1).

![image](https://user-images.githubusercontent.com/89811204/146212310-d319e5d3-7cf9-4ef6-9525-7114c1f8db4c.png)

In the equation above:
- w: vector of real valued weights
- b: bias (an element that adjusts the boundary away from the origin without any dependence on the input value
- x: vector of input values

![image](https://user-images.githubusercontent.com/89811204/146212640-e65cef67-2d62-4d45-9245-3239cde4d8c6.png)

- m: number of inputs to the percpetron

![image](https://www.simplilearn.com/ice9/free_resources_article_thumb/Perceptron/Perceptron_17.jpg)

Choose an activation function

![image](https://www.simplilearn.com/ice9/free_resources_article_thumb/Perceptron/Perceptron_9.jpg)

- [Heaviside step function](https://en.wikipedia.org/wiki/Heaviside_step_function): triggered above a certain value of neuron output; otherwise it outputs zero
- Sign function: outputs +1 or -1 depending whether the neuron output is greater than 0 or not
- Sigmoid: S-curve that outputs a value between 0 and 1 (using [Logistic Regression](https://github.com/Madison-Bunting/INDE-577/tree/main/supervised%20learning/2%20-%20logistic%20regression))

**3. Update Weights**

The goal is to reduce the number of misclassified points, so by iterating through the algorithm, the separation line moves in space and after a few epochs, the algorithm classifies it correctly.

In the Perceptron learnning rule, predicted output is compared with known output; if they do not match, error is propagated backward to allow weight adjustment to happen

The future of perceptron technology is bright and significant as it helps to interpret data by building intuitive patterns and applying them in the future. It is continuously becoming more advanced and working efficiently on complex problems with the help of artificial neurons.

![image](https://pbs.twimg.com/media/FXo8u7JaQAANoNm.png)

In conclusion, perceptron models are continuously contributing to artificial intelligence and machine learning, and these models are becoming more advanced. Perceptron enables computers to work more efficiently on complex problems using various machine learning technologies. It is the fundamental of artificial neural networks, and it is essential to have in-depth knowledge of perceptron models to study deep neural networks.
## Acknowledgements

 - https://www.javatpoint.com/perceptron-in-machine-learning
