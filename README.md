# Implementation of Multivariate Linear Regression
## Aim
To write a python program to implement multivariate linear regression and predict the output.
## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:
### Step1 
Import Libraries and Load Dataset Import the required Python libraries and load the California Housing dataset.

### Step2
Define Input and Output Variables Store the feature matrix in X and target values in y.

### Step3
Split the Dataset Divide the dataset into training and testing sets using train_test_split().

### Step4
Create and Train the Linear Regression Model Create a Linear Regression object and train it using the training data.

### Step5
Predict and Plot Residual Errors Predict the output values, calculate residual errors, and display the residual error graph using Matplotlib.

## Program:
```
import pandas as pd
from sklearn import linear_model
df=pd.read_csv("car (1).csv")
x=df[["Volume","Weight"]]
y=df["CO2"]
regression=linear_model.LinearRegression()
regression.fit(x,y)
print(regression.coef_)
print(regression.intercept_)
print(regression.predict([[3300,1300]]))
```
## Output:
<img width="1357" height="315" alt="image" src="https://github.com/user-attachments/assets/f45340bd-875b-42f7-8498-a7311a05a2c3" />


## Result
Thus the multivariate linear regression is implemented and predicted the output using python program.
