# Implementation of Multivariate Linear Regression
## Aim
To write a python program to implement multivariate linear regression and predict the output.
## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:
### Step1
Import pandas as pd and sklearn into that import linear_model, by importing pandas and sklearn from python library.

### Step2
Use pandas inbuilt function to get and input csv file from user using pd.read_csv(path of csv file) command.


### Step3
From dataset select dependent variable and one independent variable to and to find the relationship of one more two independent variables.

### Step4
Use linearmodel into that use linear regression function to compute the variables.

### Step5
Use regression.fit function of inputted variables of x and y and print corresponding results to get output.

## Program:
```
Developed by: SHREEDHAR KUMAR K.J
Reg.No: 24901118
import pandas as pd
from sklearn import linear_model
df = pd.read_csv("carsemission.csv")
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
![image](https://github.com/user-attachments/assets/22d08f95-65b2-4fdc-9950-8cdac9471ca7)


## Result
Thus the multivariate linear regression is implemented and predicted the output using python program.
