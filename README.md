# Implementation of Univariate Linear Regression
## Aim:
To implement univariate Linear Regression to fit a straight line using least squares.
## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:
1.	Get the independent variable X and dependent variable Y.
2.	Calculate the mean of the X -values and the mean of the Y -values.
3.	Find the slope m of the line of best fit using the formula.
 ![eqn1](./eq1.jpg)
4.	Compute the y -intercept of the line by using the formula:
![eqn2](./eq2.jpg)  
5.	Use the slope m and the y -intercept to form the equation of the line.
6.	Obtain the straight line equation Y=mX+b and plot the scatterplot.
## Program
```
import numpy as np

# Preprocessing Input data

X = np.array(eval(input()))
Y = np.array(eval(input()))
x_mean=np.mean(X)
y_mean=np.mean(Y)
num=0
den=0
for i in range(len(X)):
    num+=(X[i]-x_mean)*(Y[i]-y_mean)
    den+=(X[i]-x_mean)**2
m=num/den
b=y_mean-m*x_mean
    
# Building the model
# write your code here

print (m, b)

y=m*X+b
print(y)






```
## Sample Input and Output
![OUTPUT](H1.png)

![OUTPUT](H2.jpeg)
## Result
Thus the univariate Linear Regression was implemented to fit a straight line using least squares.
