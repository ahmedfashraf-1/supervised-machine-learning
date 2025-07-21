# Supervised Machine Learning

This repository contains basic implementations of Supervised Machine Learning algorithms using Python and NumPy. It includes:

- 📈 Linear Regression
- 🌀 Polynomial Regression
- 💰 Cost Function
- 📉 Gradient Descent

---

## 📘 Linear Regression

Linear Regression is a fundamental algorithm used to model the relationship between a dependent variable `y` and an independent variable `x` by fitting a straight line.

The equation of the line is:


Where:
- `w` is the weight (slope)
- `b` is the bias (intercept)

The goal is to find the best `w` and `b` that minimize the error between predicted and actual values.

---
## 🧮 Multiple Linear Regression

Multiple Linear Regression is an extension of simple linear regression, where the model predicts the target variable `y` based on **multiple input features** instead of just one.

The general form of the equation is:
Where:
- `x1, x2, ..., xn` are input features
- `w1, w2, ..., wn` are their corresponding weights
- `b` is the bias (intercept)

This model is useful when the output depends on more than one factor. For example, predicting house price based on size, location, and number of rooms.

Just like in simple regression, we use gradient descent or other optimization methods to learn the best parameters.
---
## 🌀 Polynomial Regression

Polynomial Regression is an extension of linear regression that fits a non-linear curve to the data by introducing higher-degree terms of the input variable `x`.

## 💰 Cost Function (Mean Squared Error)

The cost function measures how well the model is performing by calculating the average of the squared differences between predicted and actual values:
Where:
- `m` is the number of training examples
- `y_pred` is the predicted output
- `y_actual` is the true label

The goal is to minimize the cost function as much as possible.

---

## 📉 Gradient Descent

Gradient Descent is an optimization algorithm used to minimize the cost function by updating the model parameters `w` and `b` iteratively.

Update rules:
Where:
- `α` is the learning rate (a small constant)
- `∂J/∂w` and `∂J/∂b` are gradients (partial derivatives)

It moves the parameters in the direction of the negative gradient to reduce the cost.
