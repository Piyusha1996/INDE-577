# Linear Regression

![image](https://pimages.toolbox.com/wp-content/uploads/2022/04/07040339/25-4.png)

Linear regression is a statistical method frequently used in machine learning and data science to analyze the linear relationship between two variables, namely an independent variable and a dependent variable. The algorithm helps to forecast future outcomes by predicting how fluctuations in the independent variable will affect the dependent variable.

The independent variable, also known as the predictor or explanatory variable, remains constant as other variables change. Conversely, the dependent variable changes as the independent variable fluctuates. The regression model predicts the value of the dependent variable, which is the outcome variable being studied or analyzed.

Linear regression is a supervised learning algorithm that predicts continuous or numeric variables, such as age, salary, product price, and sales, by simulating a mathematical relationship between variables. It is a useful method for stock market forecasting, scientific analysis, and portfolio management when there are at least two variables available in the data.

The linear regression model is represented by a straight line with a slope, which can be used to make predictions for new data points. The line of regression is the best-fit line that represents the linear relationship between the independent and dependent variables.

Linear regression has several benefits that make it a valuable algorithm for predictive analysis. Here are some key benefits of linear regression:

- Simplicity: Linear regression is a straightforward algorithm that is easy to understand and interpret, making it a popular choice for beginners in data   science and machine learning.

- Interpretability: The linear regression model provides interpretable coefficients that allow us to understand how each independent variable affects the dependent variable.

- Predictive accuracy: Linear regression can provide accurate predictions for continuous or numeric variables, making it a valuable tool for forecasting.

- Versatility: Linear regression can be applied to a wide range of applications, such as financial forecasting, scientific analysis, and market research.

- Efficiency: Linear regression is a computationally efficient algorithm that can handle large datasets and complex models.

- Outlier detection: Linear regression can detect outliers, which are data points that deviate significantly from the rest of the dataset, and can help in identifying and removing them.

- Feature selection: Linear regression can help in identifying the most important features that affect the dependent variable, allowing us to focus on the most relevant variables.

There are also a few evaluation metrics for regression:
- R^2 aka the "coefficient of determination": the most common metric, is the ratio of variation to the total variation (equation below - SS_res is the residual sum of squares and SS_tot is the total sum of squares). The value will be between 0 and 1; the closer to 1, the better the model. However, as the number of features increases, the value of R^2 increases and gives the (sometiems false) illusion of a good model.

![image](https://editor.analyticsvidhya.com/uploads/74264r2.png)

- Adjusted R^2: improvement to R^2, only considers features that are important for the model and shows the real improvement of the model. The equation is detailed below

![image](https://editor.analyticsvidhya.com/uploads/80741adjusted%20r2.png)

- Mean Squared Error (MSE)

![image](https://editor.analyticsvidhya.com/uploads/42113mse.jpg)

- Root Mean Squared Error (RMSE): root of the mean difference between actual and predicted values. It penalizes large errors

![image](https://editor.analyticsvidhya.com/uploads/69457rmse.png)


The above information was largely baesd on [this article](https://www.analyticsvidhya.com/blog/2021/05/all-you-need-to-know-about-your-first-machine-learning-model-linear-regression/), which can be referenced for further reading.
