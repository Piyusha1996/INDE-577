
# Gradient descent

Gradient Descent (GD) is an optimization algorithm commonly employed in machine learning to minimize a model's cost function. GD iteratively adjusts the model's parameters or weights in the direction of the cost function's negative gradient until the minimum cost is attained.

Various GD variants exist, which differ in the method for selecting the step size or learning rate and in the way updates are made. Below are some common variants:


![image](https://blog.paperspace.com/content/images/2018/05/convex_cost_function.png)


## Type of Gradient Decent
- Batch Gradient Descent: Computes the gradient and updates the parameters using the entire training dataset in each iteration, potentially yielding a more accurate model. However, this approach can be slow for large datasets.
- Stochastic Gradient Descent (SGD): Computes the gradient and updates the parameters using only one training example at each iteration. SGD can be faster than batch gradient descent but may result in more noise in the updates.
- Mini-batch Gradient Descent: Computes the gradient and updates the parameters using a small batch of training examples at each iteration. This approach can be a compromise between batch gradient descent and SGD, as it can be faster than batch gradient descent and less noisy than SGD.
- Momentum-based Gradient Descent: Incorporates a momentum term in the gradient update to smooth out the update process and hasten convergence, preventing the optimization process from getting trapped in local minima.
- Adaptive Learning Rate Methods: Adaptive methods, such as Adagrad, RMSProp, and Adam, adjust the learning rate based on the past gradients to enhance convergence and prevent oscillations, particularly in deep learning or problems with sparse gradients.
- Conjugate Gradient Descent: CGD is a variant of GD that can solve large-scale optimization problems with a symmetric and positive definite matrix more efficiently, using fewer iterations and memory than other GD methods.

The choice of which GD variant to use depends on the specific problem and available computing resources. GD is a powerful optimization algorithm and a popular choice for algorithms like linear regression, logistic regression, and neural networks.
## Equation used:
![image](https://miro.medium.com/v2/resize:fit:330/1*GixQ9i6cQSvlfoe_XZdcog.gif)

The Gradient Descent Algorithm is an iterative process that involves calculating the next point using the gradient at the current position. The obtained value is then scaled by a learning rate and subtracted from the current position to make a step. This is done to minimize the function since adding it would maximize it. The learning rate, denoted as η, is an important parameter that scales the gradient and determines the step size. In machine learning, the learning rate strongly influences the algorithm's performance.

If the learning rate is too small, the Gradient Descent Algorithm may take longer to converge, or it may even reach the maximum iteration before reaching the optimal point. Conversely, if the learning rate is too large, the algorithm may not converge to the optimal point, and it may jump around or even diverge completely.
## Acknowledgements

 - https://www.geeksforgeeks.org/gradient-descent-algorithm-and-its-variants/
 - https://blog.paperspace.com/intro-to-optimization-in-deep-learning-gradient-descent/
