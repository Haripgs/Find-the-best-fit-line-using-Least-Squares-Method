# Implementation of Univariate Linear Regression
## AIM:
To implement univariate Linear Regression to fit a straight line using least squares.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Jupyter notebook

## Algorithm
1. Get the independent variable X and dependent variable Y.
2. Calculate the mean of the X -values and the mean of the Y -values.
3. Find the slope m of the line of best fit using the formula. 
<img width="231" alt="image" src="https://user-images.githubusercontent.com/93026020/192078527-b3b5ee3e-992f-46c4-865b-3b7ce4ac54ad.png">
4. Compute the y -intercept of the line by using the formula:
<img width="148" alt="image" src="https://user-images.githubusercontent.com/93026020/192078545-79d70b90-7e9d-4b85-9f8b-9d7548a4c5a4.png">
5. Use the slope m and the y -intercept to form the equation of the line.
6. Obtain the straight line equation Y=mX+b and plot the scatterplot.

## Program:
```
/*
Program to implement univariate Linear Regression to fit a straight line using least squares.
Developed by: HARIHARAN P
RegisterNumber: 212220040038

import numpy as np
import matplotlib.pyplot as plt
X=np.array([0,1,2,3,4,5,6,7,8,9])
Y=np.array([1,3,2,5,7,8,8,9,10,12])
X_mean=np.mean(X)
print(X_mean)
Y_mean=np.mean(Y)
print(Y_mean)
num=0
denum=0
for i in range(len(X)):
  num+=(X[i]-X_mean)*(Y[i]-Y_mean)
  denum+=(X[i]-X_mean)**2
m=num/denum
print(m)
b=Y_mean - m*X_mean
print(b)
Y_pred=m*X+b
print(Y_pred)
plt.scatter(X,Y,color='purple')
plt.plot(X,Y_pred,color='red') 
plt.show() 

/*
```

## Output:

## Best fit line:
![A](https://user-images.githubusercontent.com/94747031/198823939-10276637-2bad-4aa5-b8db-22763369a789.png)

## Finding Mean of x:
![B](https://user-images.githubusercontent.com/94747031/198823941-524e5d10-8695-4f88-8c65-691c574e1117.png)

## Finding the slope m:
![C](https://user-images.githubusercontent.com/94747031/198823942-67bb0177-3fd3-4b74-80da-751c957285c2.png)

## Finding the y intercept:
![D](https://user-images.githubusercontent.com/94747031/198823943-af52b7ab-e317-4895-aa24-778f5c77972a.png)

## Equation of line:
![E](https://user-images.githubusercontent.com/94747031/198823944-f02b19ef-8b62-408e-b236-7256575140f0.png)

## Finding Mean of y :
![F](https://user-images.githubusercontent.com/94747031/198823946-7e691e4b-d436-432f-a14d-2d2c31364b07.png)


## Result:
Thus the univariate Linear Regression was implemented to fit a straight line using least squares using python programming.
