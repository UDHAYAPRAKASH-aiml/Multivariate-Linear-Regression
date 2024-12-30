# Implementation of Multivariate Linear Regression
## Aim
To write a python program to implement multivariate linear regression and predict the output.
## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:
Step1
import pandas as pd

Step2
from sklearn import linear_model

Step3
And then read the csv file

Step4
Then get the input and assume as X and Y

Step5
regression=linear_model.LinearRegression() regression.fit(x,y)

## Program:
```
import pandas as pd
from sklearn import linear_model
df=pd.read_csv("car.csv")
x=df[['Volume','Weight']]
y=df['CO2']
regression=linear_model.LinearRegression()
regression.fit(x,y)
print("Coefficent",regression.coef_)
print("Intercept",regression.intercept_)
print("CO2 required is",regression.predict([[3300,1300]]))

```
## Output:
![ggg](https://github.com/user-attachments/assets/8c11fd36-445a-4492-acb8-d0151e7437ab)


## Result
Thus the multivariate linear regression is implemented and predicted the output using python program.
