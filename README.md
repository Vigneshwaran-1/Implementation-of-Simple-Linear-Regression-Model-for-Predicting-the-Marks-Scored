# Implementation-of-Simple-Linear-Regression-Model-for-Predicting-the-Marks-Scored

## AIM:
To write a program to predict the marks scored by a student using the simple linear regression model.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Jupyter notebook

## Algorithm
1. 
2. 
3. 
4. 

## Program:
```
/*
Program to implement the simple linear regression model for predicting the marks scored.
Developed by: Vigneshwaran.P
RegisterNumber: 212224040358
/*

import numpy as np
import pandas as pd
from sklearn.metrics import mean_absolute_error,mean_squared_error
import matplotlib.pyplot as plt
from sklearn.model_selection import train_test_split
from sklearn.linear_model import LinearRegression

dataset = pd.read_csv('/content/student_scores (1).csv')
print(dataset.head())
print(dataset.tail()

dataset.info()

x = dataset.iloc[:,:-1].values
print(x)
Y = dataset.iloc[:,-1].values
print(Y)

x_s=x.shape
y_s=Y.shape
print(x_s)
print(y_s)

x_train,x_test,y_train,y_test = train_test_split(x,Y,test_size=1/3,random_state=1)
print(x_train.shape)
print(x_test.shape)
print(y_train.shape)
print(y_test.shape)

reg=LinearRegression()
reg.fit(x_train,y_train)
y_pred=reg.predict(x_test)
print(y_pred)
print(y_test)

mse=mean_squared_error(y_test,y_pred)
mae=mean_absolute_error(y_test,y_pred)
rmse=np.sqrt(mse)
print('MAE=',mae)
print('MSE=',mse)
print('RMSE=',rmse)

plt.scatter(x_test,y_test,color="blue")
plt.plot(x_test,y_pred,color="red")
plt.show()
*/
*/
```

## Output:
<img width="256" height="280" alt="image" src="https://github.com/user-attachments/assets/30697ede-42bb-4732-9eaf-7d3f659cccd3" />

<img width="724" height="523" alt="image" src="https://github.com/user-attachments/assets/36496686-9903-4b4f-a5df-7a8c1df7a0f4" />


## Result:
Thus the program to implement the simple linear regression model for predicting the marks scored is written and verified using python programming.
