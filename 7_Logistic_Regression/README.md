# Logistic Regression
- Classification algorithm
- Binary classification
- Sigmoid function between 0 & 1
- Extension of linear regression

### Output
- Yes/No OR 0/1 OR True/False
- Gives prob. value not exact 0 or 1
- Threshold value needs to be decided.

### Types
- Binomial
- Multinomial
- Ordinal (order is important)

### Assumptions
- Independent Observations
- Binary dependent
- Linearity relationship between independent variables and log odds
- No outliers
- Large sample size

### Terminology Alert
- Odds
- Logistic Function
- Log-odds
- Maximum Likelihood estimation

### The workings
- The sigmoid function transforms the real values of independent variables input into value between 0 and 1.
- Apply multi-linear function with input, weights and bias:
    - z = _w_.X + _b_
- Use z as the input for the sigmoid function

## Multinomial Logistic Regression
- Use softmax function instead of sigmoid function

### Evaluation methodologies for Logistic Regression Model
- Accuracy
- Precision : Focuses on the accuracy of positve predictions
- Recall / Sensitivity / True Positive Rate : Proportion of coreectly predicted positive instances among all actual positive instances
- F1 Score : harmonic mean of precision and recall = 2 * Precision * Recall / (Precision + Recall)
- AUC-ROC (Area under the receiver operating characterics curve)
- AUC-PR (Area under the Precision-Recall Curve)

>[!Note]
>Precision and Recall values greatly affect the selection of threshold values
>Ideally way aim for precision recall value being 1

# Cost function
- Cost function is a mathematical function that calculates the difference between the target actual values and the predicted values. 
### Cross Entropy Loss / Log Loss
- J = - yi * (log(h(x)) + (1-yi)(log(1-h(x)))
