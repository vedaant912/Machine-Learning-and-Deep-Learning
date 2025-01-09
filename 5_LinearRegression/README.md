## Linear Regression Explained
- It is a supervised machine-learning algorithm.
- Uses a labelled dataset and learns a linear function which results into minimum loss and helps to further make predictions on new data points.
- This is one of the simplest type of Regression.

### Definition
- It computes a linear relationship between the dependent variable and one or more independent features by fitting a linear equation to given data.
- **Simple Linear Regression** & **Multiple Linear Regression**
- _Univariate Linear Regression_ & _Multivariate Regression_

### Importance
- It is interpretable.
- The transparency of the equation where it shows how much the dependent variable is affected by indivdual independent variables.
- Basis for more advance algorithms.

### Goal
- Find the best fit line equation that can predict the values based on the independent variables.
- The best fit line is such that it minimizes the error between the predicted and the actual values. There will be least error.
- What does slope represent? : _How much dependent variable changes for a unit change in independent variable._
- Y : Dependent Variable, X : Independent Variable

### Hypothesis function
- Get best theta_1 (y-intercept) and theta_2 (slope) value for the given dataset.
- Values for above parameters should be selected in such a way that the differenc between y and y_pred is minimum.

### Cost Function
- Also known as loss function.
- In Linear Regression, Mean Squared errror (MSE) is used as loss function.
- It calculates the average of the squared errors between y and y_pred.
- The cost function is defined as: J = (1/n) Σᵢ=₁ⁿ ( (ŷᵢ - yᵢ)² )
- Using MSE function, the iterative process of Gradient Descent is applied to update the value of parameters.
- To converge to global minima.

### Gradient Descent for Linear Regression
- It is an optimization algorithm.
- A gradient is : _A derivative of the cost function that defines the effects on outputs of the function with a little bit variation in inputs._
- Move in the direction of the MSE negative gradient with respect to coefficient (parameters), the coefficient can be changed.

### Assumption of Simple Linear Regression
- **Linearity** : It is assumed that the depenedent and independent variables are linearly related. If this is not fulfilled in the dataset then the Linear Regression model won't be accurate.
- **Independence** : The observations in the dataset are indepenedent of each other. Value of dependent variable for one observation does not depenct on the value of dependent variable for another observation.
- **Homoscedasticity** : This indicates that the amount of the independent variables has no impact on the variance of the errors. If the variance of the error residuals is not constant, the linear regression will not be accurate.
- **Normality** : The residuals should be normally distributed.
> [!NOTE]
> If the dataset doesnot follow above assumptions, it means that the linear regression wouldn't be the best model for prediction.

### Assumption of Multiple Linear Regression
- Previous assumptions apply
- Additional
    - No multicollinearity
    - Additivity
    - Feature Selection
    - Overfitting