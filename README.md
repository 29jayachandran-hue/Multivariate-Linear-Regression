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
import numpy as np
import matplotlib.pyplot as plt
X = np.array(eval(input()))
Y = np.array(eval(input()))
Xmean = np.mean(X)
Ymean = np.mean(Y)
num,den = 0,0
for i in range(len(X)):
    num += (X[i]-Xmean)*(Y[i]-Ymean)
    den += (X[i]-Xmean)**2
m = num/den
c = Ymean-m*Xmean   
print (m, c)
Y_pred = m*X + c
print (Y_pred)
plt.scatter(X,Y)
plt.plot(X,Y_pred,color="red")
plt.show()
```
## Output:
<img width="721" height="617" alt="image" src="https://github.com/user-attachments/assets/3eba5842-3a6c-4c52-b568-9d4df9cda0f8" />

## Result
Thus the multivariate linear regression is implemented and predicted the output using python program.
