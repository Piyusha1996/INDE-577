# Single Neuron Network

A single neuron network, also known as a perceptron, is a basic artificial neural network architecture consisting of a single neuron with one or more input connections, one output connection, and a bias term. It is a fundamental building block of more complex neural network models.

![image](https://miro.medium.com/v2/resize:fit:2000/format:webp/1*9fxF0j8fy6mCba5soOGjbw.png)

Algorithm for single neuron network:

- Initialize the weights and bias to random values.
- Input the training data into the network.
- Compute the weighted sum of the inputs.
- Apply an activation function to the weighted sum.
- Compare the output of the activation function with the expected output.
- Adjust the weights and bias according to a learning rate and the error between the expected output and the actual output.
Repeat steps 2-6 for multiple iterations until the error is minimized.

![image](https://miro.medium.com/v2/resize:fit:4800/format:webp/1*yGT6OCJONRoMCSb5u83ZkQ.png)

# Performance analysis parameters:

- Training error: the difference between the predicted output and the actual output during training.
- Testing error: the difference between the predicted output and the actual output on the test set.
- Accuracy: the proportion of correctly classified samples in the test set.
- Precision and recall: measures of the model's ability to correctly identify positive samples and avoid false positives and false negatives.
- F1 score: a measure of the balance between precision and recall.

# Formulas:

- Weighted sum: z = w1x1 + w2x2 + ... + wn*xn + b
- Activation function: a = f(z)
- Error: E = 1/2*(y - a)^2
- Weight update rule: w = w + α*(y - a)*x
- Bias update rule: b = b + α*(y - a)

![image](https://miro.medium.com/v2/resize:fit:1376/format:webp/1*dDZskIHTcTR3BdTLPQtIrg.png)

# Advantages:

- Simple and easy to understand architecture.
- Fast training and prediction times.
- Can be used for binary classification problems.
- Can be used for linearly separable problems.

# Disadvantages:

- Cannot solve non-linearly separable problems.
- Limited in terms of the complexity of the problems it can solve.
- Can suffer from the problem of vanishing gradients when using certain activation functions.
- Prone to overfitting when the number of features is large.

# Limitations:

- Cannot perform well on complex tasks, such as image or speech recognition.
- Limited in terms of the number of layers it can have.
- Cannot learn complex patterns in the data.








# Acknowledgements


[article](https://medium.com/biffures/all-the-single-neurons-14de29a40f47)
