# Implementation of Multivariate Linear Regression
## Aim
To write a python program to implement multivariate linear regression and predict the output.
## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:
### Step1
Import pandas as pd
### Step2
Read the csv file

### Step3
Get the value of the x and y variables

### Step4
Create the linear regression model and fit.

### Step5
Predict the CO2 emission of a car where the weight is 3300kg and the volume is 1300cm^3.

## Program:
```
# program for multivariate linear regression
# Developed by: Muthu Kumaran M
# reference number:212223240101

import pandas as pd
from sklearn import linear_model
data=pd.read_csv("cars.csv")
x=data[['Weight','Volume']]
y=data[['CO2']]
regr=linear_model.LinearRegression()
regr.fit(x,y)
print('Coefficients:',regr.coef_)
print('Intercept:',regr.intercept_)
predictCO2=regr.predict([[3300,1300]])
print('predicted CO2 for the corresponding weight and volume',predictCO2)
```
## Output:
![Exp 10](https://github.com/Muthu-Kumaran-M/Multivariate-Linear-Regression/assets/144979439/a33f74c0-a65d-40f7-9d9d-2a1b512ee330)

## Result
Thus the multivariate linear regression is implemented and predicted the output using python program.
