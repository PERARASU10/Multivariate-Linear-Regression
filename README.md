# Implementation of Multivariate Linear Regression
## Aim
To write a python program to implement multivariate linear regression and predict the output.
## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:
Step1
Import panda module as pd

Step2
Import linear model from sklearn

Step3
Read the file cars.csv

Step4
Assign the values for x and y as required

Step5
Create the linearRegression model and predict the output

## Program:
```
'''
Developed by: PERARASU M
Register number: 212222100033
'''
import pandas as pd
from sklearn import linear_model
df=pd.read_csv("cars.csv")
a=df[['Weight','Volume']]
b=df[['CO2']]
regr=linear_model.LinearRegression()
regr.fit(a,b)
print("Coefficient:",regr.coef_)
print("Intercept:",regr.intercept_)
print("Amount:",regr.predict([[3300,1300]]))






```
## Output:
![image](https://github.com/PERARASU10/Multivariate-Linear-Regression/assets/118348589/6447f18e-9004-4d42-b7cf-de4af01f0f35)

## Result
Thus the multivariate linear regression is implemented and predicted the output using python program.
