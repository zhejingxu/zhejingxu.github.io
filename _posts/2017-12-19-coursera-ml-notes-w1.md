---
layout: post
title:  "Coursera ML Learning Notes"
date:   2017-12-19 23:06:11 +0800
categories: Machine Learning
---

## 1. First Week

### 1.1 Introduction
1. Supervised Learning: Given a data set and correct output, find the relationship between the intput and output.
  * Regression: Predict results within a continuous output
  * Classification: Predict results in a discrete output
2. Unsupervised Learning: Derive the structure from data, no feedback based on prediciton results.
  * Clustering: Find a way to automatically group the data
  * Non-clustering: "Cocktail Party Algorithm"

### 1.2 Model and Cost Function
Cost Function: Used to measure the accuracy of our hypothesis function. It's also called 'Squared Error Function'.
![Cost Function]({{ site.url }}/assets/cost_function.png)

### 1.3 Parameter Learning
Gradient Descent Algorithm is used to estimate the parameters in hypothesis function.
![Gradient Descent Algorithm]({{ site.url }}/assets/gradient_descent_algorithm.png)
Alpha is 'Learning Rate' and Updating the theta 0 and theta 1 simultaneously is important.

Gradient Descent can converge to a local minimum, even with the learning rate fixed. As we approach a local minimum, gradient descent will automatically take smaller steps. So, no need to decrease alpha over time.
![Gradient Descent For Linear Regression]({{ site.url }}/assets/gradient_descent_for_linear_regression.png)
When we use every example in the entire training set on every step, it's called Batch Gradient descent.


## 2. Second Week
### 2.1 Multivariate Linear Regression
Multivariable denotion
![Multivariable denotion]({{ site.url }}/assets/multivariable_denotion.png)

Multivariable hypothesis
![Multivariable hypothesis]({{ site.url }}/assets/multivariable_hypothesis.png)

Multivariable hypothesis Function
![Multivariable hypothesis Function]({{ site.url }}/assets/multivariable_hypothesis_function.png)

### 2.2 Gradient Descent for Multiple Variables
Gradient Descent for Multiple Variables
![Gradient Descent for Multiple Variables]({{ site.url }}/assets/gradient_descent_for_multiple_variables.png)

### 2.3 Feature Scaling
Having the input values in the same range helps speeding up gradient descent and so we have two method: feature scaling and mean normalization.
Feature Scaling: Divide the input value by the range - > [0, 1]
Mean Normalization:
![Mean Normalization]({{ site.url }}/assets/mean_normalization.png)
μ is the average of the values for feature
s is the range of values (max - min), it means standard deviation.

### 2.4 Learning Rate
It has been proven that if learning rate α is sufficiently small, then J(θ) will decrease on every iteration.
If α is too small: slow convergence.
If α is too large: ￼may not decrease on every iteration and thus may not converge.

