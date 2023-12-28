# Implementation of Multivariate Linear Regression
## Aim
To write a python program to implement multivariate linear regression and predict the output.
## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:
### Step1
<br>
Import pandas.
### Step2
Impor linear model from sklearn.

### Step3
Read the files cars.csv.

### Step4
Assign the values for x and y as requried.

### Step5
Create the LinearRegression model and predict the output
## Program:
```
Developed by: Logesh.N.A
RegisterNumber: 23012242

import pandas as pd
from sklearn import linear_model
df=pd.read_csv('cars.csv')
x=df[['Weight','Volume']]
y=df['CO2']
regr=linear_model.LinearRegression()
regr.fit(x,y)
print("Coefficient:",regr.coef_)
print("Intercept:",regr.intercept_)
predictedCO2=regr.predict([[3300,1300]])
print("Predicted CO2 for the corresponding weight and volume",predictedCO2)

```
## Output:
![Screenshot 2023-12-28 200159](https://github.com/Logesh051/Multivariate-Linear-Regression/assets/144979188/20264908-68a5-4c9f-adbb-ee0dcdcf4e3d)

## Result
Thus the multivariate linear regression is implemented and predicted the output using python program.
