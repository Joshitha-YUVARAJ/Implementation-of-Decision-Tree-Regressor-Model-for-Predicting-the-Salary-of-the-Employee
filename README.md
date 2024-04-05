# Implementation-of-Decision-Tree-Regressor-Model-for-Predicting-the-Salary-of-the-Employee

## AIM:
To write a program to implement the Decision Tree Regressor Model for Predicting the Salary of the Employee.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Jupyter notebook

## Algorithm
1.Import the required libraries.

2.Upload the csv file and read the dataset.

3.Check for any null values using the isnull() function.

4.From sklearn.tree import DecisionTreeRegressor.

5.Import metrics and calculate the Mean squared error.

6.Apply metrics to the dataset, and predict the output.

## Program:
```
/*
Program to implement the Decision Tree Regressor Model for Predicting the Salary of the Employee.
Developed by:YUVARAJ JOSHITHA 
RegisterNumber: 212223240189
import pandas as pd
data = pd.read_csv("Salary.csv")
data.head()
data.info()
data.isnull().sum()
from sklearn.preprocessing import LabelEncoder
le = LabelEncoder()
data["Position"] = le.fit_transform(data["Position"])
data.head()
x = data[["Position","Level"]]
y = data["Salary"]
from sklearn.model_selection import train_test_split
x_train,x_test,y_train,y_test = train_test_split(x,y,test_size=0.2,random_state=2)
from sklearn.tree import DecisionTreeRegressor
dt = DecisionTreeRegressor()
dt.fit(x_train,y_train)
y_pred = dt.predict(x_test)
from sklearn import metrics
mse = metrics.mean_squared_error(y_test,y_pred)
mse
r2 = metrics.r2_score(y_test,y_pred)
r2
dt.predict([[5,6]]) 
*/
```

## Output:
# DATA HEAD
![image](https://github.com/Joshitha-YUVARAJ/Implementation-of-Decision-Tree-Regressor-Model-for-Predicting-the-Salary-of-the-Employee/assets/145742770/2ed7b389-62ec-4d47-ab82-d6e4f1e9995e)
# DATA INFO
![image](https://github.com/Joshitha-YUVARAJ/Implementation-of-Decision-Tree-Regressor-Model-for-Predicting-the-Salary-of-the-Employee/assets/145742770/baae15fd-3073-4dc1-9163-efcd12a3209a)
# NULL DATA:
![image](https://github.com/Joshitha-YUVARAJ/Implementation-of-Decision-Tree-Regressor-Model-for-Predicting-the-Salary-of-the-Employee/assets/145742770/065a18aa-5695-466e-b903-efc1870d8bc4)

# Data Head after applying LabelEncoder():
![image](https://github.com/Joshitha-YUVARAJ/Implementation-of-Decision-Tree-Regressor-Model-for-Predicting-the-Salary-of-the-Employee/assets/145742770/349bb6b8-b6e0-4424-bc71-37f7d7cff963)
# MSE:
![Screenshot 2024-04-05 094729](https://github.com/Joshitha-YUVARAJ/Implementation-of-Decision-Tree-Regressor-Model-for-Predicting-the-Salary-of-the-Employee/assets/145742770/c5cce21f-5d44-4385-80a5-b00fab1ba46a)

# R2:
![Screenshot 2024-04-05 094738](https://github.com/Joshitha-YUVARAJ/Implementation-of-Decision-Tree-Regressor-Model-for-Predicting-the-Salary-of-the-Employee/assets/145742770/4116537a-97e9-48cf-a722-3f63b7e784a3)

# DATA PREDICTION:
![Screenshot 2024-04-05 094756](https://github.com/Joshitha-YUVARAJ/Implementation-of-Decision-Tree-Regressor-Model-for-Predicting-the-Salary-of-the-Employee/assets/145742770/5b848d52-9690-4f39-927b-4ac1122dc7c9)



## Result:
Thus the program to implement the Decision Tree Regressor Model for Predicting the Salary of the Employee is written and verified using python programming.
