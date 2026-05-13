# Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn

## AIM:
To write a program to implement the Decision Tree Classifier Model for Predicting Employee Churn.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Jupyter notebook

## Algorithm
1. Load the employee dataset and convert categorical data into numerical format using `get_dummies()`.
2. Split the dataset into training data and testing data using `train_test_split()`.
3. Train the `DecisionTreeClassifier` model using the training dataset.
4. Predict the test data results, calculate accuracy, and display the decision tree graph.
 

## Program:
```
/*
Program to implement the Decision Tree Classifier Model for Predicting Employee Churn.

import pandas as pd
import matplotlib.pyplot as plt
from sklearn.model_selection import train_test_split
from sklearn.tree import DecisionTreeClassifier, plot_tree
from sklearn.metrics import accuracy_score
data = pd.read_csv("Employee.csv")
data = pd.get_dummies(data, drop_first=True)
X = data.iloc[:, :-1]
y = data.iloc[:, -1]
X_train, X_test, y_train, y_test = train_test_split(
    X, y, test_size=0.2, random_state=42
)
model = DecisionTreeClassifier(random_state=42)
model.fit(X_train, y_train)
y_pred = model.predict(X_test)
print("Accuracy:", accuracy_score(y_test, y_pred))
plt.figure(figsize=(20,10))

plot_tree(
    model,
    feature_names=X.columns,
    filled=True
)

plt.show()

Developed by: MADHU .P
RegisterNumber: 212225040215 
*/
```

## Output:
<img width="1378" height="709" alt="WhatsApp Image 2026-05-13 at 9 24 40 AM" src="https://github.com/user-attachments/assets/6392879b-4f90-4c2b-b7ba-5a6acc25b347" />



## Result:
Thus the program to implement the  Decision Tree Classifier Model for Predicting Employee Churn is written and verified using python programming.
