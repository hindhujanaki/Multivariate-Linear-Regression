# Implementation of Multivariate Linear Regression
## Aim
To write a python program to implement multivariate linear regression and predict the output.
## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:
### Step1
Get the independent variable X and dependent variable Y.

### Step2
Import pandas as pd and also import linear_model from sklearn module.

### Step3
Read the CSV file which should be atttached to the code runner.

### Step4
Give the commmands to print Liner Regression and also the predicted CO2 for corresponding weights.

### Step5
End the program.

## Program:
```
#Developed by:G.Hindhu
#Register Number:23014493
import pandas as pd
from sklearn import linear_model

df=pd.read_csv('cars.csv')
a=df[['Weight','Volume']]
b=df[['CO2']]
regr=linear_model.LinearRegression()
regr.fit(a,b)
print("Coefficient",regr.coef_)
print("Intercept:",regr.intercept_)
print("Amount:",regr.predict([[3300,1300]])

```
## Output:
![Alt text](<Screenshot 2023-12-31 144431.png>)
## Result
Thus the multivariate linear regression is implemented and predicted the output using python program.