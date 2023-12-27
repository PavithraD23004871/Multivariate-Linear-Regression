# Implementation of Multivariate Linear Regression
## Aim
To write a python program to implement multivariate linear regression and predict the output.
## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:
### Step1
Get the independent variable Xand dependent variable Y

### Step2
import pandas as pd and also import linear_model from sklearn module

### Step3
Read the CSV file which should be attached to the code runner

### Step4
Give the commands to print 
Linear Regression and also the predicted CO2for corresponding weights

### Step5
End the program

## Program:
```
'''
#Program to implement multivariate linear regression and predict the output.
#Developed by:pavithra.D
#RegisterNumber:23004871
'''
import pandas as pd
from sklearn import linear_model

df = pd.read_csv("cars (1).csv")
X=df[['Weight','Volume']]
Y=df['CO2']
regr=linear_model.LinearRegression()
regr.fit(X,Y)
print('Coefficients:',regr.coef_)
print('Intercept:',regr.intercept_)
predictedCO2=regr.predict([[3300,1300]])
print('Predicted CO2 for the corresponding weight and volume',predictedCO2)





```
## Output:
![WhatsApp Image 2023-12-27 at 18 08 20_a0689cde](https://github.com/PavithraD23004871/Multivariate-Linear-Regression/assets/138955967/cfe7f200-ef06-4f88-8f27-744ada372ef4)

### Insert your output

<br>

## Result
Thus the multivariate linear regression is implemented and predicted the output using python program.
