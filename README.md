# Implementation of Multivariate Linear Regression
## Aim
To write a python program to implement multivariate linear regression and predict the output.
## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:
### Step1
import pandas as pd
<br>

### Step2
Read the csv file
<br>

### Step3
Get the value of X and Y variables
<br>

### Step4
Create the linear regression model and fit
<br>

### Step5
Predict the CO2 emission of a car where the weight is 2300kg, and the volume is 1300cm cube.
<br>

## Program:
```python
## Developed by : Gumma Dileep Kumar
## Reg.No : 22007129


import pandas as pd 
from sklearn import linear_model

df = pd.read_csv("carsemission.csv")

X = df[['Weight','Volume']]
Y = df['CO2']

regr = linear_model.LinearRegression()
regr.fit(X,Y)

print('Coefficient:', regr.coef_)
print('Intercept:',regr.intercept_)

precidtedCO2 = regr.predict([[3300, 1300]])
print('Predicted CO2 for the corresponding weight and volume ',predictCO2)






```
## Output:
![multivate_output](https://user-images.githubusercontent.com/118707761/214606282-f50e15e8-bb1d-4f66-8815-34a9b772a99f.jpg)



<br>

## Result
Thus the multivariate linear regression is implemented and predicted the output using python program.
