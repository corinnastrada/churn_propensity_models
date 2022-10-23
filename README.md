# churn_propensity_models

DATASET:

It was provided by a company working in the intertainment industry.
Theare are 330586 observations and 102 variables.
Every observation provides information about the behaviour of an user on the web page of the company.


PREPROCESSING:

To prepare data for the ML algorithms, the following operations have been carried out:
- Data Cleaning / Aggregation
- Study of the Correlation 
- Zero Variance and NearZero Variance Analysis


DATASET SPLITTING:

The original dataset has been splitted into Training - Test - Validation.
Then, to balance the distribution of the target variable into the 3 datasets, the SMOTE funcion has been implemented.


MODEL TRAINING:

The classifications models have been implemented with the goal of maximizing Specificity, so in order to find in the most accurate way the clients 
who leave the company.

The models trained are: 
- Classification Tree
- Random Forest
- Logistic Model 
- Bagging Tree
- Naive-Bayes
- Gradient Boosting
- Neural Network Single-Layer Perceptron
- Neural Network Multi-Layer Perceptron


CHOICE OF THE BEST MODEL:

To find the winning model, both the Cumulative Gain and Lift Curve have been examined (in particular, the second decile of them).

The winning model is the Random Forest.

In the first 20% of the population, the model is able to capture 57.2% of the churners.
Also, by selecting the first 20% of the customers, the probability that one of them is a churner is 2.86 times the global one.

