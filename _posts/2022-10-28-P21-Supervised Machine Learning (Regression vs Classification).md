---
title: "Supervised Machine Learning (Regression vs Classification)"
categories:
    - Blog
tags:
    - Machine Learning
toc: true
toc_label: "Table of Contents"
toc_icon: "cog"
toc_sticky: true
excerpt: "An overview on Regression versus Classification"
---

## 1.0 Supervised Machine Learning 
> Types of machine learning algorithms that makes predictions based on given examples (training data). 

## 2.0 Learning Rate 
> A tuning parameter that is essentially the step size of each optimization iteration while moving toward a minimum of loss function. 

## 3.0 Regularization 
> A process of encouraging a learning algorithm to shrink the weights (importance) of the parameters without necessarily demanding that the parameter is set to exactly zero. In simpler terms, adding large regularization term to the cost function reduces the weight, w of an algorithm.


![Regularization Expression](https://user-images.githubusercontent.com/79191009/198671127-22bfb5be-26a5-4833-8c87-7c488292af8b.png)

## 4.0 Symbols 
![Symbols_1](https://user-images.githubusercontent.com/79191009/198671899-d8eef0bc-7a52-4da9-888b-3fe712cc5644.png)

![Symbols_2](https://user-images.githubusercontent.com/79191009/198672051-911abdfe-b078-4d62-9c17-e362729addbe.png)


## 5.0 Summary of Comparison Between Regression and Classification 
### 5.1 Definition
#### 5.1.1 Regression
> Regression is an algorithm to predict a number from an infinitely many possible numbers (Continuous).

#### 5.1.2 Classification
> Classification is an algorithm to predict categories or classes (Discrete).

### 5.2 Simplest Model
#### 5.2.1 Regression
* Multiple Linear Regression & Vectorized Form

![Multiple Linear Regression](https://user-images.githubusercontent.com/79191009/198672821-ed80dc59-64b8-4d58-9f89-f148f13e66c8.png)

#### 5.2.2 Classification
* Logistic Regression (Sigmoid Function)

![Sigmoid Function](https://user-images.githubusercontent.com/79191009/198672763-c86c256c-3f4e-4244-89e9-b3773aa2199d.png)

### 5.3 Simple Cost Function
#### 5.3.1 Regression
* Squared Error

![Squared Error](https://user-images.githubusercontent.com/79191009/198673137-65d08d54-fa0b-4ba6-a7fe-0f7154ff123a.png)

* [Covex](https://www.coursera.org/learn/machine-learning) Shape

![image](https://user-images.githubusercontent.com/79191009/198675150-771bc0c9-f3f0-44c2-a1ff-e3001aaa6024.png)

#### 5.3.2 Classification
* Simplified Loss Function (derived from [Maximum Likelihood Estimation](https://en.wikipedia.org/wiki/Maximum_likelihood_estimation#:~:text=In%20statistics%2C%20maximum%20likelihood%20estimation,observed%20data%20is%20most%20probable.))

![Simplified Cost Function](https://user-images.githubusercontent.com/79191009/198673214-b1df0dbd-1aae-43fd-8caf-86c6dbdfbabe.png)

* [Discontinuous](https://www.researchgate.net/figure/Cost-function-for-Logistic-Regression_fig3_342720152) Shape

![image](https://user-images.githubusercontent.com/79191009/198675379-88ad07f5-322e-42c4-aed4-7cdbc038eaef.png)

### 5.4 Modified Cost Function (Regularization)
#### 5.4.1 Regression

![image](https://user-images.githubusercontent.com/79191009/198675505-cf8f1f90-5c80-4949-98e7-274cf32cad69.png)

#### 5.4.2 Classification

![image](https://user-images.githubusercontent.com/79191009/198675561-fb5abd6f-bd4c-4af6-a7b7-823270c78344.png)

### 5.5 Gradient Descent
#### 5.5.1 Regression
* Goal: Minimisze ***J(w,b)***

![image](https://user-images.githubusercontent.com/79191009/198675678-33f27a4b-b27b-4d6d-93e1-8da4ee233c40.png)

#### 5.5.2 Classification
* Goal: Minimisze ***J(w,b)***. Looks the same as regression, just function ***f*** definition is different

![image](https://user-images.githubusercontent.com/79191009/198675684-6aa47e64-7352-4850-ab30-5473d2f8182c.png)

### 5.6 Modified Gradient Descent
#### 5.6.1 Regression

![image](https://user-images.githubusercontent.com/79191009/198675989-e8b74e2c-6335-4785-a0d7-a63cf2da5fc9.png)

#### 5.6.2 Classification
* Looks the same as regression, just function ***f*** definition is different

![image](https://user-images.githubusercontent.com/79191009/198676017-ba0350dc-7451-4ee8-8e9c-21e36610b5c3.png)


---
## References
[1] "Supervised Machine Learning: Regression and Classification," *Coursera*. [Online]. https://www.coursera.org/learn/machine-learning. (Accessed: Oct 28, 2022)

[2] A. E. Yilmaz, "A Taxonomy of Artificial Neural Networks," M. S. Thesis, Department of Mathematics, Koc University, Instanbul, 2020. [Online]. Available: https://www.researchgate.net/publication/342720152_A_Taxonomy_of_Artificial_Neural_Networks

