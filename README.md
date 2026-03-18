# Implementation-of-Logistic-Regression-Using-Gradient-Descent

## AIM:
To write a program to implement the the Logistic Regression Using Gradient Descent.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Jupyter notebook

## Algorithm
1.Import the necessary python packages
2.Read the dataset.
3.Define X and Y array.
4.Define a function for costFunction,cost and gradient.
5.Define a function to plot the decision boundary and predict the Regression value


## Program:
```
/*
Program to implement the the Logistic Regression Using Gradient Descent.
Developed by: SENASH AYISHA F
RegisterNumber:212225040394
import numpy as np
import matplotlib.pyplot as plt

# Sample dataset
X = np.array([0,1,2,3,4,5,6,7,8,9])
Y = np.array([0,0,0,0,0,1,1,1,1,1])

# Initialize parameters
w = 0
b = 0

learning_rate = 0.01
epochs = 1000
n = len(X)

# Sigmoid function
def sigmoid(z):
    return 1 / (1 + np.exp(-z))

# Gradient Descent
for i in range(epochs):

    # Linear model
    z = w * X + b

    # Prediction
    y_pred = sigmoid(z)

    # Gradients
    dw = (1/n) * np.sum((y_pred - Y) * X)
    db = (1/n) * np.sum(y_pred - Y)

    # Update parameters
    w = w - learning_rate * dw
    b = b - learning_rate * db

print("Weight:", w)
print("Bias:", b)

# Predictions
z = w * X + b
prob = sigmoid(z)

plt.scatter(X, Y, color="blue", label="Actual Data")
plt.plot(X, prob, color="red", label="Logistic Curve")
plt.xlabel("X")
plt.ylabel("Probability")
plt.legend()
plt.show() 
*/
```

## Output:

<img width="565" height="452" alt="image" src="https://github.com/user-attachments/assets/461f2370-1917-45e1-ae9b-9f162219dfa5" />


## Result:
Thus the program to implement the the Logistic Regression Using Gradient Descent is written and verified using python programming.

