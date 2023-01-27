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
Read the csv file.

### Step3
Get the value of X and y variables.

### Step4
Create the linear regression model and fit.

### Step5
Predict the CO2 emission of a car where the weight is 1000kg, and the volume is 1390cm3.
###Step 6
Print the predicted output.
## Program:
```
##Developed by: C Saravanan
##REGISTER NUMBER: 22008175

import pandas as pd
from sklearn import linear_model
df = pd.read_csv("cars.csv")
X = df[['Weight', 'Volume']]
y = df['CO2']
regr = linear_model.LinearRegression()
regr.fit(X, y)
print('Coefficients:', regr.coef_)
print('Intercept:',regr.intercept_)
predictedCO2 = regr.predict([[3300, 1300]])
print('Predicted CO2 for the corresponding weight and volume',predictedCO2)

```
## Output:
![image](https://user-images.githubusercontent.com/121395849/215153372-e4c8deec-1b15-40b6-abe9-1c29ee6f9406.png)
## Result
Thus the multivariate linear regression is implemented and predicted the output using python program.
