# Implementation of Multivariate Linear Regression
## Aim
To write a python program to implement multivariate linear regression and predict the output.
## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:
### Step1
<br>
Import pandas as pd.

### Step 2:
Read the csv file.
<br>
### Step 3:
Get the value of X and y variables.
<br>
### Step 4:
Create the linear regression model and fit.
<br>
### Step 5:
Predict the CO2 emission of a car where the weight is 3300kg, and the volume is 1300cm3.
<br>


## Program:
```
#Developed by: RAVI TEJA ROYAL
#Registration no: 25011599

import pandas as pd
from sklearn import linear_model
df=pd.read_csv('cars.csv')
a=df[['Weight', 'Volume']]
b=df[['CO2']]
regr=linear_model.LinearRegression()
regr.fit(a,b)
print("coefficient",regr.coef_)
print("Intercept:", regr.intercept_)
print("Amount:", regr.predict([[3300,1300]]))


```
## Output:
<img width="853" height="637" alt="image" src="https://github.com/user-attachments/assets/0594705d-5474-49b7-9eb6-cf427082af97" />


## Result
Thus the multivariate linear regression is implemented and predicted the output using python program.
