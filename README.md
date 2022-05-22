# Logistic Regression

  **Note:** *This is a presentation of the logistic regression model and uses sources cited at the bottom of the page*

## Introduction

Logistic Regression is a simple **machine leaning** model that is used with the condition that the dependent variable, meaning the target, is **categorical**.<br> 
It is also used in both Machine Learning and Mathematical Statistics as a modeling of probability of a discrete outcome given an input variable.<br>
For example Logistic Regression can predict if an email is spam (output of 1) or not (output of 0). A Machine Learning model that's often compared to Logistic Regression is Linear Regression. The difference is that this model predicts with an output of 0 or 1, whereas the latter outpus a percentage of likelihood.

## Model

Output = 0 or 1<br>
Hypothesis: ``Z = WX +B``<br>
hⲑ(x) = sigmoid(Z)<br>

## How it works

#### a. *Linear Regression*

Consider if we need to classify if an email is spam (output 1), or not (0). If we use the linear regression model, we will need to setup a threshold to setup which classification can be done. For instant if we get a prediction of 0.4, and our threshold is 0.5, then the concerned email will be classified as not spam. Same goes fore any prediction above 0.5, which will be considered spam.<br>
Linear regression is not suitable for this kind of proble because it is unbounded with its values ranging from 0 to 1 with all the values in between. This is why we use Logistic regression which outputs a predition of 0 or 1 using the Sigmoid Function.

#### b. *Logisitc Regression*

##### Analysis of the Hypothesis *(Z = WX + B)*

The output from the Hypothesis above is the estimated probability of classification. This is then used to infer how confident can the predicted value be the same as the actual value with an input ``X``.<br>
For instance if the value X is ```X = [x0 x1] = [1 IP-Address]``` and if we obtain base of x1 a probability of 0.8, then this means that there is an 80% chance that the email is spam.

##### Mathematical Analysis

```hⲑ(x) = P(Y=1|X; theta)``` In words, hⲑ(x) is the probability that Y=1, given X, which has theta as the parameter.<br>
Similarly, ```P(Y=1|X; theta) + P(Y=0|X; theta) = 1``` which inducts that: ```P(Y=0|X; theta) = 1 - P(Y=1|X; theta)```.

##### Types of Logistic Regression

- *Binary Logistic Regression:* 2 possible outcomes, ex: spam or not
- *Multinominal Logistic Regression:* Threee or more categories without ordering, ex: Veg, Non-Veg, Vegan.
- *Ordinal Logistic Regression:* Three or more categories with ordering, rating movies from 1 to 5.



## Sources

1. [Science Direct](https://www.sciencedirect.com/topics/computer-science/logistic-regression)
2. [Towards Data Science](https://towardsdatascience.com/logistic-regression-detailed-overview-46c4da4303bc)

