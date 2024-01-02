## Aim
To write a python program to implement multivariate linear regression and predict the output.
## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:
### Step 1
Import pandas as pd.

### Step 2
Read the csv file.

### Step 3
Get the value of X and y variables.

### Step 4
Create the linear regression model and fit.

### Step 5
Predict the CO2 emission of a car where the weight is 2300kg, and the volume is 1300cm cube.

## Program:
```
#Developed by: HARIHARAN J
#Reference number:212223240047
from sklearn import linear_model
df=pd.read_csv("cars.csv")
a=df[['Weight','Volume']]
b=df[['CO2']]
regr=linear_model.LinearRegression()
regr.fit(a,b)
print("Coefficient: ",regr.coef_)
print("Intercept:",regr.intercept_)
print("Account",regr.predict([[3300,1300]]))

```
## Output:
![image](https://github.com/etjabajasphin/Multivariate-Linear-Regression/assets/144870546/551c2334-e61a-4ebc-a69b-976d5287c51c)

## Result
Thus the multivariate linear regression is implemented and predicted the output using python program.
