# Implementation of Multivariate Linear Regression
## Aim
To write a python program to implement multivariate linear regression and predict the output.
## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:
### Step1
Import pandas as pd.

### Step2
Read the CSV file.

### Step3
Get the value of X and Y variables.

### Step4
Create the linear regression model and fit.

### Step5
Predict the CO2 emission of a car where the weight is 3300kg, and the volume is 1300cm3.

## step6
Print the predicted output.

## Program:
```PYTHON
##Developed by : RIYA P L
##Register no : 23005672

import pandas as pd
from sklearn import linear_model
df=pd.read_CSV("cars,CSV")
x=df[['Weight','Volume']]
y=df['CO2']
regr=linear_model.LinearRegression()
regr.fit(x,y)
print("Coefficient:",regr.coef_)
print("Intercept:",regr.intercept_)
predictedCO2=regr.predict([[3300,1300]])
print("Predicted CO@ for the corresponding weight and volume",predictedCO2)






```
## Output:
<img width="713" alt="Screenshot 2023-12-24 152032" src="https://github.com/23005672/Multivariate-Linear-Regression/assets/138971519/6afdd885-997a-4de5-bf98-983d3b13df49">



## Result
Thus the multivariate linear regression is implemented and predicted the output using python program.
