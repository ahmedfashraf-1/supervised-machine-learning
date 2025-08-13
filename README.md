# Supervised Machine Learning

This repository contains basic implementations of Supervised Machine Learning algorithms using Python and NumPy. It includes:

- 📈 Linear Regression
- 🧮 Multiple Linear Regression
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

## 🧠 Logistic Regression
Logistic Regression is a statistical algorithm mainly used for classification tasks, rather than predicting continuous values.
It uses the Sigmoid Function to map the linear output into probabilities between 0 and 1.

The Sigmoid function is defined as:
- σ(z) = 1 / (1 + e^(-z))
- Where:

z = w·x + b is the linear combination of inputs.

The output σ(z) represents the probability of belonging to a certain class

💰 Cost Function (Log Loss / Binary Cross-Entropy)
In Logistic Regression, the cost function is defined as:

J(w,b) = - (1/m) Σ [ y·log(y_pred) + (1 - y)·log(1 - y_pred) ]
Where:

- m is the number of training examples

- y is the actual label (0 or 1)

- y_pred is the predicted probability from the sigmoid function

- The goal is to minimize this cost function using optimization algorithms such as Gradient Descent.

## 📍 K-Nearest Neighbors (KNN)
K-Nearest Neighbors (KNN) is a simple yet powerful algorithm that can be used for both classification and regression tasks.
It relies on the idea that similar data points are likely to have similar outputs.

⚙️ Hyperparameters
KNN has only two main hyperparameters:

- k – the number of nearest neighbors to consider.

- Distance metric – the method used to measure similarity between points (e.g., Euclidean, Manhattan).

🔍 Choosing k
The optimal value of k can be determined using the Elbow Method, where the model’s accuracy is evaluated for different k values, and the point where accuracy improvement slows down is selected.

🛠 How It Works
- 1-Initialization – choose k and a distance metric.

- 2-Distance Calculation – compute the distance between the new point and all training points.

- 3-Sorting – arrange points from closest to farthest.

- 4-Prediction:
  
- Classification: take the majority label among the k nearest neighbors.
If there is a tie, select the label with the smallest average distance.

- Regression: take the average value of the k nearest neighbors.

