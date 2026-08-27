# Implementation of Multivariate Linear Regression
## Aim
To write a python program to implement multivariate linear regression and predict the output.
## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:
###Steps:
Step1
import pandas as pd.

Step2
Read the csv file.

Step3
Get the value of X and y variables

Step4
Create the linear regression model and fit.


## Program:
```
Developed by: S.RISITHA
Register no: 212225240119

import pandas as pd
from sklearn import linear_model
df = pd.read_csv("car.csv")
X = df[['Weight', 'Volume']]
y = df['CO2']
regr = linear_model.LinearRegression()
regr.fit(X, y)
print('Coefficients:', regr.coef_)
print('Intercept:', regr.intercept_)
predictedCO2 = regr.predict(pd.DataFrame([[3300, 1300]], columns=['Weight', 'Volume']))
print('Predicted CO2 for the corresponding weight and volume:', predictedCO2)






```
## Output:

<img width="615" height="62" alt="image" src="https://github.com/user-attachments/assets/495ea97d-f7be-4d17-bb1b-15f8dbd7ddcf" />


## Result
Thus the multivariate linear regression is implemented and predicted the output using python program.
