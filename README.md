# Day18-Lab1-EDA2


# What is Logistic Regression

Logistic regression is a machine learning classification algorithm that is used to predict the probability of certain classes based on some dependent variables.

This machine learning technique used for classification or prediction in data sets which have many features, but where most of them have little value and should be ignored.


In short, the logistic regression model computes a sum of the input features (in most cases, there is a bias term), and calculates the logistic of the result.

The output of logistic regression is always between (0, and 1), which is suitable for a binary classification task. The higher the value, the higher the probability that the current sample is classified as class=1, and vice versa.

# Assumptions
 
1- In binary Logistic Regression requires the dependent variable and ordinal logistic regression requires the dependent variable to be ordinal.
2- The observation should not come from repeated measurements or matched data.
3- Logistic regression rejects multicollinearity among the independent variables.
4- It works on assumption of independent linearity. It requires that the independent variables linearly related to the log odds.

# HOW DOES IT WORK ?
Machine learning generally involves predicting a quantitative outcome or a qualitative class. The former is commonly referred to as a regression problem. In the scenario of linear regression, the input is a continuous variable, and the prediction is a numerical value. When predicting a qualitative outcome (class), the task is considered a classification problem.

Not all algorithms fit cleanly into this simple dichotomy, though, and logistic regression is a notable example. Logistic regression is part of the regression family as it involves predicting outcomes based on quantitative relationships between variables. However, unlike linear regression, it accepts both continuous and discrete variables as input and its output is qualitative. In addition, it predicts a discrete class such as “Yes/No” or “Customer/Non-customer”.

In practice, the logistic regression algorithm analyzes relationships between variables. It assigns probabilities to discrete outcomes using the Sigmoid function, which converts numerical results into an expression of probability between 0 and 1.0. Probability is either 0 or 1, depending on whether the event happens or not. For binary predictions, you can divide the population into two groups with a cut-off of 0.5. Everything above 0.5 is considered to belong to group A, and everything below is considered to belong to group B.

A hyperplane is used as a decision line to separate two categories (as far as possible) after data points have been assigned to a class using the Sigmoid function. The class of future data points can then be predicted using the decision boundary.

Logistic regression is named for the function used at core of the method, the logistic function. It is also called the sigmoid function. It is used to describe properties of population growth in ecology, rising quickly and maxing out at the carrying capacity of the environment. It's a three shape curve that can take any value number and map it into a value between 0 and 1, but never exactly at those limits.

We can derive

Sigmoid Function = 1 / 1 + e^-value

where:

e = base of the natural logarithm

It is also used when we can't separate the data into classes by a linear boundary.

From the example:

p / 1 - p

where;

p = probability of an event

We can create formula from this

log p / 1 - p

It was also used in biological science in the early days. It was then used in many social science applications. It is used when the dependent variable is categorical.

Here is a simple model:

Output = 0 or 1

Hypothesis => Z = Wx + B

hҩ(x) = Sigmoid(z)

There are two conditions:

Z = ∞ (infinity)

and

Y(predict) = 1

If Z = -∞

Y(predict) => 0

 
Before we implement any algorithm, we have to prepare data for it. Here are some data preparation methods for logistic regression.

 
# Methodology

Data preparation
Binary output variable
Remove Noise
Gaussian distribution
Remove co-related Inputs

# Advantages

Logistic regression is one of the most efficient techniques for solving classification problems. Some of the advantages of using logistic regression:

Logistic Regression is easy to implement, interpret and very efficient to train. It is very fast at classifying unknown records.
It performs well when the dataset is linearly separable.
It can interpret model coefficients as indicators of feature importance.
 
# Disadvantages

It constructs linear boundaries; logistic regression needs that independent variable are linearly related to the odds.
The major limitation of logistic regression is the assumption of linearity between the dependent variable and the independent variable.
More powerful and compact algorithms such as neural networks can easily outperform this algorithm.
 

# Conclusion
 
Logistic regression is one of the traditional machine learning methods. It forms a foundational set of ML approaches alongside algorithms such as linear regression, k-suggest clustering, major component analysis, and a few others. Neural networks have been developed leveraging logistic regression. You can efficiently use logistic regression even if you are not an ML specialist, not the case with many other algorithms. Conversely, it is not possible to become an ML master without a solif understanding of logistic regression.


References:
https://www.kdnuggets.com/2022/07/logistic-regression-work.html
https://www.kdnuggets.com/2022/02/overview-logistic-regression.html
