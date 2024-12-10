# Implementation of Multivariate Linear Regression
## Aim
To write a python program to implement multivariate linear regression and predict the output.
## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:
### Step1
<br>Import the pandas module.

### Step2
<br>Read the csv file.

### Step3
<br>Get the value of X and y variables.

### Step4
<br>Create the linear aggression model and fit.

### Step5
<br>Predict the CO2 emission of a car where the weight is 2300kg, and the volume is 1300cm cube.Predict the Output 

## Program:
```
import pandas as pd
from sklearn import linear_model
df = pd.read_csv("carsemmsion.csv")
X = df[['Weight', 'Volume']]
y = df['CO2']
regr = linear_model.LinearRegression()
regr.fit(X, y)
print('Coefficients:', regr.coef_)
print('Intercept:', regr.intercept_)
input_data = pd.DataFrame({'Weight': [3300], 'Volume': [1300]})
predictedCO2 = regr.predict(input_data)
print('Predicted CO2 for the corresponding weight and volume:', predictedCO2)






```
## Output:



### Insert your output

<br>![image](https://github.com/user-attachments/assets/5e4e4658-e33f-47fe-8630-ca43bab64271)


## Result
Thus the multivariate linear regression is implemented and predicted the output using python program.
