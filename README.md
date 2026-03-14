# BLENDED_LEARNING
# Implementation of Decision Tree Model for Tumor Classification

## AIM:
To implement and evaluate a Decision Tree model to classify tumors as benign or malignant using a dataset of lab test results.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Jupyter notebook

## Algorithm
1. Import required libraries such as pandas, sklearn DecisionTreeClassifier, train_test_split, and evaluation metrics.

2. Load the dataset tumor.csv and separate the input features (X) and target variable (Class).

3. Split the dataset into training and testing sets using train_test_split().

4. Train the Decision Tree Classifier model using the training data.

5. Predict the test data and evaluate the model using accuracy, classification report, and confusion matrix visualization.


## Program:
```
/*
Program to  implement a Decision Tree model for tumor classification.

import pandas as pd
from sklearn.model_selection import train_test_split
from sklearn.tree import DecisionTreeClassifier
import seaborn as sns
import matplotlib.pyplot as plt
from sklearn.metrics import accuracy_score, classification_report, confusion_matrix

data=pd.read_csv("tumor.csv")
print(data.head())
print(data.columns)

x=data.drop(columns=['Class'])
y=data['Class']

x=data[features]
y=data[target]
x_train,x_test,y_train,y_test=train_test_split(x,y,test_size=0.3,random_state=42)

model=DecisionTreeClassifier()
model.fit(x_train,y_train)

y_pred=model.predict(x_test)

accuracy=accuracy_score(y_test,y_pred)
print("Name: Lakshiya Rajkumar")
print("Register Number:212225240076")
print("Accuracy:",accuracy)
print("Classification Report:\n",classification_report(y_test,y_pred))

conf_matrix=confusion_matrix(y_test,y_pred)
sns.heatmap(conf_matrix,annot=True,fmt="d",cmap="Blues")
plt.xlabel("Predicted")
plt.ylabel("Actual")
plt.title("Confusion Matrix")
plt.show()


Developed by: Lakshiya Rajkumar
RegisterNumber:  212225240076
*/
```

## Output:
![alt text](<Screenshot 2026-03-14 123606.png>)
![alt text](<Screenshot 2026-03-14 123622.png>)
![alt text](<Screenshot 2026-03-14 123640.png>)


## Result:
Thus, the Decision Tree model was successfully implemented to classify tumors as benign or malignant, and the model’s performance was evaluated.
