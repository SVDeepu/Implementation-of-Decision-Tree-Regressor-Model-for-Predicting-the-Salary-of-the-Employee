# Implementation-of-Decision-Tree-Regressor-Model-for-Predicting-the-Salary-of-the-Employee

## AIM:
To write a program to implement the Decision Tree Regressor Model for Predicting the Salary of the Employee.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Jupyter notebook

## Algorithm

1.Import dataset and get data info

2.check for null values

3.Map values for position column

4.Split the dataset into train and test set

5.Import decision tree regressor and fit it for data

6.Calculate MSE,R2 and y predict

## Program:
```
/*
Program to implement the Decision Tree Regressor Model for Predicting the Salary of the Employee.
Developed by: SV.DEEPIKA
RegisterNumber: 212220040161
import pandas as pd
data=pd.read_csv("/content/Salary.csv")
data.head()
data.info()
data.isnull().sum()
from sklearn.preprocessing import LabelEncoder
le=LabelEncoder()
data["Position"]=le.fit_transform(data["Position"])
data.head()
x=data[["Position","Level"]]
y=data[["Salary"]]
from sklearn.model_selection import  train_test_split
x_train,x_test,y_train,y_test=train_test_split(x,y,test_size=0.2,random_state=2)
from sklearn.tree import DecisionTreeRegressor
dt=DecisionTreeRegressor()
dt.fit(x_train,y_train)
y_pred=dt.predict(x_test)
from sklearn import metrics
mse=metrics.mean_squared_error(y_test,y_pred)
mse
r2=metrics.r2_score(y_test,y_pred)
r2
dt.predict([[5,6]])
*/
```

## Output:
![7 1](https://user-images.githubusercontent.com/114275126/204461722-62d93aad-b1c8-431a-85fc-9694145a5991.PNG)

![7 2](https://user-images.githubusercontent.com/114275126/204461791-59c7c22f-9e40-4cae-b2d3-05ad474939fe.PNG)

![7 3](https://user-images.githubusercontent.com/114275126/204461842-7007cd6f-7f95-4b44-84ac-360231768870.PNG)

![7 4](https://user-images.githubusercontent.com/114275126/204461869-adb455c8-fc61-4683-b333-db13d02a696b.PNG)

![7 5](https://user-images.githubusercontent.com/114275126/204461903-30003087-f033-409c-b18c-82ba939bfbb0.PNG)

![7 6](https://user-images.githubusercontent.com/114275126/204461935-59ee342b-a12e-42cb-bf56-7e97e6a319cc.PNG)

![7 7](https://user-images.githubusercontent.com/114275126/204461953-e053dcc4-037b-45dc-99b3-bf713425df71.PNG)

![7 8](https://user-images.githubusercontent.com/114275126/204461973-2b5d87cb-e637-4a12-814d-32f3e484ab0a.PNG)

## Result:
Thus the program to implement the Decision Tree Regressor Model for Predicting the Salary of the Employee is written and verified using python programming.
